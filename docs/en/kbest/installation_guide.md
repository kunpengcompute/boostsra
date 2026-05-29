# Installation Guide

## Verified Environments

To use KBest smoothly and securely, ensure that your environment is one of the verified environments.

**Table 1** Verified environments for KBest<a id="verified environments for kbest"></a>

<a name="table4692134313211"></a>
<table><thead align="left"><tr id="row1169294312212"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.6.1.1"><p id="p12692144313211"><a name="p12692144313211"></a><a name="p12692144313211"></a>OS</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.6.1.2"><p id="p06926438214"><a name="p06926438214"></a><a name="p06926438214"></a>CPU</p>
</th>
<th class="cellrowborder" valign="top" width="15%" id="mcps1.2.6.1.3"><p id="p269284310216"><a name="p269284310216"></a><a name="p269284310216"></a>Memory </p>
</th>
<th class="cellrowborder" valign="top" width="15%" id="mcps1.2.6.1.4"><p id="p196922434215"><a name="p196922434215"></a><a name="p196922434215"></a> Compiler </p>
</th>
<th class="cellrowborder" valign="top" width="30%" id="mcps1.2.6.1.5"><p id="p1769219435210"><a name="p1769219435210"></a><a name="p1769219435210"></a>Other</p>
</th>
</tr>
</thead>
<tbody><tr id="row13692643162117"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p4692104312120"><a name="p4692104312120"></a><a name="p4692104312120"></a>openEuler 22.03 LTS SP3</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p9692124320219"><a name="p9692124320219"></a><a name="p9692124320219"></a> New Kunpeng 920 processor model</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.6.1.3 "><p id="p2692443182119"><a name="p2692443182119"></a><a name="p2692443182119"></a>16 × 32 GB</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.6.1.4 "><p id="p1269354352117"><a name="p1269354352117"></a><a name="p1269354352117"></a>GCC 12.3.1</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.6.1.5 "><a name="ul46932043172116"></a><a name="ul46932043172116"></a><ul id="ul46932043172116"><li>CMake&gt;=3.22.0</li><li>GLIBCXX&gt;=3.4.29</li><li>Python 3.9.x</li></ul>
</td>
</tr>
<tr id="row1032642113386"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p1599891016456"><a name="p1599891016456"></a><a name="p1599891016456"></a>openEuler 22.03 LTS SP3</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p383962264515"><a name="p383962264515"></a><a name="p383962264515"></a> New Kunpeng 920 processor model</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.6.1.3 "><p id="p129975359453"><a name="p129975359453"></a><a name="p129975359453"></a>16 × 32 GB</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.6.1.4 "><p id="p3686322143815"><a name="p3686322143815"></a><a name="p3686322143815"></a>GCC 10.3.1</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.6.1.5 "><a name="ul1968672223815"></a><a name="ul1968672223815"></a><ul id="ul1968672223815"><li>CMake&gt;=3.22.0</li><li>GLIBCXX&gt;=3.4.28</li><li>Python 3.9.x</li></ul>
</td>
</tr>
<tr id="row94251327203812"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p6751171816390"><a name="p6751171816390"></a><a name="p6751171816390"></a>openEuler 24.03 LTS SP1</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p14840522154517"><a name="p14840522154517"></a><a name="p14840522154517"></a> New Kunpeng 920 processor model</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.6.1.3 "><p id="p14997183511454"><a name="p14997183511454"></a><a name="p14997183511454"></a>16 × 32 GB</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.6.1.4 "><p id="p382782815383"><a name="p382782815383"></a><a name="p382782815383"></a>GCC 12.3.1</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.6.1.5 "><a name="ul382832843816"></a><a name="ul382832843816"></a><ul id="ul382832843816"><li>CMake&gt;=3.22.0</li><li>GLIBCXX&gt;=3.4.29</li><li>Python 3.9.x</li></ul>
</td>
</tr>
<tr id="row7960171410516"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p89601314753"><a name="p89601314753"></a><a name="p89601314753"></a>openEuler 24.03 LTS SP3</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p129602141518"><a name="p129602141518"></a><a name="p129602141518"></a>Kunpeng 950 processor</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.6.1.3 "><p id="p1960514556"><a name="p1960514556"></a><a name="p1960514556"></a>24 × 64 GB</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.6.1.4 "><p id="p8960151411513"><a name="p8960151411513"></a><a name="p8960151411513"></a>GCC 12.3.1</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.6.1.5 "><a name="ul19960214955"></a><a name="ul19960214955"></a><ul id="ul19960214955"><li>CMake&gt;=3.22.0</li><li>GLIBCXX&gt;=3.4.29</li><li>Python 3.9.x</li></ul>
</td>
</tr>
</tbody>
</table>

## Installing KBest

### Installation Using an RPM Package

This section describes how to install KBest using the RPM package and verify KBest. Using parameters supported by the RPM package manager but not documented in this guide may result in undefined behavior. Proceed with caution.

**Installation Procedure <a name="section349212333315"></a>**

1. Obtain the KBest software package [BoostKit-boostsra-kbest\_2.2.0.zip](https://gitcode.com/boostkit/boostsra/releases/download/v1.1.0/BoostKit-boostsra-kbest_2.2.0.zip) from GitCode and extract the archive to obtain the binary RPM package and WHL file.

    The software package structure is as follows.

    ```text
    ├── boostsra-kbest-xxxx.aarch64.rpm
    └── boostsra-kbest-xxxx-cp39-cp39-linux_aarch64.whl
    ```

    <code>boostsra-kbest-_*xxxx*_.aarch64.rpm</code> contains the header files and dynamic library files of KBest. <code>boostsra-kbest-_*xxxx*_-cp39-cp39-linux\_aarch64.whl</code> is the required installation package for testing the KBest Python framework. <code>_xxxx_</code> indicates the version of the KBest software package.

2. Install the RPM package.

    ```bash
    rpm -ivh boostsra-kbest-xxxx.aarch64.rpm
    ```

    After the installation is complete, the environment variable <code>LD_LIBRARY_PATH</code> is automatically added to <code>/etc/profile</code>, that is, the directory <code>/usr/local/sra_kbest/lib</code> where the KBest dynamic library file is located.

    In the preceding command, <code>_xxxx_</code> indicates the version.

3. Install the WHL file.

    ```bash
    pip install boostsra-kbest-xxxx-cp39-cp39-linux_aarch64.whl
    ```

    In the preceding command, <code>_xxxx_</code> indicates the version.

**Verifying the Installation <a name="section10493153333112"></a>**

1. Run the <code>source</code> command or re-log in to the terminal to apply the environment variable.

    ```bash
    source /etc/profile
    ```

2. Check whether the environment variable <code>LD_LIBRARY_PATH</code> contains the KBest installation path <code>/usr/local/sra_kbest/lib</code>.

    ```bash
    env | grep LD_LIBRARY_PATH
    ```

    If the variable contains the installation path, the installation is successful.

    After the installation, the corresponding files are generated in the installation path (the default path is <code>/usr/local/sra\_kbest</code>). The <code>include</code> folder contains the header files of KBest, the <code>lib</code> folder contains the dynamic library files of KBest.

3. Run the <code>pip show</code> command to check whether KBest <code>_xxxx_</code> has been installed.

    ```bash
    pip show kbest
    ```

    If the command output reads "Name: kbest Version: <code>_xxxx_</code>", the installation is successful.

## Uninstalling KBest

**Uninstalling the RPM Package <a name="section154931433123117"></a>**

During uninstallation, service flows that are being executed are affected. You are advised to stop the service flows before uninstalling KBest. Using parameters supported by the RPM package manager but not documented in this guide may result in undefined behavior. Proceed with caution.

1. Run the <code>rpm -e</code> command to uninstall the RPM package.

    ```bash
    rpm -e boostsra-kbest
    ```

2. Verify that the installation directory <code>/usr/local/sra\_kbest</code> is deleted.
3. Verify that the <code>/etc/profile</code> file does not contain environment variables related to <code>/usr/local/sra\_kbest</code>.

**Uninstalling the WHL Package <a name="section7493143393110"></a>**

1. Run the <code>pip uninstall</code> command to uninstall the WHL file.

    ```bash
    pip uninstall kbest
    ```

2. Run the <code>pip show</code> command to check whether KBest <code>_xxxx_</code> has been uninstalled.

    ```bash
    pip show kbest
    ```

    If the command output reads "WARNING: Package\(s\) not found: kbest", the uninstallation is successful.
