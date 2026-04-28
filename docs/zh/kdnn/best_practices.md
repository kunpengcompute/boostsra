# 最佳实践

## 适配TensorFlow

本章节提供KDNN适配TensorFlow中矩阵算子（MatMul和FusedMatMul对应KDNN的Gemm算子）的方法。请参照本章节内容操作，若操作不当，可能会引入未定义行为，请谨慎操作。

1. 安装基础软件。

    ```bash
    yum install gcc g++ zip python vim tar wget unzip 
    ```

2. 请参见《TensorFlow 移植指南》中的“[安装Bazel](https://www.hikunpeng.com/document/detail/zh/SRA/ecosystemEnable/TensorFlow/kunpengtensorflow_02_0008.html)”安装Bazel。TensorFlow编译时需要使用Bazel工具，TensorFlow 2.15.0依赖的Bazel版本为6.5.0，请下载Bazel 6.5.0版本。
3. 从GitHub下载开源TensorFlow 2.15.0版本。

    ```bash
    git clone -b v2.15.0 https://github.com/tensorflow/tensorflow.git 
    ```

4. 从GitCode下载优化补丁并合入开源TensorFlow目录中。

    ```bash
    git clone -b v2.15.0-2512 https://gitcode.com/boostkit/tensorflow.git sra-tensorflow 
    cp /path/to/sra-tensorflow/0001-boostsra-tensorflow.patch /path/to/tensorflow/ 
    cd /path/to/tensorflow && patch -p1 < 0001-boostsra-tensorflow.patch
    ```

5. 安装依赖组件。

    ```bash
    yum install patchelf perl python3-devel
    pip3 install numpy==1.24.3
    pip3 install certifi==2023.7.22
    pip3 install requests==2.31.0
    pip3 install grpcio==1.59.0
    pip3 install packaging
    pip3 install wheel
    export C_INCLUDE_PATH=/usr/include/python3.9:$C_INCLUDE_PATH
    export CPLUS_INCLUDE_PATH=/usr/include/python3.9:$CPLUS_INCLUDE_PATH
    ```

    上述配置环境变量命令中的路径“/usr/include/python3.9”为Python.h所在目录，用户操作过程中请以实际编译环境中的路径为准。

6. 准备KDNN头文件和静态库。

    ```bash
    cd /path/to/tensorflow/third_party/KDNN
    cp -r /usr/local/kdnn/include .
    mkdir -p src && cp /usr/local/kdnn/lib/threadpool/libkdnn.a src
    ```

7. 进入KDNN目录并合入头文件补丁，解决TensorFlow不支持exception机制问题。

    ```bash
    patch -p0 < tensorflow_kdnn_include_adapter.patch
    ```

8. 返回TensorFlow根目录，构建配置。请参见《TensorFlow 移植指南》中的“[源码编译安装](https://www.hikunpeng.com/document/detail/zh/SRA/ecosystemEnable/TensorFlow/kunpengtensorflow_02_0009.html)”章节配置编译选项。

    ```bash
    cd ../..
    ./configure
    ```

9. 开始构建。

    ```bash
    export TF_PYTHON_VERSION=3.9
    bazel --output_user_root=../output build -c opt --define=enable_kdnn=true //tensorflow/tools/pip_package:build_pip_package
    ```

    其中“../output”为指定的构建输出目录。

10. 安装pip包。

    ```bash
    ./bazel-bin/tensorflow/tools/pip_package/build_pip_package ./output-kdnn
    pip3 install ./output-kdnn/tensorflow-2.15.0-cp39-cp39-linux_aarch64.whl
    ```

## 适配oneDNN

本章节提供KDNN适配oneDNN的方法，请参照本章节内容操作。若操作不当，可能会引入未定义行为，请谨慎操作。

**适配步骤<a name="section39201312169"></a>**

1. 获取oneDNN适配代码。假设“/path/to”为当前拉取代码路径。

    ```bash
    git clone -b v3.1.0 https://gitcode.com/openeuler/kail_dnn_adapter.git
    cd kail_dnn_adapter
    git submodule update --init --recursive
    cd oneDNN-open
    ulimit -n 262144
    patch -p1 < ../0001-kdnn-adapter.patch
    ```

2. 进入“/path/to/kail\_dnn\_adapter“”录，编译oneDNN。

    - 鲲鹏920 7280Z处理器

        ```bash
        cd /path/to/kail_dnn_adapter
        sh build.sh --use_static_kdnn=off
        ```

        选项“--use\_static\_kdnn=on/off”指定编译时使用KDNN静态库或者动态库，默认为“off”。

    - 鲲鹏920新型号处理器（以毕昇编译器为例）

        ```bash
        cd /path/to/kail_dnn_adapter
        sh build.sh --compiler=clang
        ```

    编译产物路径。

    libdnnl.so路径为：“out/oneDNN-open/build/src/”

    其依赖库的路径如下：

    - ACL库相关so路径：“out/ComputeLibrary-23.11/build/”
    - AI库相关so路径：“/usr/local/kdnn/lib/omp/libkdnn.so”

    单独链接libdnnl.so可以得到oneDNN v3.4.0的全部接口功能。

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >编译命令中，“--compiler=clang”表示使用毕昇编译器，默认使用GCC。

**适配后验证<a name="section193111321616"></a>**

编译完成后，使用软件自带的测试用例运行和验证是否适配成功。

1. 进入“/path/to/kail\_dnn\_adapter/out/llt/scripts”目录。

    ```bash
    cd /path/to/kail_dnn_adapter/out/llt/scripts
    ```

2. 运行测试用例。

    ```bash
    python run_daily_build.py --working_dir=../../oneDNN-open/build/tests/benchdnn
    ```

    如果用例执行结果全部为**passed**，并且有如下图所示信息返回，说明oneDNN适配成功。

    ![](figures/zh-cn_image_0000002549872587.png)
