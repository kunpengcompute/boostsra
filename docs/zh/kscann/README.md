# KScaNN介绍

## 最新消息

- \[2025.12.30\]：KScaNN新增鲲鹏950 7592C服务器兼容。
- \[2025.06.30\]：优化算法性能；新增对接Milvus使用。
- \[2024.12.30\]：新增基于鲲鹏架构深度优化索引布局和算法流程，鲲鹏亲和的自研算法体系KScaNN。

## 项目介绍

KScaNN（Kunpeng Scalable Nearest Neighbors）是基于倒排索引，结合鲲鹏架构深度优化索引布局、算法流程和计算流程，充分挖掘芯片潜力形成的向量检索算法。

KScaNN适用于鲲鹏920 7282C处理器与鲲鹏950 7592C处理器，支持NEON指令（128位宽）和SVE指令（256位宽）。

## 版本说明

关于KScaNN的版本更新情况请参见[《版本说明书》](./release_notes.md)。

## 学习文档

<table>
<thead align="left">
<tr id="row1291816372202">
<th class="cellrowborder" valign="top" width="9.780978097809781%" id="mcps1.1.4.1.1"><p id="p291823714205">学习资源类别</p></th>
<th class="cellrowborder" valign="top" width="17.64176417641764%" id="mcps1.1.4.1.2"><p id="p13918183762016">学习资源名称</p></th>
<th class="cellrowborder" valign="top" width="72.57725772577258%" id="mcps1.1.4.1.3"><p id="p89181437152019">学习资源简介</p></th>
</tr>
</thead>
<tbody>
<tr id="row179181137112015">
<td class="cellrowborder" valign="top" width="9.780978097809781%" headers="mcps1.1.4.1.1"><p id="p1918123710208">文档</p></td>
<td class="cellrowborder" valign="top" width="17.64176417641764%" headers="mcps1.1.4.1.2"><p id="p2091893722011"><a href="./release_notes.md">版本说明书</a></p></td>
<td class="cellrowborder" valign="top" width="72.57725772577258%" headers="mcps1.1.4.1.3"><p id="p491893752010">提供KScaNN每个发布版本的基础信息和特性更新信息。</p></td>
</tr>
<tr id="row939116371143">
<td class="cellrowborder" valign="top" width="9.780978097809781%" headers="mcps1.1.4.1.1"><p id="p1039163711413">文档</p></td>
<td class="cellrowborder" valign="top" width="17.64176417641764%" headers="mcps1.1.4.1.2"><p id="p03913372046"><a href="./quick_start.md">快速入门</a></p></td>
<td class="cellrowborder" valign="top" width="72.57725772577258%" headers="mcps1.1.4.1.3"><p id="p1139217371746">提供KScaNN快速入门指导。</p></td>
</tr>
<tr id="row2918153732017">
<td class="cellrowborder" valign="top" width="9.780978097809781%" headers="mcps1.1.4.1.1"><p id="p598512211214">文档</p></td>
<td class="cellrowborder" valign="top" width="17.64176417641764%" headers="mcps1.1.4.1.2"><p id="p17918337172020"><a href="./installation_guide.md">安装指南</a></p></td>
<td class="cellrowborder" valign="top" width="72.57725772577258%" headers="mcps1.1.4.1.3"><p id="p15918183742018">提供KScaNN编译安装方法指导。</p></td>
</tr>
<tr id="row10576182811217">
<td class="cellrowborder" valign="top" width="9.780978097809781%" headers="mcps1.1.4.1.1"><p id="p25773281625">文档</p></td>
<td class="cellrowborder" valign="top" width="17.64176417641764%" headers="mcps1.1.4.1.2"><p id="p55779281524"><a href="./best_practices.md">最佳实践</a></p></td>
<td class="cellrowborder" valign="top" width="72.57725772577258%" headers="mcps1.1.4.1.3"><p id="p1657712287211">提供KScaNN的使用实践案例。</p></td>
</tr>
<tr id="row12311255193916">
<td class="cellrowborder" valign="top" width="9.780978097809781%" headers="mcps1.1.4.1.1"><p id="p1176012581392">文档</p></td>
<td class="cellrowborder" valign="top" width="17.64176417641764%" headers="mcps1.1.4.1.2"><p id="p13760358183920"><a href="./api_reference.md">API参考</a></p></td>
<td class="cellrowborder" valign="top" width="72.57725772577258%" headers="mcps1.1.4.1.3"><p id="p1776019584395">提供KScaNN的API接口定义和接口说明。</p></td>
</tr>
<tr id="row92097207RU01">
<td class="cellrowborder" valign="top" width="9.780978097809781%" headers="mcps1.1.4.1.1"><p id="p92097207RU01a">专利</p></td>
<td class="cellrowborder" valign="top" width="17.64176417641764%" headers="mcps1.1.4.1.2"><p id="p92097207RU01b">一种自适应感知分桶优化的向量检索装置</p></td>
<td class="cellrowborder" valign="top" width="72.57725772577258%" headers="mcps1.1.4.1.3"><p id="p92097207RU01c">Patent Ref：92097207RU01<br>Application No.：RU2025123028</p></td>
</tr>
</tbody>
</table>

## 免责声明

此代码仓计划参与GoogleResearch社区开源，仅作用于向量检索加速，编码风格遵照原生开源软件，继承原生开源软件安全设计，不破坏原生开源软件设计及编码风格和方式，软件的任何漏洞与安全问题，均由相应的上游社区根据其漏洞和安全响应机制解决。请密切关注上游社区发布的通知和版本更新。鲲鹏计算社区对软件的漏洞及安全问题不承担任何责任。

## License

KScaNN采用 Apache 2.0 License 许可证授权，支持修改代码和再开源。

本项目的文档适用CC-BY 4.0许可证。

## 贡献声明

欢迎大家为社区做贡献，如果使用过程中有任何问题/建议，或者需要反馈特性需求和bug报告，可以提交[Issues](https://gitcode.com/boostkit/community/blob/master/docs/contributor/issue-submit.md)联系我们，具体贡献方法可参考[这里](https://gitcode.com/boostkit/community/blob/master/docs/contributor/contributing.md)。同时也欢迎大家在[讨论专区](https://gitcode.com/boostkit/community/discussions)展开讨论交流。感谢您的支持。

## 致谢

KScaNN由华为公司的下列部门联合贡献：

- 鲲鹏计算Boostkit开发部

感谢来自社区的每一个PR，欢迎贡献KScaNN！
