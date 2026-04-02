# KDNN介绍

## 最新消息

- \[2026.03.30\]：KDNN新增基于MMLA指令的s8/u8数据类型MatMul实现；支持Post-ops（后处理操作）；支持FusedMatMul融合算子。
- \[2025.12.30\]：KDNN新增MatMul的NEON实现，新增支持MatMul的自定义线程池模式，新增Group Normalization、SparseGemm深度神经网络算子的鲲鹏平台支持。
- \[2025.06.30\]：KDNN新增Pool、Batch Normalization、Local Response Normalization、Reduction、PReLU、Binary、RNN深度神经网络算子的鲲鹏平台支持。新增支持鲲鹏920新型号处理器。
- \[2024.12.30\]：KDNN新增reorder、resampling、concat、shuffle 4个深度神经网络算子的鲲鹏平台支持。

## 项目介绍

KDNN（Kunpeng Deep Neural Network Library）是华为提供的基于鲲鹏平台优化的高性能神经网络算子库，包含KDNN和KDNN\_EXT（Kunpeng Deep Neural Network Extension Library，鲲鹏深度神经网络算子扩展库），主要由C/C++、汇编语言实现。KDNN\_EXT扩展算子包括softmax、random\_choice等。KDNN的组成如[表1](#table113613052017)所示。

**表 1**  KDNN组成部分

<a name="table113613052017"></a>
<table><thead align="left"><tr id="row237018052015"><th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.1"><p id="p13701307204"><a name="p13701307204"></a><a name="p13701307204"></a>序号</p>
</th>
<th class="cellrowborder" valign="top" width="13.83%" id="mcps1.2.5.1.2"><p id="p10370130112016"><a name="p10370130112016"></a><a name="p10370130112016"></a>库名</p>
</th>
<th class="cellrowborder" valign="top" width="44.11%" id="mcps1.2.5.1.3"><p id="p173704019205"><a name="p173704019205"></a><a name="p173704019205"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="36.059999999999995%" id="mcps1.2.5.1.4"><p id="p737019032019"><a name="p737019032019"></a><a name="p737019032019"></a>适用场景</p>
</th>
</tr>
</thead>
<tbody><tr id="row737011016208"><td class="cellrowborder" valign="top" width="6%" headers="mcps1.2.5.1.1 "><p id="p7370107203"><a name="p7370107203"></a><a name="p7370107203"></a>1</p>
</td>
<td class="cellrowborder" valign="top" width="13.83%" headers="mcps1.2.5.1.2 "><p id="p1237011013202"><a name="p1237011013202"></a><a name="p1237011013202"></a>KDNN</p>
</td>
<td class="cellrowborder" valign="top" width="44.11%" headers="mcps1.2.5.1.3 "><p id="p193701909209"><a name="p193701909209"></a><a name="p193701909209"></a>深度神经网络算子库结合鲲鹏处理器微架构特性与软优化手段，优化AI算子性能。该算子库以插件形式集成至开源软件oneDNN。</p>
</td>
<td class="cellrowborder" valign="top" width="36.059999999999995%" headers="mcps1.2.5.1.4 "><p id="p153707032017"><a name="p153707032017"></a><a name="p153707032017"></a>适用于各种机器学习应用，包括图像分类、目标检测、语音识别等，并可以与各种深度学习框架集成，如TensorFlow、PyTorch等。</p>
</td>
</tr>
<tr id="row163701804202"><td class="cellrowborder" valign="top" width="6%" headers="mcps1.2.5.1.1 "><p id="p173701403204"><a name="p173701403204"></a><a name="p173701403204"></a>2</p>
</td>
<td class="cellrowborder" valign="top" width="13.83%" headers="mcps1.2.5.1.2 "><p id="p163704072014"><a name="p163704072014"></a><a name="p163704072014"></a>KDNN_EXT</p>
</td>
<td class="cellrowborder" valign="top" width="44.11%" headers="mcps1.2.5.1.3 "><p id="p73701209208"><a name="p73701209208"></a><a name="p73701209208"></a>深度神经网络算子扩展库，深度优化softmax、random_choice等算子，封装为Python语言接口提供给用户调用。</p>
</td>
<td class="cellrowborder" valign="top" width="36.059999999999995%" headers="mcps1.2.5.1.4 "><p id="p1237015014202"><a name="p1237015014202"></a><a name="p1237015014202"></a>适用于多分类任务、随机选择等场景，并可以与各种深度学习框架集成，如TensorFlow、PyTorch等。</p>
</td>
</tr>
</tbody>
</table>

KDNN仅适用于鲲鹏系列处理器。

为获得最优性能，KDNN接口内部不做完整入参校验，入参合法性由调用方业务来保证。

**应用场景<a name="section1957994882217"></a>**

KDNN主要在以下场景中使用：

- 深度学习加速：图像分类、目标检测和分割、自然语言处理、推荐系统
- HPC：气象、生命科学、制造、教育科研
- 大数据：机器学习算法

## 版本说明

关于KDNN的版本更新情况请参见《<a href="release_notes.md">版本说明书</a>》。

## 兼容性信息

为保证您可以顺利安全地使用KDNN，请确保所使用的环境信息在已验证环境范围内。

**表 1**  KDNN已验证环境

<a name="table7471331132318"></a>
<table><thead align="left"><tr id="row757143152315"><th class="cellrowborder" valign="top" width="12.15%" id="mcps1.2.7.1.1"><p id="p457831192313"><a name="p457831192313"></a><a name="p457831192313"></a>组件</p>
</th>
<th class="cellrowborder" valign="top" width="19.97%" id="mcps1.2.7.1.2"><p id="p5571831182318"><a name="p5571831182318"></a><a name="p5571831182318"></a>操作系统</p>
</th>
<th class="cellrowborder" valign="top" width="22.32%" id="mcps1.2.7.1.3"><p id="p55733113238"><a name="p55733113238"></a><a name="p55733113238"></a>CPU类型</p>
</th>
<th class="cellrowborder" valign="top" width="18.94%" id="mcps1.2.7.1.4"><p id="p35713152318"><a name="p35713152318"></a><a name="p35713152318"></a>编译器</p>
</th>
<th class="cellrowborder" valign="top" width="11.07%" id="mcps1.2.7.1.5"><p id="p135718319231"><a name="p135718319231"></a><a name="p135718319231"></a>构建工具</p>
</th>
<th class="cellrowborder" valign="top" width="15.55%" id="mcps1.2.7.1.6"><p id="p657153142317"><a name="p657153142317"></a><a name="p657153142317"></a>Python解释器</p>
</th>
</tr>
</thead>
<tbody><tr id="row165716316236"><td class="cellrowborder" valign="top" width="12.15%" headers="mcps1.2.7.1.1 "><p id="p4571531192317"><a name="p4571531192317"></a><a name="p4571531192317"></a>KDNN</p>
</td>
<td class="cellrowborder" valign="top" width="19.97%" headers="mcps1.2.7.1.2 "><p id="p45713315237"><a name="p45713315237"></a><a name="p45713315237"></a>openEuler 22.03 LTS SP3</p>
</td>
<td class="cellrowborder" valign="top" width="22.32%" headers="mcps1.2.7.1.3 "><p id="p2057631172312"><a name="p2057631172312"></a><a name="p2057631172312"></a>华为鲲鹏920 7270Z/7280Z处理器</p>
</td>
<td class="cellrowborder" valign="top" width="18.94%" headers="mcps1.2.7.1.4 "><p id="p115753102316"><a name="p115753102316"></a><a name="p115753102316"></a>GCC 10.3.1</p>
</td>
<td class="cellrowborder" valign="top" width="11.07%" headers="mcps1.2.7.1.5 "><p id="p14571131142319"><a name="p14571131142319"></a><a name="p14571131142319"></a>CMake 3.22.0</p>
</td>
<td class="cellrowborder" valign="top" width="15.55%" headers="mcps1.2.7.1.6 "><p id="p3571531102318"><a name="p3571531102318"></a><a name="p3571531102318"></a>Python 3.9.21</p>
</td>
</tr>
<tr id="row157193172311"><td class="cellrowborder" valign="top" width="12.15%" headers="mcps1.2.7.1.1 "><p id="p127798522236"><a name="p127798522236"></a><a name="p127798522236"></a>KDNN</p>
</td>
<td class="cellrowborder" valign="top" width="19.97%" headers="mcps1.2.7.1.2 "><p id="p155719317232"><a name="p155719317232"></a><a name="p155719317232"></a>openEuler 22.03 LTS SP4</p>
<p id="p105793172319"><a name="p105793172319"></a><a name="p105793172319"></a>内核版本高于5.10.0-228.0.0.127</p>
</td>
<td class="cellrowborder" valign="top" width="22.32%" headers="mcps1.2.7.1.3 "><p id="p65733172315"><a name="p65733172315"></a><a name="p65733172315"></a>华为鲲鹏920新型号处理器</p>
</td>
<td class="cellrowborder" valign="top" width="18.94%" headers="mcps1.2.7.1.4 "><p id="p1757183162316"><a name="p1757183162316"></a><a name="p1757183162316"></a>GCC 12.3.1/毕昇 4.2.0</p>
</td>
<td class="cellrowborder" valign="top" width="11.07%" headers="mcps1.2.7.1.5 "><p id="p75743122317"><a name="p75743122317"></a><a name="p75743122317"></a>CMake 3.22.0</p>
</td>
<td class="cellrowborder" valign="top" width="15.55%" headers="mcps1.2.7.1.6 "><p id="p55720316236"><a name="p55720316236"></a><a name="p55720316236"></a>Python 3.9.21</p>
</td>
</tr>
<tr id="row1457531142317"><td class="cellrowborder" valign="top" width="12.15%" headers="mcps1.2.7.1.1 "><p id="p3571631172311"><a name="p3571631172311"></a><a name="p3571631172311"></a>KDNN_EXT</p>
</td>
<td class="cellrowborder" valign="top" width="19.97%" headers="mcps1.2.7.1.2 "><p id="p45714313232"><a name="p45714313232"></a><a name="p45714313232"></a>openEuler 22.03 LTS SP3</p>
</td>
<td class="cellrowborder" valign="top" width="22.32%" headers="mcps1.2.7.1.3 "><p id="p7571931162318"><a name="p7571931162318"></a><a name="p7571931162318"></a>华为鲲鹏920系列处理器</p>
</td>
<td class="cellrowborder" valign="top" width="18.94%" headers="mcps1.2.7.1.4 "><p id="p1379182902417"><a name="p1379182902417"></a><a name="p1379182902417"></a>GCC 10.3.1</p>
</td>
<td class="cellrowborder" valign="top" width="11.07%" headers="mcps1.2.7.1.5 "><p id="p1479132912419"><a name="p1479132912419"></a><a name="p1479132912419"></a>CMake 3.22.0</p>
</td>
<td class="cellrowborder" valign="top" width="15.55%" headers="mcps1.2.7.1.6 "><p id="p879162942416"><a name="p879162942416"></a><a name="p879162942416"></a>Python 3.9.21</p>
</td>
</tr>
</tbody>
</table>

## 学习文档

<a name="table11320174415582"></a>
<table><thead align="left"><tr id="row532024445820"><th class="cellrowborder" valign="top" width="14.8014801480148%" id="mcps1.1.4.1.1"><p id="p10320944115815"><a name="p10320944115815"></a><a name="p10320944115815"></a>学习资源类别</p>
</th>
<th class="cellrowborder" valign="top" width="28.012801280128013%" id="mcps1.1.4.1.2"><p id="p14321184425814"><a name="p14321184425814"></a><a name="p14321184425814"></a>学习资源名称</p>
</th>
<th class="cellrowborder" valign="top" width="57.18571857185718%" id="mcps1.1.4.1.3"><p id="p1932112447589"><a name="p1932112447589"></a><a name="p1932112447589"></a>学习资源简介</p>
</th>
</tr>
</thead>
<tbody><tr id="row183211844195812"><td class="cellrowborder" valign="top" width="14.8014801480148%" headers="mcps1.1.4.1.1 "><p id="p77463013710"><a name="p77463013710"></a><a name="p77463013710"></a>文档</p>
</td>
<td class="cellrowborder" valign="top" width="28.012801280128013%" headers="mcps1.1.4.1.2 "><p id="p132119442580"><a name="p132119442580"></a><a name="p132119442580"></a><a href="release_notes.md">版本说明书</a></p>
</td>
<td class="cellrowborder" valign="top" width="57.18571857185718%" headers="mcps1.1.4.1.3 "><p id="p13321194412589"><a name="p13321194412589"></a><a name="p13321194412589"></a>提供KDNN每个发布版本的基础信息和特性更新信息。</p>
</td>
</tr>
<tr id="row4533125512117"><td class="cellrowborder" valign="top" width="14.8014801480148%" headers="mcps1.1.4.1.1 "><p id="p19321184415819"><a name="p19321184415819"></a><a name="p19321184415819"></a>文档</p>
</td>
<td class="cellrowborder" valign="top" width="28.012801280128013%" headers="mcps1.1.4.1.2 "><p id="p032144418580"><a name="p032144418580"></a><a name="p032144418580"></a><a href="quick_start.md">快速入门</a></p>
</td>
<td class="cellrowborder" valign="top" width="57.18571857185718%" headers="mcps1.1.4.1.3 "><p id="p83216449586"><a name="p83216449586"></a><a name="p83216449586"></a>提供KDNN快速入门指导。</p>
</td>
</tr>
<tr id="row6321164455815"><td class="cellrowborder" valign="top" width="14.8014801480148%" headers="mcps1.1.4.1.1 "><p id="p9991857717"><a name="p9991857717"></a><a name="p9991857717"></a>文档</p>
</td>
<td class="cellrowborder" valign="top" width="28.012801280128013%" headers="mcps1.1.4.1.2 "><p id="p14321104418585"><a name="p14321104418585"></a><a name="p14321104418585"></a><a href="installation_guide.md">安装指南</a></p>
</td>
<td class="cellrowborder" valign="top" width="57.18571857185718%" headers="mcps1.1.4.1.3 "><p id="p1332134420587"><a name="p1332134420587"></a><a name="p1332134420587"></a>提供KDNN编译安装的详细指导。</p>
</td>
</tr>
<tr id="row13219448585"><td class="cellrowborder" valign="top" width="14.8014801480148%" headers="mcps1.1.4.1.1 "><p id="p131000513714"><a name="p131000513714"></a><a name="p131000513714"></a>文档</p>
</td>
<td class="cellrowborder" valign="top" width="28.012801280128013%" headers="mcps1.1.4.1.2 "><p id="p5321124418587"><a name="p5321124418587"></a><a name="p5321124418587"></a><a href="api_reference.md">API参考</a></p>
</td>
<td class="cellrowborder" valign="top" width="57.18571857185718%" headers="mcps1.1.4.1.3 "><p id="p53214445588"><a name="p53214445588"></a><a name="p53214445588"></a>提供KDNN提供的API接口定义、接口说明、接口调用示例等。</p>
</td>
</tr>
<tr id="row1632118447589"><td class="cellrowborder" valign="top" width="14.8014801480148%" headers="mcps1.1.4.1.1 "><p id="p1510111511718"><a name="p1510111511718"></a><a name="p1510111511718"></a>文档</p>
</td>
<td class="cellrowborder" valign="top" width="28.012801280128013%" headers="mcps1.1.4.1.2 "><p id="p183213445582"><a name="p183213445582"></a><a name="p183213445582"></a><a href="best_practices.md">最佳实践</a></p>
</td>
<td class="cellrowborder" valign="top" width="57.18571857185718%" headers="mcps1.1.4.1.3 "><p id="p232174455818"><a name="p232174455818"></a><a name="p232174455818"></a>提供KDNN使用的实践案例。</p>
</td>
</tr>
</tbody>
</table>

## 免责声明

**致本项目使用者**

- 本项目仅供调试和开发之用，使用者需自行承担使用风险，并理解以下内容：
    - 数据处理及删除：用户在使用本工具过程中产生的数据属于用户责任范畴。建议用户在使用完毕后及时删除相关数据，以防信息泄露。
    - 数据保密与传播：使用者了解并同意不得将通过本工具产生的数据随意外发或传播。对于由此产生的信息泄露、数据泄露或其他不良后果，本工具及其开发者概不负责。
    - 用户输入安全性：用户需自行保证输入的命令行的安全性，并承担因输入不当而导致的任何安全风险或损失。对于输入命令行不当所导致的问题，本工具及其开发者概不负责。

- 免责声明范围：本免责声明适用于所有使用本工具的个人或实体。使用本工具即表示您同意并接受本声明的内容，并愿意承担因使用该功能而产生的风险和责任，如有异议请停止使用本工具。
- 在使用本工具之前，请**谨慎阅读并理解以上免责声明的内容**。对于使用本工具所产生的任何问题或疑问，请及时联系开发者。

**致数据所有者**

如果您不希望您的模型或数据集等信息在本项目中被提及，或希望更新本项目有关的描述，请在GitCode提交issue，我们将根据您的issue要求删除或更新您相关描述。衷心感谢您对本项目的理解和贡献。

## License

本项目的文档适用CC-BY 4.0许可证，具体请参见[LICENSE](LICENSE)文件。 

## 贡献声明

欢迎大家为社区做贡献，如果使用过程中有任何问题/建议，或者需要反馈特性需求和bug报告，可以提交[Issues](https://gitcode.com/boostkit/community/blob/master/docs/contributor/issue-submit.md)联系我们，具体贡献方法可参考[这里](https://gitcode.com/boostkit/community/blob/master/docs/contributor/contributing.md)。同时也欢迎大家在[讨论专区](https://gitcode.com/boostkit/community/discussions)展开讨论交流。感谢您的支持。

## 致谢

KDNN由华为公司的下列部门联合贡献：

- 鲲鹏计算Boostkit开发部

感谢来自社区的每一个PR，欢迎贡献KDNN！
