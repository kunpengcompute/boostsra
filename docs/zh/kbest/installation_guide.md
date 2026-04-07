# 安装指南

## 已验证环境

为保证您可以顺利安全地使用KBest，请确保所使用的环境信息在已验证环境范围内。

**表 1** KBest已验证环境<a id="KBest已验证环境"></a>

<a name="table4692134313211"></a>
<table><thead align="left"><tr id="row1169294312212"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.6.1.1"><p id="p12692144313211"><a name="p12692144313211"></a><a name="p12692144313211"></a>操作系统</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.6.1.2"><p id="p06926438214"><a name="p06926438214"></a><a name="p06926438214"></a>CPU类型</p>
</th>
<th class="cellrowborder" valign="top" width="15%" id="mcps1.2.6.1.3"><p id="p269284310216"><a name="p269284310216"></a><a name="p269284310216"></a>内存</p>
</th>
<th class="cellrowborder" valign="top" width="15%" id="mcps1.2.6.1.4"><p id="p196922434215"><a name="p196922434215"></a><a name="p196922434215"></a>编译器</p>
</th>
<th class="cellrowborder" valign="top" width="30%" id="mcps1.2.6.1.5"><p id="p1769219435210"><a name="p1769219435210"></a><a name="p1769219435210"></a>其他</p>
</th>
</tr>
</thead>
<tbody><tr id="row13692643162117"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p4692104312120"><a name="p4692104312120"></a><a name="p4692104312120"></a>openEuler 22.03 LTS SP3</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p9692124320219"><a name="p9692124320219"></a><a name="p9692124320219"></a>鲲鹏920 7282C处理器</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.6.1.3 "><p id="p2692443182119"><a name="p2692443182119"></a><a name="p2692443182119"></a>16*32GB</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.6.1.4 "><p id="p1269354352117"><a name="p1269354352117"></a><a name="p1269354352117"></a>GCC 12.3.1</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.6.1.5 "><a name="ul46932043172116"></a><a name="ul46932043172116"></a><ul id="ul46932043172116"><li>CMake&gt;=3.22.0</li><li>GLIBCXX&gt;=3.4.29</li><li>Python 3.9.x</li></ul>
</td>
</tr>
<tr id="row1032642113386"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p1599891016456"><a name="p1599891016456"></a><a name="p1599891016456"></a>openEuler 22.03 LTS SP3</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p383962264515"><a name="p383962264515"></a><a name="p383962264515"></a>鲲鹏920 7282C处理器</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.6.1.3 "><p id="p129975359453"><a name="p129975359453"></a><a name="p129975359453"></a>16*32GB</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.6.1.4 "><p id="p3686322143815"><a name="p3686322143815"></a><a name="p3686322143815"></a>GCC 10.3.1</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.6.1.5 "><a name="ul1968672223815"></a><a name="ul1968672223815"></a><ul id="ul1968672223815"><li>CMake&gt;=3.22.0</li><li>GLIBCXX&gt;=3.4.28</li><li>Python 3.9.x</li></ul>
</td>
</tr>
<tr id="row94251327203812"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p6751171816390"><a name="p6751171816390"></a><a name="p6751171816390"></a>openEuler 24.03 LTS SP1</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p14840522154517"><a name="p14840522154517"></a><a name="p14840522154517"></a>鲲鹏920 7282C处理器</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.6.1.3 "><p id="p14997183511454"><a name="p14997183511454"></a><a name="p14997183511454"></a>16*32GB</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.6.1.4 "><p id="p382782815383"><a name="p382782815383"></a><a name="p382782815383"></a>GCC 12.3.1</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.6.1.5 "><a name="ul382832843816"></a><a name="ul382832843816"></a><ul id="ul382832843816"><li>CMake&gt;=3.22.0</li><li>GLIBCXX&gt;=3.4.29</li><li>Python 3.9.x</li></ul>
</td>
</tr>
<tr id="row7960171410516"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p89601314753"><a name="p89601314753"></a><a name="p89601314753"></a>openEuler 24.03 LTS SP3</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p129602141518"><a name="p129602141518"></a><a name="p129602141518"></a>鲲鹏950 7592C处理器</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.6.1.3 "><p id="p1960514556"><a name="p1960514556"></a><a name="p1960514556"></a>24*64GB</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.6.1.4 "><p id="p8960151411513"><a name="p8960151411513"></a><a name="p8960151411513"></a>GCC 12.3.1</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.6.1.5 "><a name="ul19960214955"></a><a name="ul19960214955"></a><ul id="ul19960214955"><li>CMake&gt;=3.22.0</li><li>GLIBCXX&gt;=3.4.29</li><li>Python 3.9.x</li></ul>
</td>
</tr>
</tbody>
</table>

## 安装KBest

### RPM安装

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

    安装结束后，自动追加环境变量LD\_LIBRARY\_PATH到“/etc/profile“中，即KBest的动态库文件所在目录“/usr/local/sra\_kbest/lib“。

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

2. 查看环境变量LD\_LIBRARY\_PATH是否包含KBest的安装路径“/usr/local/sra\_kbest/lib“。

    ```bash
    env | grep LD_LIBRARY_PATH
    ```

    如果变量包含安装路径，说明安装成功。

    安装成功后在安装路径（默认路径是“/usr/local/sra\_kbest“）下生成相应文件，其中，“include“文件夹包含KBest的头文件，“lib“文件夹包含了KBest的动态库文件。

3. 执行**pip** **show**命令确认kbest== **_xxxx_** 已安装。

    ```bash
    pip show kbest
    ```

    如果输出包含Name: kbest Version:  **_xxxx_**，则已安装成功。

## 卸载KBest

**RPM包卸载<a name="section154931433123117"></a>**

卸载KBest将会影响您正在执行的业务流，建议先停止正在执行的业务流再进行卸载操作。若操作过程中使用了RPM包管理工具支持但本文档中未说明的参数，可能会引入未定义行为，请谨慎操作。

1. 执行**rpm -e**命令卸载RPM安装包。

    ```bash
    rpm -e boostsra-kbest
    ```

2. 确认安装目录“/usr/local/sra\_kbest“被删除。
3. 确认“/etc/profile“文件中无“/usr/local/sra\_kbest“相关环境变量。

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
