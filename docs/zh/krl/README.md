# KRL介绍

## 最新消息

- \[2025.12.30\]：新增适配鲲鹏950 7592C处理器。
- \[2025.09.30\]：新增基于鲲鹏平台优化的用于加速向量检索的算子库KRL。

## 项目介绍

鲲鹏检索算子库KRL（Kunpeng Retrieval Library）是华为提供的基于鲲鹏平台优化的用于加速向量检索的算子库。KRL针对鲲鹏处理器的指令集架构与内存访问机制进行底层优化，使用低精度量化+高精度重排等方法有效提升召回算法的计算效率与吞吐量，同时保证算法精度，适用于高并发召回场景的性能需求。目前可通过使能KRL算子的形式对开源Faiss的HNSW、PQFS、IVFPQ、IVFPQFS等算法进行加速。

KRL适用于鲲鹏920 7282C处理器与鲲鹏950 7592C处理器，支持NEON指令（128位宽）和SVE指令（256位宽）。

## 版本说明

关于KRL的版本更新情况请参见《[版本说明书](./release_notes.md)》。

## 学习文档

<a name="table1191773710200"></a>
<table><thead align="left"><tr id="row1291816372202"><th class="cellrowborder" valign="top" width="17.64176417641764%" id="mcps1.1.4.1.2"><p id="p13918183762016"><a name="p13918183762016"></a><a name="p13918183762016"></a>学习资源名称</p>
</th>
<th class="cellrowborder" valign="top" width="72.57725772577258%" id="mcps1.1.4.1.3"><p id="p89181437152019"><a name="p89181437152019"></a><a name="p89181437152019"></a>学习资源简介</p>
</th>
</tr>
</thead>
<tbody><tr id="row179181137112015"><td class="cellrowborder" valign="top" width="17.64176417641764%" headers="mcps1.1.4.1.2 "><p id="p2091893722011"><a name="p2091893722011"></a><a name="p2091893722011"></a><a href="./release_notes.md">版本说明书</a></p>
</td>
<td class="cellrowborder" valign="top" width="72.57725772577258%" headers="mcps1.1.4.1.3 "><p id="p491893752010"><a name="p491893752010"></a><a name="p491893752010"></a>提供<span>KRL</span>每个发布版本的基础信息和特性更新信息。</p>
</td>
</tr>
<tr id="row2918153732017"><td class="cellrowborder" valign="top" width="17.64176417641764%" headers="mcps1.1.4.1.2 "><p id="p17918337172020"><a name="p17918337172020"></a><a name="p17918337172020"></a><a href="./user_guide.md">用户指南</a></p>
</td>
<td class="cellrowborder" valign="top" width="72.57725772577258%" headers="mcps1.1.4.1.3 "><p id="p15918183742018"><a name="p15918183742018"></a><a name="p15918183742018"></a>提供<span>KRL</span>编译安装方法指导与使用示例。</p>
</td>
</tr>
<tr id="row12311255193916"><td class="cellrowborder" valign="top" width="17.64176417641764%" headers="mcps1.1.4.1.2 "><p id="p13760358183920"><a name="p13760358183920"></a><a name="p13760358183920"></a><a href="./api_reference.md">API参考</a></p>
</td>
<td class="cellrowborder" valign="top" width="72.57725772577258%" headers="mcps1.1.4.1.3 "><p id="p1776019584395"><a name="p1776019584395"></a><a name="p1776019584395"></a>提供<span>KRL</span>的API接口定义和接口说明。</p>
</td>
</tr>
</tbody>
</table>

## 免责声明

本软件仅供调试和开发之用，使用者需自行承担使用风险，并理解以下内容：

* 数据处理及删除：用户在使用本软件过程中产生的数据属于用户责任范畴。建议用户在使用完毕后及时删除相关数据，以防信息泄露。
* 数据保密与传播：使用者了解并同意不得将通过本软件产生的数据随意外发或传播。对于由此产生的信息泄露、数据泄露或其他不良后果，本软件及其开发者概不负责。
* 用户输入安全性：用户需自行保证输入的命令行的安全性，并承担因输入不当而导致的任何安全风险或损失。对于输入命令行不当所导致的问题，本软件及其开发者概不负责。
* 免责声明范围：本免责声明适用于所有使用本软件的个人或实体。使用本软件即表示您同意并接受本声明的内容，并愿意承担因使用该功能而产生的风险和责任，如有异议请停止使用本软件。

在使用本软件之前，请谨慎阅读并理解以上免责声明的内容。对于使用本软件所产生的任何问题或疑问，请及时联系开发者。

## License

KRL采用 Apache 2.0 License 许可证授权，支持修改代码和再开源。

本项目的文档适用CC-BY 4.0许可证。

## 贡献声明

欢迎大家为社区做贡献，如果使用过程中有任何问题/建议，或者需要反馈特性需求和bug报告，可以提交[Issues](https://gitcode.com/boostkit/community/blob/master/docs/contributor/issue-submit.md)联系我们，具体贡献方法可参考[这里](https://gitcode.com/boostkit/community/blob/master/docs/contributor/contributing.md)。同时也欢迎大家在[讨论专区](https://gitcode.com/boostkit/community/discussions)展开讨论交流。感谢您的支持。

## 致谢

KRL由华为公司的下列部门联合贡献：

- 鲲鹏计算Boostkit开发部

感谢来自社区的每一个PR，欢迎贡献KRL！
