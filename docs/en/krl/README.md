# Latest Updates

- [2025.12.30]: Added support for the Kunpeng 950 processors.
- [2025.09.30]: Added the Kunpeng Retrieval Library (KRL), an operator library optimized for the Kunpeng platform to accelerate vector retrieval.

## Introduction to KRL

Kunpeng Retrieval Library (KRL), provided by Huawei, is an operator library optimized for the Kunpeng platform to accelerate vector retrieval. This library optimizes the instruction set architecture and memory access mechanism of the Kunpeng processor at the hardware level. By combining low-precision quantization with high-precision re-ranking, the library significantly improves the computational efficiency and throughput of recall algorithms without compromising accuracy. These optimizations make it suitable for high-concurrency recall scenarios. KRL operators can be enabled to accelerate the open-source Faiss algorithms, such as HNSW, PQFS, IVFPQ, and IVFPQFS.

KRL applies to Kunpeng 920 and Kunpeng 950 processors, and supports NEON instructions (128-bit width) and SVE instructions (256-bit width).

## Version Description

For details about the feature updates of KRL, see [Release Notes](./release_notes.md).

## Related Documents

<a name="table1191773710200"></a>
<table><thead align="left"><tr id="row1291816372202"><th class="cellrowborder" valign="top" width="9.780978097809781%" id="mcps1.1.4.1.1"><p id="p291823714205"><a name="p291823714205"></a><a name="p291823714205"></a>Resource Type</p>
</th>
<th class="cellrowborder" valign="top" width="17.64176417641764%" id="mcps1.1.4.1.2"><p id="p13918183762016"><a name="p13918183762016"></a><a name="p13918183762016"></a>Resource Name</p>
</th>
Introduction to <th class="cellrowborder" valign="top" width="72.57725772577258%" id="mcps1.1.4.1.3"><p id="p89181437152019"><a name="p89181437152019"></a><a name="p89181437152019"></a>Resource Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row179181137112015"><td class="cellrowborder" valign="top" width="9.780978097809781%" headers="mcps1.1.4.1.1 "><p id="p1918123710208"><a name="p1918123710208"></a><a name="p1918123710208"></a>Document</p>
</td>
<td class="cellrowborder" valign="top" width="17.64176417641764%" headers="mcps1.1.4.1.2 "><p id="p2091893722011"><a name="p2091893722011"></a><a name="p2091893722011"></a><a href="./release_notes.md">Release Notes</a></p>
</td>
<td class="cellrowborder" valign="top" width="72.57725772577258%" headers="mcps1.1.4.1.3 "><p id="p491893752010"><a name="p491893752010"></a><a name="p491893752010"></a>Provides basic information and feature updates for each <span>KRL</span> version</p>
</td>
</tr>
<tr id="row939116371143"><td class="cellrowborder" valign="top" width="9.780978097809781%" headers="mcps1.1.4.1.1 "><p id="p1039163711413"><a name="p1039163711413"></a><a name="p1039163711413"></a>Document</p>
</td>
<td class="cellrowborder" valign="top" width="17.64176417641764%" headers="mcps1.1.4.1.2 "><p id="p03913372046"><a name="p03913372046"></a><a name="p03913372046"></a><a href="./quick_start.md"> Quick Start</a></p>
</td>
<td class="cellrowborder" valign="top" width="72.57725772577258%" headers="mcps1.1.4.1.3 "><p id="p1139217371746"><a name="p1139217371746"></a><a name="p1139217371746"></a>Provides guidance for getting started with <span>KRL</span>.</p>
</td>
</tr>
<tr id="row2918153732017"><td class="cellrowborder" valign="top" width="9.780978097809781%" headers="mcps1.1.4.1.1 "><p id="p598512211214"><a name="p598512211214"></a><a name="p598512211214"></a>Document</p>
</td>
<td class="cellrowborder" valign="top" width="17.64176417641764%" headers="mcps1.1.4.1.2 "><p id="p17918337172020"><a name="p17918337172020"></a><a name="p17918337172020"></a><a href="./installation_guide.md"> Installation Guide</a></p>
</td>
<td class="cellrowborder" valign="top" width="72.57725772577258%" headers="mcps1.1.4.1.3 "><p id="p15918183742018"><a name="p15918183742018"></a><a name="p15918183742018"></a>Provides guidance for compiling and installing <span>KRL</span>.</p>
</td>
</tr>
<tr id="row12311255193916"><td class="cellrowborder" valign="top" width="9.780978097809781%" headers="mcps1.1.4.1.1 "><p id="p1176012581392"><a name="p1176012581392"></a><a name="p1176012581392"></a>Document</p>
</td>
<td class="cellrowborder" valign="top" width="17.64176417641764%" headers="mcps1.1.4.1.2 "><p id="p13760358183920"><a name="p13760358183920"></a><a name="p13760358183920"></a><a href="./api_reference.md">API Reference</a></p>
</td>
<td class="cellrowborder" valign="top" width="72.57725772577258%" headers="mcps1.1.4.1.3 "><p id="p1776019584395"><a name="p1776019584395"></a><a name="p1776019584395"></a>Provides definitions and descriptions of <span>KRL</span> APIs.</p>
</td>
</tr>
</tbody>
</table>

## Disclaimer

This software is intended solely for debugging and development. You are responsible for any risks and should carefully review the following information:

+ Data processing and deletion: Users are responsible for managing and deleting any data generated while using this software. Users are advised to delete such data promptly after use to prevent information leakage.
+ Data confidentiality and transmission: Users understand and agree not to share or transmit any data generated by this software. Neither the software nor its developers are responsible for any information leaks, data breaches, or other negative consequences.
+ User input security: Users are responsible for the security of any commands they enter and for any risks or losses resulting from improper input. The software and its developers are not liable for issues caused by incorrect command usage.
+ Disclaimer scope: This disclaimer applies to all individuals and entities using this software. By using the software, you acknowledge and accept this statement and assume all risks and responsibilities arising from its use. If you do not agree, please stop using the software immediately.

Before using this software, please read and understand the preceding disclaimer. If you have any questions, contact the developer.

## License

KRL is licensed under the Apache 2.0 License, which allows modification and redistribution of derivative works as open source.

The documentation of this project is licensed under the CC BY 4.0 License.

## Contribution Statement

We welcome your contributions to the community. If you have any questions/suggestions or want to provide feedback on feature requirements and bug reports, you can [submit issues](https://gitcode.com/boostkit/community/blob/master/docs/contributor/issue-submit.md). For details, see the [contribution guideline](https://gitcode.com/boostkit/community/blob/master/docs/contributor/contributing.md). You are also welcome to share insights in the [Discussions](https://gitcode.com/boostkit/community/discussions). Thank you for your support.

## Acknowledgments

KRL is jointly developed by the following Huawei department:

- Kunpeng Computing BoostKit Development Dept

Thank you to everyone in the community for your PRs. We warmly welcome contributions to KRL!
