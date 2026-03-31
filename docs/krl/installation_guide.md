# 安装指南

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

### RPM安装

本节提供RPM包安装KRL方法。请参照本节内容对KRL进行安装和安装后验证。若操作过程中使用了RPM包管理工具支持但本文档中未说明的参数，可能会引入未定义行为，请谨慎操作。

1. 从GitCode仓获取对应的鲲鹏检索算子库软件安装包[BoostKit-boostsra-krl\_1.0.0.zip](https://gitcode.com/boostkit/boostsra/releases/download/v1.0.0/BoostKit-SRA_KRL-1.0.0.zip)，用户解压zip文件后可获取RPM安装包。

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

    安装结束后，自动追加环境变量LD\_LIBRARY\_PATH到“/etc/profile“中，即KRL的动态库文件所在目录“/usr/local/sra\_krl/lib“。

    上述命令中涉及的 **_xxxx_** 代表版本号。

3. 执行**source**命令或重新登录终端使环境变量生效。

    ```bash
    source /etc/profile
    ```

4. 查看环境变量LD\_LIBRARY\_PATH是否包含KRL的安装路径“/usr/local/sra\_krl/lib“。

    ```bash
    env | grep LD_LIBRARY_PATH
    ```

    如果变量包含安装路径，说明安装成功。

    安装成功后在安装路径（默认路径是“/usr/local/sra\_krl“）下生成相应文件，其中，“include“文件夹包含KRL的头文件，“lib“文件夹包含了KRL的动态库文件。

## 卸载KRL

如需要卸载KRL，请先停止调用KRL的业务流再进行卸载操作。若操作过程中使用了RPM包管理工具支持但本文档中未说明的参数，可能会引入未定义行为，请谨慎操作。

**RPM包卸载<a name="section175738555173"></a>**

1. 执行**rpm -e**命令卸载RPM安装包。

    ```bash
    rpm -e boostkit-sra_krl
    ```

2. 确认安装目录“/usr/local/sra\_krl“被删除。
3. 确认“/etc/profile“文件中无“/usr/local/sra\_krl“相关环境变量。
