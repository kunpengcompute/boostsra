# Installation Guide

## Verified Environments

To use KDNN smoothly and securely, ensure that your environment is one of the verified environments.

**Table 1** Verified environments for KDNN<a id="verified-environments-for-kdnn"></a>

<a name="zh-cn_topic_0000001831167081_table2919mcpsimp"></a>
<table><thead align="left"><tr id="zh-cn_topic_0000001831167081_row2926mcpsimp"><th class="cellrowborder" valign="top" width="12.15%" id="mcps1.2.7.1.1"><p id="p672213451215"><a name="p672213451215"></a><a name="p672213451215"></a>Component</p>
</th>
<th class="cellrowborder" valign="top" width="19.97%" id="mcps1.2.7.1.2"><p id="zh-cn_topic_0000001831167081_p2928mcpsimp"><a name="zh-cn_topic_0000001831167081_p2928mcpsimp"></a><a name="zh-cn_topic_0000001831167081_p2928mcpsimp"></a>OS</p>
</th>
<th class="cellrowborder" valign="top" width="22.32%" id="mcps1.2.7.1.3"><p id="zh-cn_topic_0000001831167081_p2930mcpsimp"><a name="zh-cn_topic_0000001831167081_p2930mcpsimp"></a><a name="zh-cn_topic_0000001831167081_p2930mcpsimp"></a>CPU</p>
</th>
<th class="cellrowborder" valign="top" width="18.94%" id="mcps1.2.7.1.4"><p id="zh-cn_topic_0000001831167081_p94235351693"><a name="zh-cn_topic_0000001831167081_p94235351693"></a><a name="zh-cn_topic_0000001831167081_p94235351693"></a>Compiler</p>
</th>
<th class="cellrowborder" valign="top" width="11.07%" id="mcps1.2.7.1.5"><p id="p157041029488"><a name="p157041029488"></a><a name="p157041029488"></a>Build Tool</p>
</th>
<th class="cellrowborder" valign="top" width="15.55%" id="mcps1.2.7.1.6"><p id="p10171835144516"><a name="p10171835144516"></a><a name="p10171835144516"></a>Python Interpreter</p>
</th>
</tr>
</thead>
<tbody><tr id="row056323751218"><td class="cellrowborder" valign="top" width="12.15%" headers="mcps1.2.7.1.1 "><p id="p7180194317123"><a name="p7180194317123"></a><a name="p7180194317123"></a>KDNN</p>
</td>
<td class="cellrowborder" valign="top" width="19.97%" headers="mcps1.2.7.1.2 "><p id="p16180743171218"><a name="p16180743171218"></a><a name="p16180743171218"></a>openEuler 22.03 LTS SP3</p>
</td>
<td class="cellrowborder" valign="top" width="22.32%" headers="mcps1.2.7.1.3 "><p id="p818014317128"><a name="p818014317128"></a><a name="p818014317128"></a>New Kunpeng 920 processor model</p>
</td>
<td class="cellrowborder" valign="top" width="18.94%" headers="mcps1.2.7.1.4 "><p id="p718017432120"><a name="p718017432120"></a><a name="p718017432120"></a>GCC 10.3.1</p>
</td>
<td class="cellrowborder" valign="top" width="11.07%" headers="mcps1.2.7.1.5 "><p id="p191801843141211"><a name="p191801843141211"></a><a name="p191801843141211"></a>CMake 3.22.0</p>
</td>
<td class="cellrowborder" valign="top" width="15.55%" headers="mcps1.2.7.1.6 "><p id="p1518012435123"><a name="p1518012435123"></a><a name="p1518012435123"></a>Python 3.9.21</p>
</td>
</tr>
<tr id="row15391159141317"><td class="cellrowborder" valign="top" width="12.15%" headers="mcps1.2.7.1.1 "><p id="p1782141813236"><a name="p1782141813236"></a><a name="p1782141813236"></a>KDNN</p>
</td>
<td class="cellrowborder" valign="top" width="19.97%" headers="mcps1.2.7.1.2 "><p id="p126842487387"><a name="p126842487387"></a><a name="p126842487387"></a>openEuler 22.03 LTS SP4</p>
<p id="p618613441416"><a name="p618613441416"></a><a name="p618613441416"></a>The kernel version is later than 5.10.0-228.0.0.127.</p>
</td>
<td class="cellrowborder" valign="top" width="22.32%" headers="mcps1.2.7.1.3 "><p id="p161878491412"><a name="p161878491412"></a><a name="p161878491412"></a>New Kunpeng 920 processor model</p>
</td>
<td class="cellrowborder" valign="top" width="18.94%" headers="mcps1.2.7.1.4 "><p id="p6187843140"><a name="p6187843140"></a><a name="p6187843140"></a>GCC 12.3.1/BiSheng 4.2.0</p>
</td>
<td class="cellrowborder" valign="top" width="11.07%" headers="mcps1.2.7.1.5 "><p id="p191879461419"><a name="p191879461419"></a><a name="p191879461419"></a>CMake 3.22.0</p>
</td>
<td class="cellrowborder" valign="top" width="15.55%" headers="mcps1.2.7.1.6 "><p id="p7187124181413"><a name="p7187124181413"></a><a name="p7187124181413"></a>Python 3.9.21</p>
</td>
</tr>
<tr id="row122015101207"><td class="cellrowborder" valign="top" width="12.15%" headers="mcps1.2.7.1.1 "><p id="p57227410129"><a name="p57227410129"></a><a name="p57227410129"></a>KDNN_EXT</p>
</td>
<td class="cellrowborder" valign="top" width="19.97%" headers="mcps1.2.7.1.2 "><p id="zh-cn_topic_0000001831167081_p49592815115"><a name="zh-cn_topic_0000001831167081_p49592815115"></a><a name="zh-cn_topic_0000001831167081_p49592815115"></a>openEuler 22.03 LTS SP3</p>
</td>
<td class="cellrowborder" valign="top" width="22.32%" headers="mcps1.2.7.1.3 "><p id="zh-cn_topic_0000001831167081_p1871451912230"><a name="zh-cn_topic_0000001831167081_p1871451912230"></a><a name="zh-cn_topic_0000001831167081_p1871451912230"></a>Kunpeng 920 processors</p>
</td>
<td class="cellrowborder" valign="top" width="18.94%" headers="mcps1.2.7.1.4 "><p id="zh-cn_topic_0000001831167081_p17184611237"><a name="zh-cn_topic_0000001831167081_p17184611237"></a><a name="zh-cn_topic_0000001831167081_p17184611237"></a>GCC 10.3.1</p>
</td>
<td class="cellrowborder" valign="top" width="11.07%" headers="mcps1.2.7.1.5 "><p id="p87043212484"><a name="p87043212484"></a><a name="p87043212484"></a>CMake 3.22.0</p>
</td>
<td class="cellrowborder" valign="top" width="15.55%" headers="mcps1.2.7.1.6 "><p id="p61863514518"><a name="p61863514518"></a><a name="p61863514518"></a>Python 3.9.20</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **NOTE**
>
>- KDNN supports the Kunpeng 920 processors and new Kunpeng 920 processor model. Using other processors may cause undefined results.
>- KDNN is a low-level primitive library whose computational workflow manages memory read/write and allocation operations. It does not provide or distribute an operating system (OS). Users are responsible for OS installation and its subsequent security. Users must harden the OS based on their specific application scenarios, which includes disabling or removing unnecessary applications.
>- To prevent buffer overflow attacks, you are advised to use the address space layout randomization (ASLR) technology to randomize the layout of linear areas such as the heap, stack, and shared library mapping to make it more difficult for attackers to predict target addresses and locate code. This technology can be applied to heaps, stacks, and memory mapping areas (mmap base addresses, shared libraries, and vDSO pages). Enabling method: **echo 2 > /proc/sys/kernel/randomize_va_space**

## Configuring a Network Proxy<a name="ZH-CN_TOPIC_0000002518232616"></a>

If you cannot directly access the Internet, configure a network proxy temporarily or permanently. A permanent network proxy may cause password leakage because all users in the environment can obtain the password. Therefore, you are advised to configure a temporary network proxy. You can also select the proxy mode that better suits your requirements.

**Method 1: Configuring a Temporary Network Proxy<a name="section1694205085318"></a>**

1. Set the environment variable.

    Set the user name, password, proxy IP address, and proxy port based on your requirements.

    ```bash
    export http_proxy="http://_Username:Password_@_Proxy IP address:proxy port_"
    export https_proxy=$http_proxy
    ```

2. Confirm that the Internet connection is normal.

    Run the <code>curl</code> command to access any website. If the website information is displayed, the proxy is successfully configured and the Internet is connected.

**Method 2: Configuring a Permanent Network Proxy<a name="section49515065317"></a>**

1. Modify the <code>profile</code> file.
    1. Open the <code>/etc/profile</code> file.

        ```bash
        vi /etc/profile
        ```

    2. Press <code>i</code> to enter the insert mode and add the following content to the <code>/etc/profile</code> file.

        Set the user name, password, proxy IP address, and proxy port based on your requirements.

        ```bash
        export http_proxy="http://_Username:Password_@_Proxy IP address:proxy port_"
        export https_proxy=$http_proxy 
        export no_proxy=127.0.0.1,localhost,local,.local
        ```

    3. Press <code>Esc</code>, type <code>:wq!</code>, and press <code>Enter</code> to save the file and exit.
    4. Make the proxy take effect.

        ```bash
        source /etc/profile
        ```

2. Confirm that the Internet connection is normal.

    Run the <code>curl</code> command to access any website. If the website information is displayed, the proxy is successfully configured and the Internet is connected.

## Installing Environment Dependencies

Use Yum repositories to install the base software on which the system depends, including GCC/G++.

1. Install system dependencies.

    ```bash
    yum install make git gcc-c++ cmake
    ```

2. Install NumPy (required when the KDNN\_EXT component is used).

    ```bash
    pip install numpy==1.24.2
    ```

3. Install one of the following compilers based on your target environment.

    - GCC 10.3.1 (for openEuler 22.03 LTS SP3):

        ```bash
        yum install gcc gcc-c++
        gcc --version
        g++ --version
        ```

    - GCC 12.3.1 (for openEuler 22.03 LTS SP4):

        ```bash
        yum install gcc-toolset-12-gcc gcc-toolset-12-gcc-c++ gcc-toolset-12-libstdc++-static gcc-toolset-12-gcc-gfortran
        export PATH=/opt/openEuler/gcc-toolset-12/root/usr/bin/:$PATH
        export LD_LIBRARY_PATH=/opt/openEuler/gcc-toolset-12/root/usr/lib64/:$LD_LIBRARY_PATH
        gcc --version
        g++ --version
        ```

    - BiSheng Compiler 4.2.0:

        Obtain the `BiShengCompiler-4.2.0-aarch64-linux.tar.gz` installation package from the [BiSheng Compiler release page](https://mirrors.huaweicloud.com/kunpeng/archive/compiler/bisheng_compiler), and replace `<bisheng-package>` with the actual file name.

        ```bash
        tar -xzf <bisheng-package>.tar.gz -C /opt
        export PATH=/opt/<bisheng-directory>/bin:$PATH
        export LD_LIBRARY_PATH=/opt/<bisheng-directory>/lib:$LD_LIBRARY_PATH
        export CC=/opt/<bisheng-directory>/bin/clang
        export CXX=/opt/<bisheng-directory>/bin/clang++
        clang --version
        ```

## Obtaining the Software Package

### Downloading the Software Package

Obtain the corresponding software digital certificate and software installation package from the [AtomGit release page](https://gitcode.com/boostkit/boostsra/releases). Decompress the ZIP file to obtain the RPM installation package.

**Table 1** KDNN software package list<a id="kdnn-software-package-list"></a>

<a name="zh-cn_topic_0000001784526702_table677mcpsimp"></a>
<table><thead align="left"><tr id="zh-cn_topic_0000001784526702_row684mcpsimp"><th class="cellrowborder" valign="top" width="28.96%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0000001784526702_p686mcpsimp"><a name="zh-cn_topic_0000001784526702_p686mcpsimp"></a><a name="zh-cn_topic_0000001784526702_p686mcpsimp"></a>Name</p>
</th>
<th class="cellrowborder" valign="top" width="32.04%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0000001784526702_p688mcpsimp"><a name="zh-cn_topic_0000001784526702_p688mcpsimp"></a><a name="zh-cn_topic_0000001784526702_p688mcpsimp"></a>Package Name</p>
</th>
<th class="cellrowborder" valign="top" width="39%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0000001784526702_p690mcpsimp"><a name="zh-cn_topic_0000001784526702_p690mcpsimp"></a><a name="zh-cn_topic_0000001784526702_p690mcpsimp"></a>Release Version</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0000001784526702_row692mcpsimp"><td class="cellrowborder" valign="top" width="28.96%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0000001784526702_p694mcpsimp"><a name="zh-cn_topic_0000001784526702_p694mcpsimp"></a><a name="zh-cn_topic_0000001784526702_p694mcpsimp"></a>KDNN software package (GCC)</p>
</td>
<td class="cellrowborder" valign="top" width="32.04%" headers="mcps1.2.4.1.2">
<p id="zh-cn_topic_0000001784526702_p696mcpsimp">
    <a name="zh-cn_topic_0000001784526702_p696mcpsimp"></a>
    BoostKit-boostcore-kdnn_3.2.0.zip
</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 ">
<p id="p125955276200"><a name="p125955276200"></a><a name="p125955276200"></a>v1.4.0</p>
</td>
</tr>
<tr id="row1487285541019"><td class="cellrowborder" valign="top" width="28.96%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0000001784526702_p708mcpsimp"><a name="zh-cn_topic_0000001784526702_p708mcpsimp"></a><a name="zh-cn_topic_0000001784526702_p708mcpsimp"></a>KDNN software package (BiSheng Compiler)</p>
</td>
<td class="cellrowborder" valign="top" width="32.04%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0000001784526702_p711mcpsimp"><a name="zh-cn_topic_0000001784526702_p711mcpsimp"></a><a name="zh-cn_topic_0000001784526702_p711mcpsimp"></a>BoostKit-boostcore-kdnn.3.0.0_bisheng.zip<sup id="sup195471318183"><a name="sup195471318183"></a><a name="sup195471318183"></a>a</sup></p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 ">
<p id="p141301730112014"><a name="p141301730112014"></a><a name="p141301730112014"></a>v1.1.0</p>
</td>
</tr>
</tbody>
</table>

### Verifying Package Integrity

#### Overview

To check whether the package was damaged during transmission or storage because of network or device issues, verify its integrity after obtaining it. Only a package that passes the verification can be deployed.<br>
Compare the checksum recorded in the checksum file with the checksum manually calculated for the software package. If the values are identical, the file is complete. Otherwise, the file integrity has been compromised and the package must be obtained again.

#### Prerequisites

Prepare the following files before verifying package integrity:

- Software package: `BoostKit-boostcore-kdnn_xxx.zip`.
- Checksum file: A `.sha256` file with the same name.

#### Procedure

Perform the following steps to verify file integrity:

1. Calculate the SHA-256 checksum of the package. On Linux, run:

   ```bash
   sha256sum BoostKit-boostcore-kdnn_xxx.zip
   ```

   On Windows, run:

   ```cmd
   certutil -hashfile BoostKit-boostcore-kdnn_xxx.zip SHA256
   ```

   The checksum is displayed after the command execution finishes.
2. Compare the checksum calculated in step 1 with the SHA-256 value in the checksum file.<br>
   If the values match, the file is complete. If they do not match, the file integrity has been compromised and the package must be obtained again.

## Using KDNN

### Installing KDNN

This section describes how to install KDNN using an RPM package and verify the installation. If you use parameters supported by the RPM package management tool but not described in this document, undefined behavior may be introduced. Exercise caution when performing this operation.

**Installation Procedure<a name="section39201312169"></a>**

1. Obtain the KDNN package by following [Downloading the Software Package](#downloading-the-software-package), and decompress it to obtain the binary RPM package.
2. Install KDNN.

    ```bash
    rpm -ivh boostcore-kdnn-xxxx.aarch64.rpm
    ```

    After the installation is complete, the directories of the header file, static library, and dynamic library of the KAIL are <code>/usr/local/kdnn/include</code>, <code>/usr/local/kdnn/lib/threadpool</code>, and <code>/usr/local/kdnn/lib/omp</code>, respectively.

**Verification After Installation<a name="section193111321616"></a>**

**Verifying KDNN**

1. Run the <code>source</code> command or log in to the terminal again for the environment variable to take effect.

    ```bash
    source /etc/profile
    ```

2. Check whether the environment variable <code>LD\_LIBRARY\_PATH</code> contains the installation path <code>/usr/local/kdnn/lib/omp</code> of the KDNN dynamic library.

    ```bash
    env | grep LD_LIBRARY_PATH
    ```

    If the variable contains the installation path, the installation is successful.

    After the installation, the corresponding files are generated in the installation path (the default path is <code>/usr/local/kdnn</code>). The <code>include</code> folder contains the header file of the sublibrary, and the <code>lib</code> folder contains the static and dynamic library files of KDNN.

**Verifying KDNN_EXT**

1. Set the <code>PYTHONPATH</code> environment variable.
    - To use the single-threaded version:

        ```bash
        export PYTHONPATH=/usr/local/kdnn/lib/extension/python39/single/:$PYTHONPATH
        ```

    - To use the multi-threaded version:

        ```bash
        export PYTHONPATH=/usr/local/kdnn/lib/extension/python39/omp/:$PYTHONPATH
        ```

2. Go to the Python interactive CLI and import the <code>libkdnn_ext</code> operator package.

    ```bash
    python
    >>> import libkdnn_ext
    ```

    Or

    ```bash
    >>> from libkdnn_ext import random_choice, softmax, get_version
    ```

    If no error information is displayed in the command output, KDNN_EXT has been installed successfully.

## Uninstalling KDNN

If KDNN is no longer needed, uninstall it. Using parameters supported by the RPM package manager but not documented in this guide may result in undefined behavior. Proceed with caution.

1. Run the <code>rpm -e</code> command to uninstall the RPM package.

    ```bash
    rpm -e boostcore-kdnn
    ```

2. Confirm that the installation directory <code>/usr/local/kdnn</code> is deleted.

## Change History

| Version | Date | Description |
| ------- | ---- | -------- |
| 01 | 2026-09-30 | This is the first official release. |
