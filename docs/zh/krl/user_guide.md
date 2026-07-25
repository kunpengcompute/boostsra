# 用户指南

## 已验证环境

为保证您可以顺利安全地使用KRL，请确保所使用的环境信息在已验证环境范围内。

**表 1** KRL已验证环境<a id="KRL已验证环境"></a>

<a name="table113653362525"></a>
<table><thead align="left"><tr id="row2036563612525"><th class="cellrowborder" valign="top" width="21.77%" id="mcps1.2.6.1.1"><p id="p10365836165218"><a name="p10365836165218"></a><a name="p10365836165218"></a>操作系统</p>
</th>
<th class="cellrowborder" valign="top" width="23.5%" id="mcps1.2.6.1.2"><p id="p53652363523"><a name="p53652363523"></a><a name="p53652363523"></a>CPU类型</p>
</th>
<th class="cellrowborder" valign="top" width="18.44%" id="mcps1.2.6.1.3"><p id="p136510367522"><a name="p136510367522"></a><a name="p136510367522"></a>内存</p>
</th>
<th class="cellrowborder" valign="top" width="16.900000000000002%" id="mcps1.2.6.1.4"><p id="p20365836185215"><a name="p20365836185215"></a><a name="p20365836185215"></a>编译器</p>
</th>
<th class="cellrowborder" valign="top" width="19.39%" id="mcps1.2.6.1.5"><p id="p6365123615524"><a name="p6365123615524"></a><a name="p6365123615524"></a>CMake</p>
</th>
</tr>
</thead>
<tbody><tr id="row10365113685217"><td class="cellrowborder" valign="top" width="21.77%" headers="mcps1.2.6.1.1 "><p id="p1636573614523"><a name="p1636573614523"></a><a name="p1636573614523"></a>openEuler 22.03 LTS SP3</p>
</td>
<td class="cellrowborder" valign="top" width="23.5%" headers="mcps1.2.6.1.2 "><p id="p173654366528"><a name="p173654366528"></a><a name="p173654366528"></a>鲲鹏920 7282C处理器</p>
</td>
<td class="cellrowborder" valign="top" width="18.44%" headers="mcps1.2.6.1.3 "><p id="p636533625218"><a name="p636533625218"></a><a name="p636533625218"></a>16 * 32G</p>
</td>
<td class="cellrowborder" valign="top" width="16.900000000000002%" headers="mcps1.2.6.1.4 "><p id="p103651036185219"><a name="p103651036185219"></a><a name="p103651036185219"></a>GCC 12.3.1</p>
</td>
<td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.6.1.5 "><p id="p285111515577"><a name="p285111515577"></a><a name="p285111515577"></a>&gt;=3.22.0</p>
</td>
</tr>
<tr id="row10335834165819"><td class="cellrowborder" valign="top" width="21.77%" headers="mcps1.2.6.1.1 "><p id="p7336183465815"><a name="p7336183465815"></a><a name="p7336183465815"></a>openEuler 24.03 LTS SP3</p>
</td>
<td class="cellrowborder" valign="top" width="23.5%" headers="mcps1.2.6.1.2 "><p id="p15336103415817"><a name="p15336103415817"></a><a name="p15336103415817"></a>鲲鹏950 7592C处理器</p>
</td>
<td class="cellrowborder" valign="top" width="18.44%" headers="mcps1.2.6.1.3 "><p id="p233663465818"><a name="p233663465818"></a><a name="p233663465818"></a>24 * 64G</p>
</td>
<td class="cellrowborder" valign="top" width="16.900000000000002%" headers="mcps1.2.6.1.4 "><p id="p12971140142310"><a name="p12971140142310"></a><a name="p12971140142310"></a>GCC 12.3.1</p>
</td>
<td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.6.1.5 "><p id="p102524252319"><a name="p102524252319"></a><a name="p102524252319"></a>&gt;=3.22.0</p>
</td>
</tr>
</tbody>
</table>

## 安装KRL

本节提供RPM包安装KRL方法。请参照本节内容对KRL进行安装和安装后验证。若操作过程中使用了RPM包管理工具支持但本文档中未说明的参数，可能会引入未定义行为，请谨慎操作。

1. 从GitCode仓获取对应的鲲鹏检索算子库软件安装包[BoostKit-boostsra-krl\_1.1.0.zip](https://gitcode.com/boostkit/boostsra/releases/download/v1.3.0/Boostkit-boostsra-krl_1.1.0.zip)，用户解压zip文件后可获取RPM安装包。

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >- KRL软件包结构如下所示。
    >
    > ```text
    > ├── boostsra-krl-xxxx.aarch64.rpm
    > └── 0001-faiss-1.8.0-add-krl.patch
    >    ```
    >
    > 其中，boostsra-krl-**_xxxx_**.aarch64.rpm包含KRL的头文件与动态库文件，0001-faiss-1.8.0-add-krl.patch为Faiss 1.8.0使能KRL所需的补丁文件，**_xxxx_** 表示KRL软件包的版本号。

2. 安装RPM包。

    ```bash
    rpm -ivh boostsra-krl-xxxx.aarch64.rpm
    ```

    安装结束后，自动追加环境变量LD\_LIBRARY\_PATH到“/etc/profile”中，即KRL的动态库文件所在目录“/usr/local/sra\_krl/lib”。

    上述命令中涉及的 **_xxxx_** 代表版本号。

3. 执行**source**命令或重新登录终端使环境变量生效。

    ```bash
    source /etc/profile
    ```

4. 查看环境变量LD\_LIBRARY\_PATH是否包含KRL的安装路径“/usr/local/sra\_krl/lib”。

    ```bash
    env | grep LD_LIBRARY_PATH
    ```

    如果变量包含安装路径，说明安装成功。

    安装成功后在安装路径（默认路径是“/usr/local/sra\_krl”）下生成相应文件，其中，“include”文件夹包含KRL的头文件，“lib”文件夹包含了KRL的动态库文件。

## 卸载KRL

如需要卸载KRL，请先停止调用KRL的业务流再进行卸载操作。若操作过程中使用了RPM包管理工具支持但本文档中未说明的参数，可能会引入未定义行为，请谨慎操作。

**RPM包卸载<a name="section175738555173"></a>**

1. 执行**rpm -e**命令卸载RPM安装包。

    ```bash
    rpm -e boostsra-krl
    ```

2. 确认安装目录“/usr/local/sra\_krl”被删除。
3. 确认“/etc/profile”文件中无“/usr/local/sra\_krl”相关环境变量。

## Faiss使能KRL

Faiss可对接KRL增强HNSW、PQFS、IVFPQ、IVFPQFS、IVFFLAT算法性能。用户需获取开源Faiss 1.8.0版本代码，合入使能KRL补丁后编译，最后得到KRL性能增强后的动态库文件。

1. 从[GitHub仓](https://github.com/facebookresearch/faiss.git)下载开源Faiss源代码，标签为**v1.8.0**。保存在编译机器可访问的路径中，假设位于“/path/to/faiss-1.8.0”。

    ```bash
    git clone --branch v1.8.0 --single-branch https://github.com/facebookresearch/faiss.git
    ```

2. 安装Make、CMake、GCC 12。

    - openEuler 22.03 LTS SP3系统

      ```bash
      yum install make cmake gcc-toolset-12-gcc gcc-toolset-12-gcc-c++ gcc-toolset-12-libstdc++-static gcc-toolset-12-gcc-gfortran
      export PATH=/opt/openEuler/gcc-toolset-12/root/usr/bin/:$PATH
      export LD_LIBRARY_PATH=/opt/openEuler/gcc-toolset-12/root/usr/lib64/:$LD_LIBRARY_PATH
      ```

    - openEuler 24.03 LTS SP3系统

      ```bash
      yum install make cmake gcc g++
      ```

3. <a name="li84129301112"></a>Faiss依赖数学库，从[Github仓](https://github.com/OpenMathLib/OpenBLAS.git)下载开源OpenBLAS源代码，标签为**v0.3.29**。保存在编译机器可访问的路径中，假设位于“/path/to/OpenBLAS-0.3.29”。

    ```bash
    git clone --branch v0.3.29 --single-branch https://github.com/OpenMathLib/OpenBLAS.git
    ```

4. 编译源代码，生成libopenblas.so动态库文件。

    ```bash
    cd /path/to/OpenBLAS-0.3.29/OpenBLAS
    make
    make install
    ```

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >可通过**make install PREFIX=/path/to/openblas/install**设置“/path/to/openblas/install”以指定安装路径，默认安装路径为“/opt/OpenBLAS”。

5. 解压BoostKit-boostsra-krl\_1.1.0.zip后可获取到使能KRL所需补丁文件0001-faiss-1.8.0-add-krl.patch。安装补丁文件。

    ```bash
    cd /path/to/faiss-1.8.0/faiss
    patch -p1 < /path/to/krl/0001-faiss-1.8.0-add-krl.patch
    ```

6. 编译Faiss代码获取libfaiss.so。

    ```bash
    export KRL_PATH=/usr/local/sra_krl
    cd /path/to/faiss-1.8.0
    cmake -B build . \
      -DFAISS_ENABLE_GPU=OFF \
      -DBUILD_TESTING=OFF \
      -DBUILD_SHARED_LIBS=ON \
      -DCMAKE_BUILD_TYPE=Release \
      -DFAISS_OPT_LEVEL=generic \
      -DFAISS_ENABLE_PYTHON=OFF \
      -DMKL_LIBRARIES=/opt/OpenBLAS/lib/libopenblas.so
    make -C build -j faiss
    make -C build install
    ```

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >- **KRL_PATH**设置为“/usr/local/sra_krl”。
    >- 可通过在编译时添加编译选项 **-DCMAKE\_INSTALL\_PREFIX=/path/to/faiss/install**设置“/path/to/faiss/install”以指定安装路径，默认安装路径为“/usr/local”。
    >- 编译选项 **-DMKL\_LIBRARIES**需指定为步骤[3](#li84129301112)中OpenBLAS的安装路径。

## 性能测试

本章节提供的示例以使用sift-128-euclidean.hdf5数据集，Faiss（IVFPQ）算法，线程数32为例。

**获取数据集与测试程序<a name="section5300679419"></a>**

1. 获取[测试程序](https://atomgit.com/openeuler/sra_test.git)。分支为**v2.0.0**，假设程序运行的目录为“/path/to/sra\_test”，完整的目录结构应如下所示：

    ```text
    ├── configs                                                   // 存放对应算法和数据集配置文件
          └── ivfpq
                └── ivfpq_sift-128-euclidean.config 
    ├── include                                                   // 存放测试框架对应的头文件
          └── algo                                                // 各算法Index定义
          └── core                                                // 数据处理、测试结果处理等头文件
          └── framework                                           // 测试框架相关头文件
    ├── src                                                       // 存放测试框架对应的源文件
          └── algo                                                // 各算法适配层
          └── bench                                               // 统一测试文件
          └── core                                                // 数据处理、测试结果处理等文件
          └── registry                                            // 各算法工厂注册
    ├── Makefile                                                  // 编译脚本文件
    ├── test.sh                                                   // 测试脚本
    ├── test_muti-numas.sh                                        // 并行测试脚本
    ├── data                                                      // 存放数据集（需手动创建并存放数据集）
          └── sift-128-euclidean.hdf5
    ├── indexes
          └── ivfpq                                               // 存放构建好的索引（需手动创建）
                └── sift.faiss                                    // 构建好的索引，当运行可执行文件ivfpq_test且数据集配置文件中save_or_load参数设置为save时生成
    └── ivfpq_test                                                // 编译后生成的可执行文件
    ```

2. <a name="li1673311431218"></a>获取数据集，存放于“/path/to/sra\_test/data”。

    ```bash
    cd /path/to/sra_test
    mkdir -p data
    cd data
    wget http://ann-benchmarks.com/sift-128-euclidean.hdf5 --no-check-certificate
    ```

**性能测试<a name="section183012712414"></a>**

1. 安装相关依赖。

    ```bash
    yum install hdf5 hdf5-devel numactl numactl-devel
    ```

2. 编译可执行文件。根据命令行提示输入Faiss安装路径及其他所需依赖所在路径。在提示“Enter extra compile defines”时输入“-I/path/to/krl/out/include/ -L/path/to/krl/out/lib/ -lkrl”，其中“/path/to/krl/out”为KRL的安装路径。

    ```bash
    cd /path/to/sra_test
    make ivfpq_test
    ```

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >测试时不同的算法需要选择不同的编译指令：
    >- HNSW算法：**make hnsw\_test**
    >- PQFS算法：**make pqfs\_test**
    >- IVFPQ算法：**make ivfpq\_test**
    >- IVFPQFS算法：**make ivfpqfs\_test**
    >- IVFFLAT算法：**make ivfflat\_test**

3. 若是第一次执行，确保ivfpq\_sift-128-euclidean.config文件中的“save\_or\_load”为“save”；后续执行时可改为“load”，使用构建好的图索引或检索器查询。
4. 运行可执行文件。将OpenBLAS、Faiss与KRL动态库路径添加至环境变量。

    ```bash
    numactl -C 0-31 -m 0 ./ivfpq_test ivfpq sift-128-euclidean
    ```

   优化前运行结果如[**图 1** 优化前运行结果](#优化前运行结果)所示。

   **图 1** 优化前运行结果<a name="fig9931619182"></a><a id="优化前运行结果"></a>

   ![](./figures/quick_start-origin运行结果.jpg "优化前运行结果")

   优化后结果如[**图 2** 优化后运行结果](#优化后运行结果)所示。

   **图 2** 优化后运行结果<a name="fig9931619183"></a><a id="优化后运行结果"></a>

   ![](./figures/quick_start-运行结果.jpg "优化后运行结果")
