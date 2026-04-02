# 安装指南

## 已验证环境

为保证您可以顺利安全地使用KDNN，请确保所使用的环境信息在已验证环境范围内。

**表 1** KDNN已验证环境<a id="KDNN已验证环境"></a>

<a name="zh-cn_topic_0000001831167081_table2919mcpsimp"></a>
<table><thead align="left"><tr id="zh-cn_topic_0000001831167081_row2926mcpsimp"><th class="cellrowborder" valign="top" width="12.15%" id="mcps1.2.7.1.1"><p id="p672213451215"><a name="p672213451215"></a><a name="p672213451215"></a>组件</p>
</th>
<th class="cellrowborder" valign="top" width="19.97%" id="mcps1.2.7.1.2"><p id="zh-cn_topic_0000001831167081_p2928mcpsimp"><a name="zh-cn_topic_0000001831167081_p2928mcpsimp"></a><a name="zh-cn_topic_0000001831167081_p2928mcpsimp"></a>操作系统</p>
</th>
<th class="cellrowborder" valign="top" width="22.32%" id="mcps1.2.7.1.3"><p id="zh-cn_topic_0000001831167081_p2930mcpsimp"><a name="zh-cn_topic_0000001831167081_p2930mcpsimp"></a><a name="zh-cn_topic_0000001831167081_p2930mcpsimp"></a>CPU类型</p>
</th>
<th class="cellrowborder" valign="top" width="18.94%" id="mcps1.2.7.1.4"><p id="zh-cn_topic_0000001831167081_p94235351693"><a name="zh-cn_topic_0000001831167081_p94235351693"></a><a name="zh-cn_topic_0000001831167081_p94235351693"></a>编译器</p>
</th>
<th class="cellrowborder" valign="top" width="11.07%" id="mcps1.2.7.1.5"><p id="p157041029488"><a name="p157041029488"></a><a name="p157041029488"></a>构建工具</p>
</th>
<th class="cellrowborder" valign="top" width="15.55%" id="mcps1.2.7.1.6"><p id="p10171835144516"><a name="p10171835144516"></a><a name="p10171835144516"></a>Python解释器</p>
</th>
</tr>
</thead>
<tbody><tr id="row056323751218"><td class="cellrowborder" valign="top" width="12.15%" headers="mcps1.2.7.1.1 "><p id="p7180194317123"><a name="p7180194317123"></a><a name="p7180194317123"></a>KDNN</p>
</td>
<td class="cellrowborder" valign="top" width="19.97%" headers="mcps1.2.7.1.2 "><p id="p16180743171218"><a name="p16180743171218"></a><a name="p16180743171218"></a>openEuler 22.03 LTS SP3</p>
</td>
<td class="cellrowborder" valign="top" width="22.32%" headers="mcps1.2.7.1.3 "><p id="p818014317128"><a name="p818014317128"></a><a name="p818014317128"></a>华为鲲鹏920 7270Z/7280Z处理器</p>
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
<p id="p618613441416"><a name="p618613441416"></a><a name="p618613441416"></a>内核版本高于5.10.0-228.0.0.127</p>
</td>
<td class="cellrowborder" valign="top" width="22.32%" headers="mcps1.2.7.1.3 "><p id="p161878491412"><a name="p161878491412"></a><a name="p161878491412"></a>华为鲲鹏920新型号处理器</p>
</td>
<td class="cellrowborder" valign="top" width="18.94%" headers="mcps1.2.7.1.4 "><p id="p6187843140"><a name="p6187843140"></a><a name="p6187843140"></a>GCC 12.3.1/毕昇 4.2.0</p>
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
<td class="cellrowborder" valign="top" width="22.32%" headers="mcps1.2.7.1.3 "><p id="zh-cn_topic_0000001831167081_p1871451912230"><a name="zh-cn_topic_0000001831167081_p1871451912230"></a><a name="zh-cn_topic_0000001831167081_p1871451912230"></a>华为鲲鹏920系列处理器</p>
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

>![](public_sys-resources/icon-notice.gif) **须知：** 
>
>- KDNN目前支持鲲鹏920 7270Z/7280Z处理器、鲲鹏920新型号处理器，使用其他处理器可能会造成未定义的结果。
>- KDNN为底层原语库，计算流程涉及内存读写、分配。KDNN不提供也不发布操作系统，操作系统须用户自行安装，不承担操作系统的安全责任，用户需要结合自身应用对操作系统安全加固，包括不安装或者移除不必要的应用等。
>- 为阻止缓冲区溢出攻击，建议使用ASLR（Address Space Layout Randomization）技术，通过对堆、栈、共享库映射等线性区布局的随机化，增加攻击者预测目的地址的难度，防止攻击者直接定位攻击代码位置。该技术可作用于堆、栈、内存映射区（mmap基址、shared libraries、vdso页）。
> 开启方式：**echo 2 \>/proc/sys/kernel/randomize\_va\_space**

## 配置网络代理<a name="ZH-CN_TOPIC_0000002518232616"></a>

如果环境无法直接访问外网，则需要配置网络代理。本章节提供临时配置和永久配置两种方法，永久配置网络代理有密码泄露的风险，环境中的所有用户均能获取配置的密码，因此推荐临时配置网络代理。您可以根据实际情况选择合理的配置方法。

**方法1：临时配置网络代理<a name="section1694205085318"></a>**

1. 配置环境变量。

    其中，用户名、密码、代理IP地址和代理端口请根据实际情况填写。

    ```bash
    export http_proxy="http://用户名:密码@代理IP地址:代理端口" 
    export https_proxy=$http_proxy
    ```

2. 确认可以访问外网。

    使用**curl**命令访问任意网站，若能显示网站信息则表示代理配置成功，可以访问外网。

**方法2：永久配置网络代理<a name="section49515065317"></a>**

1. 修改profile文件。
    1. 打开“/etc/profile“文件。

        ```bash
        vi /etc/profile
        ```

    2. 按“i“进入编辑模式，在“/etc/profile“文件中增加以下内容。

        其中，用户名、密码、代理IP地址和代理端口请根据实际情况填写。

        ```bash
        export http_proxy="http://用户名:密码@代理IP地址:代理端口" 
        export https_proxy=$http_proxy 
        export no_proxy=127.0.0.1,localhost,local,.local
        ```

    3. 按“Esc“键，输入**:wq!**，按“Enter“保存并退出编辑。
    4. 使代理生效。

        ```bash
        source /etc/profile
        ```

2. 确认可以访问外网。

    使用**curl**命令访问任意网站，若能显示网站信息则表示代理配置成功，可以访问外网。

## 安装环境依赖

本章节使用Yum源方式安装GCC/G++等系统依赖的基础软件。

1. 执行以下命令安装系统依赖。

    ```bash
    yum install make git gcc-c++ cmake
    ```

2. 执行以下命令安装NumPy（若使用KDNN\_EXT组件，需执行该步骤）。

    ```bash
    pip install numpy==1.24.2
    ```

3. 安装编译器GCC 10.3.1或者GCC 12.3.1或者毕昇4.2.0。

## 获取软件包

安装KDNN之前请先从官网地址获取软件包，再进行软件包校验，确保与网站上的原始软件包一致。

1. 从鲲鹏社区获取对应的软件数字证书和软件安装包，用户解压zip文件后可获取RPM安装包。

    **表 1** KDNN软件包获取列表<a id="KDNN软件包获取列表"></a>

    <a name="zh-cn_topic_0000001784526702_table677mcpsimp"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0000001784526702_row684mcpsimp"><th class="cellrowborder" valign="top" width="28.96%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0000001784526702_p686mcpsimp"><a name="zh-cn_topic_0000001784526702_p686mcpsimp"></a><a name="zh-cn_topic_0000001784526702_p686mcpsimp"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="32.04%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0000001784526702_p688mcpsimp"><a name="zh-cn_topic_0000001784526702_p688mcpsimp"></a><a name="zh-cn_topic_0000001784526702_p688mcpsimp"></a>包名</p>
    </th>
    <th class="cellrowborder" valign="top" width="39%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0000001784526702_p690mcpsimp"><a name="zh-cn_topic_0000001784526702_p690mcpsimp"></a><a name="zh-cn_topic_0000001784526702_p690mcpsimp"></a>获取地址</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0000001784526702_row692mcpsimp"><td class="cellrowborder" valign="top" width="28.96%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0000001784526702_p694mcpsimp"><a name="zh-cn_topic_0000001784526702_p694mcpsimp"></a><a name="zh-cn_topic_0000001784526702_p694mcpsimp"></a>KDNN软件包（GCC版本）</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.04%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0000001784526702_p696mcpsimp"><a name="zh-cn_topic_0000001784526702_p696mcpsimp"></a><a name="zh-cn_topic_0000001784526702_p696mcpsimp"></a>BoostKit-boostcore-kdnn.3.1.0.zip<sup id="sup81399218186"><a name="sup81399218186"></a><a name="sup81399218186"></a>a</sup></p>
    </td>
    <td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p125955276200"><a name="p125955276200"></a><a name="p125955276200"></a><a href="https://gitcode.com/boostkit/boostsra/releases/download/v1.2.0/BoostKit-boostcore-kdnn_3.1.0.zip" target="_blank" rel="noopener noreferrer">获取链接</a></p>
    </td>
    </tr>
    <tr id="row1487285541019"><td class="cellrowborder" valign="top" width="28.96%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0000001784526702_p708mcpsimp"><a name="zh-cn_topic_0000001784526702_p708mcpsimp"></a><a name="zh-cn_topic_0000001784526702_p708mcpsimp"></a>KDNN软件包（毕昇编译器版本）</p>
    </td>
    <td class="cellrowborder" valign="top" width="32.04%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0000001784526702_p711mcpsimp"><a name="zh-cn_topic_0000001784526702_p711mcpsimp"></a><a name="zh-cn_topic_0000001784526702_p711mcpsimp"></a>BoostKit-boostcore-kdnn.3.0.0_bisheng.zip<sup id="sup195471318183"><a name="sup195471318183"></a><a name="sup195471318183"></a>a</sup></p>
    </td>
    <td class="cellrowborder" valign="top" width="39%" headers="mcps1.2.4.1.3 "><p id="p141301730112014"><a name="p141301730112014"></a><a name="p141301730112014"></a><a href="https://gitcode.com/boostkit/boostsra/releases/download/v1.1.0/BoostKit-boostcore-kdnn_3.0.0_bisheng.zip" target="_blank" rel="noopener noreferrer">获取链接</a></p>
    </td>
    </tr>
    <tr id="row1660012761511"><td class="cellrowborder" colspan="3" valign="top" headers="mcps1.2.4.1.1 mcps1.2.4.1.2 mcps1.2.4.1.3 "><p id="p1238171011299"><a name="p1238171011299"></a><a name="p1238171011299"></a>a：<span id="zh-cn_topic_0000001784116274_ph22354711282"><a name="zh-cn_topic_0000001784116274_ph22354711282"></a><a name="zh-cn_topic_0000001784116274_ph22354711282"></a>使用软件包前请先阅读<span id="zh-cn_topic_0000001784116274_zh-cn_topic_0000001784116274_ph16146198202211"><a name="zh-cn_topic_0000001784116274_zh-cn_topic_0000001784116274_ph16146198202211"></a><a name="zh-cn_topic_0000001784116274_zh-cn_topic_0000001784116274_ph16146198202211"></a>《<a href="https://www.hikunpeng.com/zh/legal/developer/boostkit/software/protocol" target="_blank" rel="noopener noreferrer">鲲鹏应用使能套件BoostKit用户许可协议 2.0</a>》</span>，如确认继续使用，则默认同意协议的条款和条件。</span></p>
    </td>
    </tr>
    </tbody>
    </table>

2. <a name="zh-cn_topic_0000001784526702_li178091993411"></a>从[华为企业业务网站](https://support.huawei.com/enterprise/zh/tool/pgp-verify-TL1000000054)获取校验工具和校验方法。
3. 参见[2](#zh-cn_topic_0000001784526702_li178091993411)中下载的《OpenPGP签名验证指南》进行软件包完整性检查。

## 如何使用KDNN

### 安装KDNN

本文提供RPM包安装KDNN的方法，请参照本节内容对KDNN进行安装和验证。若使用了RPM包管理工具支持但本文档中未说明的参数，可能会引入未定义行为，因此请谨慎操作。

**安装步骤<a name="section39201312169"></a>**

1. 按照[获取软件包](#获取软件包)获取到KDNN软件包，解压后得到二进制RPM包。
2. 安装KDNN。

    ```bash
    rpm -ivh boostcore-kdnn-xxxx.aarch64.rpm
    ```

    安装结束后，AI库的头文件和静态库、动态库文件目录分别为“/usr/local/kdnn/include“和“/usr/local/kdnn/lib/threadpool“、“/usr/local/kdnn/lib/omp“。

    上述命令中涉及的**_xxxx_**代表版本号。

**安装后验证<a name="section193111321616"></a>**

**验证KDNN**

1. 执行**source**命令或重新登录终端让环境变量生效。

    ```bash
    source /etc/profile
    ```

2. 查看环境变量LD\_LIBRARY\_PATH是否包含KDNN动态库的安装路径“/usr/local/kdnn/lib/omp“。

    ```bash
    env | grep LD_LIBRARY_PATH
    ```

    如果变量包含安装路径，说明安装成功。

    安装成功后在安装路径（默认路径是“/usr/local/kdnn“）下生成相应文件，其中，include文件夹包含子库的头文件，lib文件夹包含了KDNN库的静态库、动态库文件。

**验证KDNN\_EXT**

1. 设置“PYTHONPATH“环境变量。
    - 使用单线程版本：

        ```bash
        export PYTHONPATH=/usr/local/kdnn/lib/extension/python39/single/:$PYTHONPATH
        ```

    - 使用多线程版本：

        ```bash
        export PYTHONPATH=/usr/local/kdnn/lib/extension/python39/omp/:$PYTHONPATH
        ```

2. 进入Python交互式命令界面，导入libkdnn\_ext算子包。

    ```bash
    python
    >>> import libkdnn_ext
    ```

    或

    ```bash
    >>> from libkdnn_ext import random_choice, softmax, get_version
    ```

    如果回显中没有报错信息，说明KDNN\_EXT已经安装成功。

### 卸载KDNN

若不再需要使用KDNN，可卸载KDNN。若操作过程中使用了RPM包管理工具支持但本文档中未说明的参数，可能会引入未定义行为，请谨慎操作。

1. 执行**rpm -e**命令卸载RPM安装包。

    ```bash
    rpm -e boostcore-kdnn
    ```

2. 确认安装目录“/usr/local/kdnn“被删除。
