# Installation Guide

## Verified Environments

To use KRL smoothly and securely, ensure that your environment is one of the verified environments.

**Table 1** Verified environments for KRL<a id="verified-environments-for-krl"></a>

<a name="table113653362525"></a>
<table><thead align="left"><tr id="row2036563612525"><th class="cellrowborder" valign="top" width="21.77%" id="mcps1.2.6.1.1"><p id="p10365836165218"><a name="p10365836165218"></a><a name="p10365836165218"></a>OS</p>
</th>
<th class="cellrowborder" valign="top" width="23.5%" id="mcps1.2.6.1.2"><p id="p53652363523"><a name="p53652363523"></a><a name="p53652363523"></a>CPU</p>
</th>
<th class="cellrowborder" valign="top" width="18.44%" id="mcps1.2.6.1.3"><p id="p136510367522"><a name="p136510367522"></a><a name="p136510367522"></a>Memory</p>
</th>
<th class="cellrowborder" valign="top" width="16.900000000000002%" id="mcps1.2.6.1.4"><p id="p20365836185215"><a name="p20365836185215"></a><a name="p20365836185215"></a>Compiler</p>
</th>
<th class="cellrowborder" valign="top" width="19.39%" id="mcps1.2.6.1.5"><p id="p6365123615524"><a name="p6365123615524"></a><a name="p6365123615524"></a>CMake</p>
</th>
</tr>
</thead>
<tbody><tr id="row10365113685217"><td class="cellrowborder" valign="top" width="21.77%" headers="mcps1.2.6.1.1 "><p id="p1636573614523"><a name="p1636573614523"></a><a name="p1636573614523"></a>openEuler 22.03 LTS SP3</p>
</td>
<td class="cellrowborder" valign="top" width="23.5%" headers="mcps1.2.6.1.2 "><p id="p173654366528"><a name="p173654366528"></a><a name="p173654366528"></a>New Kunpeng 920 processor model</p>
</td>
<td class="cellrowborder" valign="top" width="18.44%" headers="mcps1.2.6.1.3 "><p id="p636533625218"><a name="p636533625218"></a><a name="p636533625218"></a>16 × 32 GB</p>
</td>
<td class="cellrowborder" valign="top" width="16.900000000000002%" headers="mcps1.2.6.1.4 "><p id="p103651036185219"><a name="p103651036185219"></a><a name="p103651036185219"></a>GCC 12.3.1</p>
</td>
<td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.6.1.5 "><p id="p285111515577"><a name="p285111515577"></a><a name="p285111515577"></a>&gt;=3.22.0</p>
</td>
</tr>
<tr id="row10335834165819"><td class="cellrowborder" valign="top" width="21.77%" headers="mcps1.2.6.1.1 "><p id="p7336183465815"><a name="p7336183465815"></a><a name="p7336183465815"></a>openEuler 24.03 LTS SP3</p>
</td>
<td class="cellrowborder" valign="top" width="23.5%" headers="mcps1.2.6.1.2 "><p id="p15336103415817"><a name="p15336103415817"></a><a name="p15336103415817"></a>Kunpeng 950 processor</p>
</td>
<td class="cellrowborder" valign="top" width="18.44%" headers="mcps1.2.6.1.3 "><p id="p233663465818"><a name="p233663465818"></a><a name="p233663465818"></a>24 ×* 64 GB</p>
</td>
<td class="cellrowborder" valign="top" width="16.900000000000002%" headers="mcps1.2.6.1.4 "><p id="p12971140142310"><a name="p12971140142310"></a><a name="p12971140142310"></a>GCC 12.3.1</p>
</td>
<td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.6.1.5 "><p id="p102524252319"><a name="p102524252319"></a><a name="p102524252319"></a>&gt;=3.22.0</p>
</td>
</tr>
</tbody>
</table>

## Installing KRL

### Installation Using an RPM Package

This section describes how to install KRL using the RPM package and verify the package. If you use parameters that are supported by the RPM package management tool but not described in this document, undefined behavior may be introduced. Exercise caution when performing this operation.

1. Obtain the KRL software installation package [BoostKit-boostsra-krl\_1.0.0.zip](https://gitcode.com/boostkit/boostsra/releases/download/v1.0.0/BoostKit-SRA_KRL-1.0.0.zip) from the GitCode repository. Decompress the ZIP file to obtain the RPM installation package.

    >![note](public_sys-resources/icon-note.gif) **NOTE**
    >- The KRL software package consists of the following files:
    >
    > ```text
    > ├── boostsra-krl-xxxx.aarch64.rpm
    > └── 0001-faiss-1.8.0-add-krl.patch
    >    ```
    >
    > `boostsra-krl-_xxxx_aarch64.rpm` contains the KRL header files and dynamic library files. `0001-faiss-1.8.0-add-krl.patch` is the patch file required for enabling KRL in Faiss 1.8.0. _xxxx_ indicates the KRL software package version.

2. Install the RPM package.

    ```bash
    rpm -ivh boostsra-krl-xxxx.aarch64.rpm
    ```

    After the installation is complete, the environment variable `LD\_LIBRARY\_PATH` is automatically added to `/etc/profile`, that is, the directory `/usr/local/sra\_krl/lib` where the KRL dynamic library files are located.

    In the preceding command, _xxxx_ indicates the version.

3. Run the `source` command or re-log in to the terminal to apply the environment variable.

    ```bash
    source /etc/profile
    ```

4. Check whether the environment variable `LD_LIBRARY_PATH` contains the KRL installation path `/usr/local/sra\_krl/lib`.

    ```bash
    env | grep LD_LIBRARY_PATH
    ```

    If the variable contains the installation path, the installation is successful.

    After the installation, the corresponding files are generated in the installation path (the default path is `/usr/local/sra\_krl`). The `include` folder contains the header files of KRL, the `lib` folder contains the dynamic library files of KRL.

## Uninstalling KRL

Before uninstalling KRL, make sure to stop any service flows that depend on it. If you use parameters that are supported by the RPM package management tool but not described in this document, undefined behavior may be introduced. Exercise caution when performing this operation.

**Uninstalling the RPM Package <a name="section175738555173"></a>**

1. Run the `rpm -e` command to uninstall the RPM package.

    ```bash
    rpm -e boostkit-sra_krl
    ```

2. Verify that the installation directory `/usr/local/sra\_krl` is deleted.
3. Verify that the `/etc/profile` file does not contain environment variables related to `/usr/local/sra\_krl`.
