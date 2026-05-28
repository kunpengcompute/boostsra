# Installation Guide

## Verified Environments

To use KScaNN smoothly and securely, ensure that your environment is one of the verified environments.

Table 1 Verified environments for KScaNN<a id="verified-environments-for-kscaNN"></a>

<table><thead align="left"><tr>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.6.1.1"><p>OS</p></th>
<th class="cellrowborder" valign="top" width="18%" id="mcps1.2.6.1.2"><p>CPU</p></th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.6.1.3"><p>Memory</p></th>
<th class="cellrowborder" valign="top" width="15%" id="mcps1.2.6.1.4"><p>Compiler</p></th>
<th class="cellrowborder" valign="top" width="35%" id="mcps1.2.6.1.5"><p>Remarks</p></th>
</tr></thead>
<tbody>
<tr>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p>openEuler 22.03 LTS SP3</p></td>
<td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.6.1.2 "><p> New Kunpeng 920 processor model</p></td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.6.1.3 "><p>16 × 32 GB</p></td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.6.1.4 "><p>GCC 12.3.1</p></td>
<td class="cellrowborder" valign="top" width="35%" headers="mcps1.2.6.1.5 "><ul><li>CMake>=3.22.0</li><li>GLIBCXX>=3.4.29</li><li>Python 3.9.x</li></ul></td>
</tr>
<tr>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p>openEuler 22.03 LTS SP3</p></td>
<td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.6.1.2 "><p> New Kunpeng 920 processor model</p></td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.6.1.3 "><p>16 × 32 GB</p></td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.6.1.4 "><p>GCC 10.3.1</p></td>
<td class="cellrowborder" valign="top" width="35%" headers="mcps1.2.6.1.5 "><ul><li>CMake>=3.22.0</li><li>GLIBCXX>=3.4.28</li><li>Python 3.9.x</li></ul></td>
</tr>
<tr>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p>openEuler 24.03 LTS SP3</p></td>
<td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.6.1.2 "><p> Kunpeng 950 processor</p></td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.6.1.3 "><p>24 × 64 GB</p></td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.6.1.4 "><p>GCC 12.3.1</p></td>
<td class="cellrowborder" valign="top" width="35%" headers="mcps1.2.6.1.5 "><ul><li>CMake>=3.22.0</li><li>GLIBCXX>=3.4.29</li><li>Python 3.9.x</li></ul></td>
</tr>
</tbody></table>

## Installing KScaNN

### Installation Using an RPM Package

This section describes how to install KScaNN using the RPM package and verify the package. Using parameters supported by the RPM package manager but not documented in this guide may result in undefined behavior. Proceed with caution.

1. Obtain the KScaNN software package [BoostKit-boostsra-kscann_2.2.0.zip](https://gitcode.com/boostkit/boostsra/releases/download/v1.1.0/BoostKit-boostsra-kscann_2.2.0.zip) from GitCode and decompress it to obtain the binary RPM package.

    The software package structure is as follows.

    ```text
    └── boostsra-kscann-xxxx.aarch64.rpm
    ```

    `boostkit-sra_kscann-_xxxx_.aarch64.rpm` contains the header files, dynamic library files, and static library files of KScaNN. _xxxx_ indicates the version of the KScaNN software package.

2. Install the RPM package.

    ```bash
    rpm -ivh boostsra-kscann-xxxx.aarch64.rpm
    ```

    After the installation is complete, the environment variable `LD_LIBRARY_PATH` is automatically added to `/etc/profile`, that is, the directories `/usr/local/sra_kscann/lib/` and `/usr/local/sra_kscann/lib/sve` where the KScaNN dynamic and static library files are stored.

    In the preceding command, _xxxx_ indicates the version.

## Generating a Full ScaNN Library

KScaNN depends on the open-source ScaNN optimized for Kunpeng to provide full functionality. Therefore, after installing KScaNN, obtain the source code of the ScaNN optimized for Kunpeng to compile a full ScaNN Python installation package and dynamic library files.

**Procedure<a name="section106931822175410"></a>**

1. Download the open-source ScaNN source code optimized for Kunpeng from [GitCode](https://atomgit.com/openeuler/sra_scann_adapter.git). The tag is `v2.2.1`. Save the file to a path accessible to the compiler, such as `/path/to/kscann-build`.

    ```bash
    mkdir /path/to/kscann-build && cd /path/to/kscann-build
    git clone --branch v2.2.1 --single-branch https://atomgit.com/openeuler/sra_scann_adapter.git
    ```

2. Obtain the open-source code from the google-research repository, which includes the ScaNN v1.2.10 code. Assume that the code is stored in `/path/to/kscann-build`.

    ```bash
    cd /path/to/kscann-build
    git clone https://github.com/google-research/google-research.git
    cd google-research
    git reset --hard 03c4c851a28dffe0244c65089e68d6cbf73c730b
    cp -r scann/ ../sra_scann_adapter
    ```

3. Integrate the patch file `0001-boostsra-kscann-adapter.patch` required for enabling KScaNN in ScaNN v1.2.10.

    ```bash
    cd /path/to/kscann-build/sra_scann_adapter
    patch -p1 < 0001-boostsra-kscann-adapter.patch
    ```

4. ScaNN depends on the AVX2KI library. Therefore, perform the following steps to install the AVX2KI RPM package.
    1. To install AVX2KI, obtain the software package from the [Kunpeng community](https://www.hikunpeng.com/document/detail/en/kunpengaccel/system-lib/dg-avx2ki/kunpengaccel_ksl_16_0006.html#EN-US_TOPIC_0000002507568443__li13931917173512) and verify the software package to ensure that it is consistent with the original software package on the website. Decompress the ZIP file to obtain the RPM installation package.

        >![notice](public_sys-resources/icon-notice.gif) **NOTICE:**
        >Before using the software package, read and agree to [Kunpeng BoostKit User License Agreement 2.0](https://www.hikunpeng.com/en/legal/developer/boostkit/software/protocol).

    2. <span id="li6766112117714">Obtain the verification tool and guide from</span> [Huawei enterprise website](https://support.huawei.com/enterprise/en/tool/pgp-verify-TL1000000054).
    3. Verify the software package integrity by following the instructions described in _OpenPGP Signature Verification Guide_ obtained in [4.2](#li6766112117714).
    4. Install the RPM package of AVX2KI.

        ```bash
        rpm -ivh boostkit-ksl-xxxx.aarch64.rpm
        ```

        After the installation is complete, the environment variable `LD_LIBRARY_PATH` is automatically added to `/etc/profile`, that is, the directory `/usr/local/ksl/lib` where the AVX2KI dynamic library files are located.

        In the preceding command, _xxxx_ indicates the version.

    5. Run the `source` command or log in to the terminal again for the AVX2KI environment variable to take effect.

        ```bash
        source /etc/profile
        ```

    6. Check whether the environment variable `LD_LIBRARY_PATH` contains the AVX2KI installation path `/usr/local/ksl/lib`.

        ```bash
        env | grep LD_LIBRARY_PATH
        ```

        If the variable contains the installation path, the installation is successful.

        After the installation, the target files are generated in the installation path (the default path is `/usr/local/ksl`), where the `include` folder contains the AVX2KI header files, and the `lib` folder contains the AVX2KI dynamic library files.

5. Install OpenJDK 11.

    ```bash
    yum install java-11-openjdk java-11-openjdk-devel
    ```

    Check whether OpenJDK 11 is successfully installed.

    ```bash
    java -version
    ```

    If the command output contains `openjdk version "11._x**_._x_**`, the installation is successful. An earlier OpenJDK version may cause an error during Bazel compilation.

    >![note](public_sys-resources/icon-note.gif) **NOTE:**
    >If the preceding command output shows that there is a version conflict, perform the following steps to configure the environment variable:
    >
    >```bash
    >find / -name java
    >```
    >
    >Configure the environment variable. Assume that the installation directory is `/usr/lib/jvm/java-11-openjdk-11.0.23.9-2.oe2203sp3.aarch64`.
    >
    >```bash
    >export JAVA_HOME=/usr/lib/jvm/java-11-openjdk-11.0.23.9-2.oe2203sp3.aarch64
    >export PATH=/usr/lib/jvm/java-11-openjdk-11.0.23.9-2.oe2203sp3.aarch64/bin:$PATH
    >```

6. Install Bazel 5.4.0.
    1. Download the Bazel 5.4.0 source code. Assume that the path is `/path/to/bazel`.

        ```bash
        wget https://github.com/bazelbuild/bazel/releases/download/5.4.0/bazel-5.4.0-dist.zip --no-check-certificate
        ```

    2. Decompress and compile Bazel.

        ```bash
        unzip bazel-5.4.0-dist.zip -d bazel-5.4.0
        cd bazel-5.4.0
        env EXTRA_BAZEL_ARGS="--tool_java_runtime_version=local_jdk" bash ./compile.sh
        ```

    3. After the build is successful, the generated executable file `bazel` is stored in `/path/to/bazel/bazel-5.4.0/output`. Configure the path in the environment variable `PATH` for subsequent ScaNN compilation.

        ```bash
        export PATH=/path/to/bazel/bazel-5.4.0/output:$PATH
        ```

    4. Perform the verification.

        ```bash
        bazel --version
        ```

        If the command output contains `bazel 5.4.0- (@non-git)`, the installation is successful.

7. Install GCC 12.3.1 and GCC-C++ 12.3.1.
    1. Obtain the corresponding GCC.

        ```bash
        wget https://mirrors.huaweicloud.com/kunpeng/archive/compiler/kunpeng_gcc/gcc-12.3.1-2025.06-aarch64-linux.tar.gz --no-check-certificate
        ```

    2. For details, see section [Installing GCC for openEuler](https://www.hikunpeng.com/document/detail/en/kunpengdevps/compiler/ug-hgcc/kunpenghgcc_06_0004.html) in the _GCC for openEuler User Guide_.

        ```bash
        export CC=/opt/aarch64/compiler/gcc-12.3.1-2025.06-aarch64-linux/bin/gcc
        export CXX=/opt/aarch64/compiler/gcc-12.3.1-2025.06-aarch64-linux/bin/g++
        ```

8. Install the compilation dependencies.

    ```bash
    yum install python python3-devel python3-pip rsync libomp libuuid-devel
    ```

    Ensure that KScaNN is located in `/usr/local/sra_recall/lib/kscann` and AVX2KI is located in `/usr/local/ksl/lib`.

9. Start the build.

    1. Specify the KScaNN installation directory. The installation directory is `/usr/local/sra_kscann`. Configure a proper pip repository.

        ```bash
        export KSCANN_PATH=/usr/local/sra_kscann
        ```

    2. Run the following commands to install the dependencies:

        ```bash
        cd /path/to/scann
        sh project.sh --prepare
        ```

    3. Run the following command to build the Python installation package of ScaNN:

        ```bash
        sh project.sh --build_whl
        ```

    4. The resulting Python installation package `scann-1.2.10-cp39-cp39-linux_aarch64.whl` is stored in `/path/to/kscann-build/scann`.
    5. Run the following command to build the dynamic library file of ScaNN:

        ```bash
        sh project.sh --build_scann_cc_sve
        ```

        The resulting dynamic library file `libscann_cc.so` is stored in `/path/to/kscann-build/scann`.

        >![note](public_sys-resources/icon-note.gif) **NOTE:**
        >`project.sh` contains the following compilation options. You can select them as required:
        >- --`prepare`: installs Python dependencies.
        >- --`build_whl`: builds the full Python installation package of ScaNN.
        >- --`build_scann_cc_sve`: builds the full ScaNN dynamic library file optimized with SVE instructions.
        >- --`build_scann_cc_neon`: builds the full ScaNN dynamic library file optimized with NEON instructions.
        >- --`build_scann_cc_sve_milvus`: builds the full ScaNN dynamic library file optimized with SVE instructions for Milvus.
        >- --`build_scann_cc_neon_milvus`: builds the full ScaNN dynamic library file optimized with NEON instructions for Milvus .
        >
        >If the message "unable to find valid certification path to requested target" is displayed during environment setup, see [The Certificate Path Cannot Be Found During ScaNN Compilation](https://www.hikunpeng.com/document/detail/en/SRA/ecosystemEnable/ScaNN/kunpengscann_02_0014.html) in the _ScaNN Porting Guide_.

10. Install the WHL file.

    ```bash
    pip install scann-1.2.10-cp39-cp39-linux_aarch64.whl
    ```

11. Run the `pip show` command to check whether ScaNN 1.2.10 has been installed.

    ```bash
    pip show scann
    ```

    If the command output reads `Name: scann Version: 1.2.10`, the installation is successful.

## Uninstalling KScaNN

**RPM Package Uninstallation<a name="section118069490504"></a>**

During uninstallation, service flows that are being executed are affected. You are advised to stop the service flows before uninstalling KScaNN. Using parameters supported by the RPM package manager but not documented in this guide may result in undefined behavior. Proceed with caution.

1. Run the `rpm -e` command to uninstall the RPM package.

    ```bash
    rpm -e boostsra-kscann
    ```

2. Verify that the installation directory `/usr/local/sra_kscann` is deleted.
3. Verify that the `/etc/profile` file does not contain environment variables related to `/usr/local/sra_kscann`.

**WHL Package Uninstallation<a name="section58079490509"></a>**

1. Run the `pip uninstall` command to uninstall the WHL file.

    ```bash
    pip uninstall scann
    ```

2. Run the `pip show` command to check whether ScaNN 1.2.10 has been uninstalled.

    ```bash
    pip show scann
    ```

    If the command output reads `WARNING: Package(s) not found: scann`, the uninstallation is successful.
