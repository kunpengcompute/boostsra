# 安装指南

## 已验证环境

为保证您可以顺利安全地使用KScaNN，请确保所使用的环境信息在已验证环境范围内。

**表 1** KScaNN已验证环境<a id="KScaNN已验证环境"></a>

<table><thead align="left"><tr>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.6.1.1"><p>操作系统</p></th>
<th class="cellrowborder" valign="top" width="18%" id="mcps1.2.6.1.2"><p>CPU类型</p></th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.6.1.3"><p>内存</p></th>
<th class="cellrowborder" valign="top" width="15%" id="mcps1.2.6.1.4"><p>编译器</p></th>
<th class="cellrowborder" valign="top" width="35%" id="mcps1.2.6.1.5"><p>其他</p></th>
</tr></thead>
<tbody>
<tr>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p>openEuler 22.03 LTS SP3</p></td>
<td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.6.1.2 "><p>鲲鹏920 7282C处理器</p></td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.6.1.3 "><p>16 * 32GB</p></td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.6.1.4 "><p>GCC 12.3.1</p></td>
<td class="cellrowborder" valign="top" width="35%" headers="mcps1.2.6.1.5 "><ul><li>CMake>=3.22.0</li><li>GLIBCXX>=3.4.29</li><li>Python 3.9.x</li></ul></td>
</tr>
<tr>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p>openEuler 22.03 LTS SP3</p></td>
<td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.6.1.2 "><p>鲲鹏920 7282C处理器</p></td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.6.1.3 "><p>16 * 32GB</p></td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.6.1.4 "><p>GCC 10.3.1</p></td>
<td class="cellrowborder" valign="top" width="35%" headers="mcps1.2.6.1.5 "><ul><li>CMake>=3.22.0</li><li>GLIBCXX>=3.4.28</li><li>Python 3.9.x</li></ul></td>
</tr>
<tr>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p>openEuler 24.03 LTS SP3</p></td>
<td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.6.1.2 "><p>鲲鹏950 7592C处理器</p></td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.6.1.3 "><p>24 * 64GB</p></td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.6.1.4 "><p>GCC 12.3.1</p></td>
<td class="cellrowborder" valign="top" width="35%" headers="mcps1.2.6.1.5 "><ul><li>CMake>=3.22.0</li><li>GLIBCXX>=3.4.29</li><li>Python 3.9.x</li></ul></td>
</tr>
</tbody></table>

## 安装KScaNN

### RPM安装

本节提供RPM包安装KRL方法。请参照本节内容对KRL进行安装和安装后验证。若操作过程中使用了RPM包管理工具支持但本文档中未说明的参数，可能会引入未定义行为，请谨慎操作。

1. 从GitCode获取KScaNN软件包[BoostKit-boostsra-kscann\_2.2.0.zip](https://gitcode.com/boostkit/boostsra/releases/download/v1.1.0/BoostKit-boostsra-kscann_2.2.0.zip)，解压后得到二进制RPM包。

    软件包构成如下所示。

    ```text
    └── boostsra-kscann-xxxx.aarch64.rpm
    ```

    其中，boostkit-sra\_kscann-**_xxxx_**.aarch64.rpm包含KScaNN的头文件、动态库文件与静态库文件，**_xxxx_** 表示KScaNN软件包的版本号。

2. 安装RPM包。

    ```bash
    rpm -ivh boostsra-kscann-xxxx.aarch64.rpm
    ```

    安装结束后，自动追加环境变量LD\_LIBRARY\_PATH到“/etc/profile“中，即KScaNN的动态库文件与静态库文件所在目录“/usr/local/sra\_kscann/lib/“与“/usr/local/sra\_kscann/lib/sve“。

    上述命令中涉及的 **_xxxx_** 代表版本号。

## 生成完整的ScaNN

KScaNN依赖基于鲲鹏优化的开源ScaNN以提供完整的功能。因此安装KScaNN后需自行获取基于鲲鹏优化的开源ScaNN代码，以编译生成完整的ScaNN的Python安装包及动态库文件。

**操作步骤<a name="section106931822175410"></a>**

1. 从[GitCode](https://atomgit.com/openeuler/sra_scann_adapter.git)仓下载基于鲲鹏优化的开源ScaNN源代码，标签为**v2.2.1**。保存在编译机器可访问的路径中，假设位于“/path/to/kscann-build“。

    ```bash
    mkdir /path/to/kscann-build && cd /path/to/kscann-build
    git clone --branch v2.2.1 --single-branch https://atomgit.com/openeuler/sra_scann_adapter.git
    ```

2. 获取google-research的开源代码，其中包含ScaNN v1.2.10代码。假设代码存放于“/path/to/kscann-build”。

    ```bash
    cd /path/to/kscann-build
    git clone https://github.com/google-research/google-research.git
    cd google-research
    git reset --hard 03c4c851a28dffe0244c65089e68d6cbf73c730b
    cp -r scann/ ../sra_scann_adapter
    ```

3. 合入ScaNN v1.2.10使能KScaNN所需的补丁文件0001-boostsra-kscann-adapter.patch。

    ```bash
    cd /path/to/kscann-build/sra_scann_adapter
    patch -p1 < 0001-boostsra-kscann-adapter.patch
    ```

4. ScaNN依赖AVX2KI库，因此需要通过以下步骤安装AVX2KI的RPM包。
    1. 安装AVX2KI之前请先从[鲲鹏社区](https://www.hikunpeng.com/developer/boostkit/library/detail?subtab=AVX2KI)获取软件包，再进行软件包校验，确保与网站上的原始软件包一致，用户解压zip文件后可获取RPM安装包。

        >![](public_sys-resources/icon-notice.gif) **须知：** 
        >使用软件包前请先阅读《[鲲鹏应用使能套件BoostKit用户许可协议 2.0](https://www.hikunpeng.com/zh/legal/developer/boostkit/software/protocol)》，如确认继续使用，则默认同意协议的条款和条件。

    2. <a name="li6766112117714"></a>从[华为企业业务网站](https://support.huawei.com/enterprise/zh/tool/pgp-verify-TL1000000054)获取校验工具和校验方法。
    3. 请参见[4.2](#li6766112117714)中下载的《OpenPGP签名验证指南》进行软件包完整性检查。
    4. 安装AVX2KI的RPM包。

        ```bash
        rpm -ivh boostkit-ksl-xxxx.aarch64.rpm
        ```

        安装结束后，自动追加环境变量LD\_LIBRARY\_PATH到“/etc/profile“中，即AVX2KI的动态库文件所在目录“/usr/local/ksl/lib“。

        上述命令中的 **xxxx** 代表版本号。

    5. 执行**source**命令或重新登录终端使AVX2KI环境变量生效。

        ```bash
        source /etc/profile
        ```

    6. 查看环境变量LD\_LIBRARY\_PATH是否包含AVX2KI的安装路径“/usr/local/ksl/lib“。

        ```bash
        env | grep LD_LIBRARY_PATH
        ```

        如果变量包含安装路径，说明安装成功。

        安装成功后在安装路径（默认路径是“/usr/local/ksl“）下生成相应文件，其中，“include“文件夹包含AVX2KI的头文件，“lib“文件夹包含了AVX2KI的动态库文件。

5. 安装OpenJDK 11。

    ```bash
    yum install java-11-openjdk java-11-openjdk-devel
    ```

    检查OpenJDK 11是否安装成功。

    ```bash
    java -version
    ```

    如果回显包含openjdk version "11._**x**_.**_x_**"，则表示安装成功。若OpenJDK版本低于此版本，则后续编译Bazel可能会发生错误，导致无法正常构建Bazel。

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >若执行上述命令发现版本不匹配，请按以下步骤配置环境变量。
    >
    >```bash
    >find / -name java
    >```
    >
    >找到安装目录后，配置环境变量，假设安装目录为“/usr/lib/jvm/java-11-openjdk-11.0.23.9-2.oe2203sp3.aarch64“。
    >
    >```bash
    >export JAVA_HOME=/usr/lib/jvm/java-11-openjdk-11.0.23.9-2.oe2203sp3.aarch64
    >export PATH=/usr/lib/jvm/java-11-openjdk-11.0.23.9-2.oe2203sp3.aarch64/bin:$PATH
    >```

6. 安装Bazel 5.4.0。
    1. 下载Bazel 5.4.0源码，假设路径为“/path/to/bazel“。

        ```bash
        wget https://github.com/bazelbuild/bazel/releases/download/5.4.0/bazel-5.4.0-dist.zip --no-check-certificate
        ```

    2. 执行以下命令解压并编译Bazel。

        ```bash
        unzip bazel-5.4.0-dist.zip -d bazel-5.4.0
        cd bazel-5.4.0
        env EXTRA_BAZEL_ARGS="--tool_java_runtime_version=local_jdk" bash ./compile.sh
        ```

    3. 构建成功后，生成的可执行文件bazel在“/path/to/bazel/bazel-5.4.0/output“路径中，将该路径配置在环境变量PATH中，以便后续编译ScaNN使用。

        ```bash
        export PATH=/path/to/bazel/bazel-5.4.0/output:$PATH
        ```

    4. 执行以下命令验证。

        ```bash
        bazel --version
        ```

        如果回显包含bazel 5.4.0- \(@non-git\)，则表示安装成功。

7. 安装GCC 12.3.1与GCC-C++ 12.3.1。
    1. 获取对应的GCC。

        ```bash
        wget https://mirrors.huaweicloud.com/kunpeng/archive/compiler/kunpeng_gcc/gcc-12.3.1-2025.06-aarch64-linux.tar.gz --no-check-certificate
        ```

    2. 请参见《GCC for openEuler 用户指南》的[安装GCC for openEuler](https://www.hikunpeng.com/document/detail/zh/kunpengdevps/compiler/ug-hgcc/kunpenghgcc_06_0004.html)章节完成安装。

        ```bash
        export CC=/opt/aarch64/compiler/gcc-12.3.1-2025.06-aarch64-linux/bin/gcc
        export CXX=/opt/aarch64/compiler/gcc-12.3.1-2025.06-aarch64-linux/bin/g++
        ```

8. 安装编译依赖。

    ```bash
    yum install python python3-devel python3-pip rsync libomp libuuid-devel
    ```

    确保KScaNN位于“/usr/local/sra\_recall/lib/kscann“，AVX2KI位于“/usr/local/ksl/lib“。

9. 开始编译。

    1. 指定KScaNN的安装目录。安装目录为"/usr/local/sra_kscann"。配置合适的pip源。

        ```bash
        export KSCANN_PATH=/usr/local/sra_kscann
        ```

    2. 运行以下指令以进行必要的依赖安装。

        ```bash
        cd /path/to/scann
        sh project.sh --prepare
        ```

    3. 运行以下指令以开始ScaNN的Python安装包的构建。

        ```bash
        sh project.sh --build_whl
        ```

    4. 构建完的Python安装包scann-1.2.10-cp39-cp39-linux\_aarch64.whl位于“/path/to/kscann-build/scann“下。
    5. 运行以下指令以开始ScaNN的动态库文件的构建。

        ```bash
        sh project.sh --build_scann_cc_sve
        ```

        构建完的动态库文件libscann\_cc.so位于“/path/to/kscann-build/scann“下。

        >![](public_sys-resources/icon-note.gif) **说明：** 
        >project.sh中包含以下编译选项，可根据需求进行选择：
        >- --prepare：进行Python依赖安装。
        >- --build\_whl：构建完整的ScaNN的Python安装包。
        >- --build\_scann\_cc\_sve：构建SVE指令版本的完整的ScaNN的动态库文件。
        >- --build\_scann\_cc\_neon：构建NEON指令版本的完整的ScaNN的动态库文件。
        >- --build\_scann\_cc\_sve\_milvus：构建适用于Milvus场景的SVE指令版本的完整的ScaNN的动态库文件。
        >- --build\_scann\_cc\_neon\_milvus：构建适用于Milvus场景的构建NEON指令版本的完整的ScaNN的动态库文件。

        >若环境搭建过程中提示“unable to find valid certification path to requested target”，请参见《ScaNN 移植指南》中的[编译ScaNN过程中提示找不到证书路径的解决办法](https://www.hikunpeng.com/document/detail/zh/SRA/ecosystemEnable/ScaNN/kunpengscann_02_0014.html)章节解决。

10. 安装whl。

    ```bash
    pip install scann-1.2.10-cp39-cp39-linux_aarch64.whl
    ```

11. 执行**pip** **show**命令确认scann==1.2.10已安装。

    ```bash
    pip show scann
    ```

    如果输出包含Name: scann Version: 1.2.10，则已安装成功。

## 卸载KScaNN

**RPM包卸载<a name="section118069490504"></a>**

卸载KScaNN将会影响您正在执行的业务流，建议先停止正在执行的业务流再进行卸载操作。若操作过程中使用了RPM包管理工具支持但本文档中未说明的参数，可能会引入未定义行为，请谨慎操作。

1. 执行**rpm -e**命令卸载RPM安装包。

    ```bash
    rpm -e boostsra-kscann
    ```

2. 确认安装目录“/usr/local/sra\_kscann“被删除。
3. 确认“/etc/profile“文件中无“/usr/local/sra\_kscann“相关环境变量。

**whl卸载<a name="section58079490509"></a>**

1. 执行**pip uninstall**命令卸载whl文件。

    ```bash
    pip uninstall scann
    ```

2. 执行**pip** **show**命令确认scann==1.2.10已卸载。

    ```bash
    pip show scann
    ```

    如果输出包含WARNING: Package\(s\) not found: scann，则已卸载成功。
