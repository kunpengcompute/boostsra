# KBest介绍

## 最新消息

- \[2025.12.30\]：KBest新增鲲鹏950 7592C处理器兼容。
- \[2025.06.30\]：KBest算法性能优化，新增SetEarlyStoppingParams接口，Add接口和构造函数KBest。
- \[2025.03.30\]：KBest新增SaveGraph/LoadGraph接口、Serialize/Deserialize接口、BuildSearcher及GetNTotal和GetDim接口，并且修改Add、Save和Load接口，目前已对接Milvus使用。
- \[2024.12.30\]：新增鲲鹏自研的高效的图检索算法KBest（Kunpeng Blazing-fast embedding similarity search thruster）。

## 项目介绍

KBest（Kunpeng Blazing-fast embedding similarity search thruster）鲲鹏召回图检索算法，是鲲鹏自研的高效的图检索算法，提供对标开源Faiss HNSW算法的检索能力。通过量化、NUMA访存调度等方法优化了最近邻搜索的性能和精度，用于多维向量近似最近邻搜索，适用于网络搜索、多模态搜索、推荐系统和RAG等场景。

## 版本说明

关于KBest算法的版本更新情况请参见《[版本说明书](./release_notes.md)》。

## 学习文档

<table>
<thead align="left">
<tr id="row532024445820">
<th class="cellrowborder" valign="top" width="28.012801280128013%" id="mcps1.1.4.1.2"><p id="p14321184425814">学习资源名称</p></th>
<th class="cellrowborder" valign="top" width="57.18571857185718%" id="mcps1.1.4.1.3"><p id="p1932112447589">学习资源简介</p></th>
</tr>
</thead>
<tbody>
<tr id="row183211844195812">
<td class="cellrowborder" valign="top" width="28.012801280128013%" headers="mcps1.1.4.1.2"><p id="p132119442580"><a href="./release_notes.md">版本说明书</a></p></td>
<td class="cellrowborder" valign="top" width="57.18571857185718%" headers="mcps1.1.4.1.3"><p id="p13321194412589">提供KBest每个发布版本的基础信息和特性更新信息。</p></td>
</tr>
<tr id="row18632162163420">
<td class="cellrowborder" valign="top" width="28.012801280128013%" headers="mcps1.1.4.1.2"><p id="p863317218347"><a href="./quick_start.md">快速入门</a></p></td>
<td class="cellrowborder" valign="top" width="57.18571857185718%" headers="mcps1.1.4.1.3"><p id="p26331921183410">提供KBest快速上手使用指导。</p></td>
</tr>
<tr id="row6321164455815">
<td class="cellrowborder" valign="top" width="28.012801280128013%" headers="mcps1.1.4.1.2"><p id="p14321104418585"><a href="./installation_guide.md">安装指南</a></p></td>
<td class="cellrowborder" valign="top" width="57.18571857185718%" headers="mcps1.1.4.1.3"><p id="p1332134420587">提供KBest编译安装的详细指导。</p></td>
</tr>
<tr id="row13219448585">
<td class="cellrowborder" valign="top" width="28.012801280128013%" headers="mcps1.1.4.1.2"><p id="p5321124418587"><a href="./best_practices.md">最佳实践</a></p></td>
<td class="cellrowborder" valign="top" width="57.18571857185718%" headers="mcps1.1.4.1.3"><p id="p232174455818">提供KBest使用的实践案例。</p></td>
</tr>
<tr id="row1632118447589">
<td class="cellrowborder" valign="top" width="28.012801280128013%" headers="mcps1.1.4.1.2"><p id="p183213445582"><a href="./api_reference.md">API参考</a></p></td>
<td class="cellrowborder" valign="top" width="57.18571857185718%" headers="mcps1.1.4.1.3"><p id="p53214445588">提供KBest提供的API接口定义、接口说明、接口调用示例等。</p></td>
</tr>
</tbody>
</table>

本项目基于我们在KBest论文中提出的方法实现，如果您在学术研究或其他方面使用本项目，请引用我们的KBest论文：

```text
@misc{ma2025kbestefficientvectorsearch,
      title={KBest: Efficient Vector Search on Kunpeng CPU}, 
      author={Kaihao MA and Meiling Wang and Senkevich Oleg and Zijian LI and Daihao Xue and Dmitriy Malyshev and Yangming Lv and Shihai Xiao and Xiao Yan and Radionov Alexander and Weidi Zeng and Yuanzhan Gao and Zhiyu Zou and Yao xin and Liu Lin and Junhao Wu and Yiding Liu and Yaoyao Fu and Gongyi Wang and Gong Zhang and Fei Yi and Yingfan Liu},
      year={2025},
      eprint={2508.03016},
      archivePrefix={arXiv},
      primaryClass={cs.IR},
      url={https://arxiv.org/abs/2508.03016}, 
}
```

## 免责声明

本软件仅供调试和开发之用，使用者需自行承担使用风险，并理解以下内容：

+ 数据处理及删除：用户在使用本软件过程中产生的数据属于用户责任范畴。建议用户在使用完毕后及时删除相关数据，以防信息泄露。
+ 数据保密与传播：使用者了解并同意不得将通过本软件产生的数据随意外发或传播。对于由此产生的信息泄露、数据泄露或其他不良后果，本软件及其开发者概不负责。
+ 用户输入安全性：用户需自行保证输入的命令行的安全性，并承担因输入不当而导致的任何安全风险或损失。对于输入命令行不当所导致的问题，本软件及其开发者概不负责。
+ 免责声明范围：本免责声明适用于所有使用本软件的个人或实体。使用本软件即表示您同意并接受本声明的内容，并愿意承担因使用该功能而产生的风险和责任，如有异议请停止使用本软件。

在使用本软件之前，请谨慎阅读并理解以上免责声明的内容。对于使用本软件所产生的任何问题或疑问，请及时联系开发者。

## License

KBest采用Apache 2.0 License许可证授权，支持修改代码和再开源。

本项目的文档适用CC-BY 4.0许可证。

## 贡献声明

欢迎大家为社区做贡献，如果使用过程中有任何问题/建议，或者需要反馈特性需求和bug报告，可以提交[Issues](https://gitcode.com/boostkit/community/blob/master/docs/contributor/issue-submit.md)联系我们，具体贡献方法可参考[这里](https://gitcode.com/boostkit/community/blob/master/docs/contributor/contributing.md)。同时也欢迎大家在[讨论专区](https://gitcode.com/boostkit/community/discussions)展开讨论交流。感谢您的支持。

## 致谢

感谢来自社区的每一个PR，欢迎贡献KBest！
