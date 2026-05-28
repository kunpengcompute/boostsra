# Introduction to KBest

## Latest Updates

- [2025.12.30]: Added support for Kunpeng 950 processors.
- [2025.06.30]: Optimized the KBest algorithm performance. Added descriptions for the SetEarlyStoppingParams API, modified the Add API and KBest constructors.
- [2025.03.30]: Added the SaveGraph, LoadGraph, Serialize, Deserialize, BuildSearcher, GetNTotal, and GetDim APIs to the KBest library, and modified the Add, Save, and Load APIs. The KBest algorithm now supports integration with Milvus.
- [2024.12.30]: Added Kunpeng Blazing-fast embedding similarity search thruster (KBest), an efficient, proprietary graph-based search algorithm.

## Project Introduction

KBest is a proprietary, efficient graph-based search algorithm. It provides the search capability benchmarking against Faiss HNSW. In multi-dimensional vector Approximate Nearest Neighbor Search (ANNS), KBest employs methods such as quantization and NUMA scheduling to optimize the search performance and precision. It is applicable to network search, multi-modal search, recommendation systems, and retrieval-augmented generation (RAG).

## Feature Updates

For details about the feature updates of KBest, see [Release Notes](./release_notes.md).

## Related Documents

<table>
<thead align="left">
<tr id="row532024445820">
<th class="cellrowborder" valign="top" width="14.8014801480148%" id="mcps1.1.4.1.1"><p id="p10320944115815">Resource Type</p></th>
<th class="cellrowborder" valign="top" width="28.012801280128013%" id="mcps1.1.4.1.2"><p id="p14321184425814">Resource Name</p></th>
<th class="cellrowborder" valign="top" width="57.18571857185718%" id="mcps1.1.4.1.3"><p id="p1932112447589">Resource Description</p></th>
</tr>
</thead>
<tbody>
<tr id="row183211844195812">
<td class="cellrowborder" valign="top" width="14.8014801480148%" headers="mcps1.1.4.1.1"><p id="p77463013710">Document</p></td>
<td class="cellrowborder" valign="top" width="28.012801280128013%" headers="mcps1.1.4.1.2"><p id="p132119442580"><a href="./release_notes.md">Release Notes</a></p></td>
<td class="cellrowborder" valign="top" width="57.18571857185718%" headers="mcps1.1.4.1.3"><p id="p13321194412589">Provides basic information and feature updates for each KBest version.</p></td>
</tr>
<tr id="row18632162163420">
<td class="cellrowborder" valign="top" width="14.8014801480148%" headers="mcps1.1.4.1.1"><p id="p186331521183417">Document</p></td>
<td class="cellrowborder" valign="top" width="28.012801280128013%" headers="mcps1.1.4.1.2"><p id="p863317218347"><a href="./quick_start.md">Quick Start</a></p></td>
<td class="cellrowborder" valign="top" width="57.18571857185718%" headers="mcps1.1.4.1.3"><p id="p26331921183410">Provides a quick start guide for KBest.</p></td>
</tr>
<tr id="row6321164455815">
<td class="cellrowborder" valign="top" width="14.8014801480148%" headers="mcps1.1.4.1.1"><p id="p9991857717">Document</p></td>
<td class="cellrowborder" valign="top" width="28.012801280128013%" headers="mcps1.1.4.1.2"><p id="p14321104418585"><a href="./installation_guide.md">Installation Guide</a></p></td>
<td class="cellrowborder" valign="top" width="57.18571857185718%" headers="mcps1.1.4.1.3"><p id="p1332134420587">Provides detailed instructions for compiling and installing KBest.</p></td>
</tr>
<tr id="row13219448585">
<td class="cellrowborder" valign="top" width="14.8014801480148%" headers="mcps1.1.4.1.1"><p id="p131000513714">Document</p></td>
<td class="cellrowborder" valign="top" width="28.012801280128013%" headers="mcps1.1.4.1.2"><p id="p5321124418587"><a href="./best_practices.md">Best Practices</a></p></td>
<td class="cellrowborder" valign="top" width="57.18571857185718%" headers="mcps1.1.4.1.3"><p id="p232174455818">Provides practice cases of KBest.</p></td>
</tr>
<tr id="row1632118447589">
<td class="cellrowborder" valign="top" width="14.8014801480148%" headers="mcps1.1.4.1.1"><p id="p1510111511718">Document</p></td>
<td class="cellrowborder" valign="top" width="28.012801280128013%" headers="mcps1.1.4.1.2"><p id="p183213445582"><a href="./api_reference.md">API Reference</a></p></td>
<td class="cellrowborder" valign="top" width="57.18571857185718%" headers="mcps1.1.4.1.3"><p id="p53214445588">Provides definitions, descriptions, and calling examples of KBest APIs.</p></td>
</tr>
</tbody>
</table>

This project is implemented based on the methodology proposed in our KBest paper. If you use this project in academic research or other contexts, please cite our KBest paper.

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

## Disclaimer

This software is intended solely for debugging and development. You are responsible for any risks and should carefully review the following information:

- Data processing and deletion: Users are responsible for managing and deleting any data generated while using this software. Users are advised to delete such data promptly after use to prevent information leakage.
- Data confidentiality and transmission: Users understand and agree not to share or transmit any data generated by this software. Neither the software nor its developers are responsible for any information leaks, data breaches, or other negative consequences.
- User input security: Users are responsible for the security of any commands they enter and for any risks or losses resulting from improper input. The software and its developers are not liable for issues caused by incorrect command usage.
- Disclaimer scope: This disclaimer applies to all individuals and entities using this software. By using the software, you acknowledge and accept this statement and assume all risks and responsibilities arising from its use. If you do not agree, please stop using the software immediately.

Before using this software, please read and understand the preceding disclaimer. If you have any questions, contact the developer.

## License

KBest is licensed under the Apache 2.0 License, which allows modification and redistribution of derivative works as open source.

The documentation of this project is licensed under the CC BY 4.0 License.

## Contribution Statement

You are welcome to contribute to the community. If you have any questions/suggestions or want to provide feedback on feature requirements and bug reports, you can submit [issues](https://gitcode.com/boostkit/community/blob/master/docs/contributor/issue-submit.md). For details, see the [contribution guideline](https://gitcode.com/boostkit/community/blob/master/docs/contributor/contributing.md). You are also welcome to share insights in the [Discussions](https://gitcode.com/boostkit/community/discussions). Thank you for your support.

## Acknowledgments

KBest is jointly developed by the following Huawei department:

- Kunpeng Computing BoostKit Development Dept

Thank you to everyone in the community for your PRs. We warmly welcome contributions to KBest!
