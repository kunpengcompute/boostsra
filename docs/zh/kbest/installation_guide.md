# 安装指南

本文档介绍KBest安装方法，提供RPM包和whl文件的安装与卸载步骤及安装后验证方法，适用于需要安装和配置KBest软件的用户。

## 已验证环境

为保证您可以顺利安全地使用KBest，请确保所使用的环境信息在已验证环境范围内。

**表 1** KBest已验证环境<a id="KBest已验证环境"></a>

<a name="table4692134313211"></a>

| 操作系统 | CPU类型 | 内存 | 编译器 | 其他 |
| --- | --- | --- | --- | --- |
| openEuler 22.03 LTS SP3 | 鲲鹏920 7282C处理器 | 16*32GB | GCC 12.3.1 | CMake>=3.22.0<br>GLIBCXX>=3.4.29<br>Python 3.9.x |
| openEuler 22.03 LTS SP3 | 鲲鹏920 7282C处理器 | 16*32GB | GCC 10.3.1 | CMake>=3.22.0<br>GLIBCXX>=3.4.28<br>Python 3.9.x |
| openEuler 24.03 LTS SP1 | 鲲鹏920 7282C处理器 | 16*32GB | GCC 12.3.1 | CMake>=3.22.0<br>GLIBCXX>=3.4.29<br>Python 3.9.x |
| openEuler 24.03 LTS SP3 | 鲲鹏950 7592C处理器 | 24*64GB | GCC 12.3.1 | CMake>=3.22.0<br>GLIBCXX>=3.4.29<br>Python 3.9.x |

## 安装KBest

本节提供RPM包安装KBest方法。请参照本节内容对KBest进行安装和验证。若操作过程中使用了RPM包管理工具支持，但本文档中未说明的参数，可能会引入未定义行为，请谨慎操作。

**安装步骤<a name="section349212333315"></a>**

1. 从GitCode仓获取KBest软件包[BoostKit-boostsra-kbest\_2.2.0.zip](https://gitcode.com/boostkit/boostsra/releases/download/v1.1.0/BoostKit-boostsra-kbest_2.2.0.zip)，解压后得到二进制RPM包和whl文件。

    软件包结构如下所示。

    ```text
    ├── boostsra-kbest-xxxx.aarch64.rpm
    └── boostsra-kbest-xxxx-cp39-cp39-linux_aarch64.whl
    ```

    其中，boostsra-kbest-**_xxxx_**.aarch64.rpm包含KBest的头文件、动态库文件，boostsra-kbest-**_xxxx_**-cp39-cp39-linux\_aarch64.whl为KBest Python框架测试所需安装的文件，**_xxxx_** 表示KBest软件包的版本号。

2. 安装RPM包。

    ```bash
    rpm -ivh boostsra-kbest-xxxx.aarch64.rpm
    ```

    安装结束后，自动追加环境变量LD\_LIBRARY\_PATH到“/etc/profile”中，即KBest的动态库文件所在目录“/usr/local/sra\_kbest/lib”。

    上述命令中涉及的 **_xxxx_** 代表版本号。

3. 安装whl文件。

    ```bash
    pip install boostsra-kbest-xxxx-cp39-cp39-linux_aarch64.whl
    ```

    上述命令中涉及的 **_xxxx_** 代表版本号。

**安装后验证<a name="section10493153333112"></a>**

1. 执行**source**命令或重新登录终端使环境变量生效。

    ```bash
    source /etc/profile
    ```

2. 查看环境变量LD\_LIBRARY\_PATH是否包含KBest的安装路径“/usr/local/sra\_kbest/lib”。

    ```bash
    env | grep LD_LIBRARY_PATH
    ```

    如果变量包含安装路径，说明安装成功。

    安装成功后在安装路径（默认路径是“/usr/local/sra\_kbest”）下生成相应文件，其中，“include”文件夹包含KBest的头文件，“lib”文件夹包含了KBest的动态库文件。

3. 执行**pip** **show**命令确认kbest== **_xxxx_** 已安装。

    ```bash
    pip show kbest
    ```

    如果输出包含Name: kbest Version:  **_xxxx_**，则已安装成功。

## （可选）卸载KBest

**RPM包卸载<a name="section154931433123117"></a>**

卸载KBest将会影响您正在执行的业务流，建议先停止正在执行的业务流再进行卸载操作。若操作过程中使用了RPM包管理工具支持但本文档中未说明的参数，可能会引入未定义行为，请谨慎操作。

1. 执行**rpm -e**命令卸载RPM安装包。

    ```bash
    rpm -e boostsra-kbest
    ```

2. 确认安装目录“/usr/local/sra\_kbest”被删除。
3. 确认“/etc/profile”文件中无“/usr/local/sra\_kbest”相关环境变量。

**whl卸载<a name="section7493143393110"></a>**

1. 执行**pip uninstall**命令卸载whl文件。

    ```bash
    pip uninstall kbest
    ```

2. 执行**pip** **show**命令确认kbest== **_xxxx_** 已卸载。

    ```bash
    pip show kbest
    ```

    如果输出包含WARNING: Package\(s\) not found: kbest，则已卸载成功。

## 修订记录

|文档版本|发布日期|修改说明|
|--|--|--|
|01|2025-12-30|第一次正式发布。|
