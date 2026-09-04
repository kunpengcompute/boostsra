# Introduction to KScaNN

## Latest Updates

- [2025.12.30]: Added support for Kunpeng 950 processors.
- [2025.06.30]: Optimized algorithm performance, and added the implementation for connecting KScaNN to Milvus.
- [2024.12.30]: Added KScaNN, a proprietary algorithm with Kunpeng affinity, which optimizes the index layout and algorithm process based on the Kunpeng architecture.

## Overview

Kunpeng Scalable Nearest Neighbors (KScaNN) is an inverted index-based vector retrieval algorithm that deeply optimizes index layout, algorithmic logic, and computing process to fully unlock the chip potential.

KScaNN applies to Kunpeng 920 and Kunpeng 950 processors, and supports NEON instructions (128-bit width) and SVE instructions (256-bit width).

## Release Notes

For details about the feature updates of KScaNN, see [Release Notes](./release_notes.md).

## Related Documents

<table>
<thead align="left">
<tr id="row1291816372202">
<th class="cellrowborder" valign="top" width="9.780978097809781%" id="mcps1.1.4.1.1"><p id="p291823714205">Resource Type</p></th>
<th class="cellrowborder" valign="top" width="17.64176417641764%" id="mcps1.1.4.1.2"><p id="p13918183762016">Resource Name</p></th>
<th class="cellrowborder" valign="top" width="72.57725772577258%" id="mcps1.1.4.1.3"><p id="p89181437152019">Resource Description</p></th>
</tr>
</thead>
<tbody>
<tr id="row179181137112015">
<td class="cellrowborder" valign="top" width="9.780978097809781%" headers="mcps1.1.4.1.1"><p id="p1918123710208">Document</p></td>
<td class="cellrowborder" valign="top" width="17.64176417641764%" headers="mcps1.1.4.1.2"><p id="p2091893722011"><a href="./release_notes.md">Release Notes</a></p></td>
<td class="cellrowborder" valign="top" width="72.57725772577258%" headers="mcps1.1.4.1.3"><p id="p491893752010">Provides basic information and feature updates for each KScaNN version.</p></td>
</tr>
<tr id="row939116371143">
<td class="cellrowborder" valign="top" width="9.780978097809781%" headers="mcps1.1.4.1.1"><p id="p1039163711413">Document</p></td>
<td class="cellrowborder" valign="top" width="17.64176417641764%" headers="mcps1.1.4.1.2"><p id="p03913372046"><a href="./quick_start.md">Quick Start</a></p></td>
<td class="cellrowborder" valign="top" width="72.57725772577258%" headers="mcps1.1.4.1.3"><p id="p1139217371746">Provides guidance for getting started with KScaNN.</p></td>
</tr>
<tr id="row2918153732017">
<td class="cellrowborder" valign="top" width="9.780978097809781%" headers="mcps1.1.4.1.1"><p id="p598512211214">Document</p></td>
<td class="cellrowborder" valign="top" width="17.64176417641764%" headers="mcps1.1.4.1.2"><p id="p17918337172020"><a href="./installation_guide.md">Installation Guide</a></p></td>
<td class="cellrowborder" valign="top" width="72.57725772577258%" headers="mcps1.1.4.1.3"><p id="p15918183742018">Provides guidance for compiling and installing KScaNN.</p></td>
</tr>
<tr id="row10576182811217">
<td class="cellrowborder" valign="top" width="9.780978097809781%" headers="mcps1.1.4.1.1"><p id="p25773281625">Document</p></td>
<td class="cellrowborder" valign="top" width="17.64176417641764%" headers="mcps1.1.4.1.2"><p id="p55779281524"><a href="./best_practices.md">Best Practices</a></p></td>
<td class="cellrowborder" valign="top" width="72.57725772577258%" headers="mcps1.1.4.1.3"><p id="p1657712287211">Provides best practices of using KScaNN.</p></td>
</tr>
<tr id="row12311255193916">
<td class="cellrowborder" valign="top" width="9.780978097809781%" headers="mcps1.1.4.1.1"><p id="p1176012581392">Document</p></td>
<td class="cellrowborder" valign="top" width="17.64176417641764%" headers="mcps1.1.4.1.2"><p id="p13760358183920"><a href="./api_reference.md">API Reference</a></p></td>
<td class="cellrowborder" valign="top" width="72.57725772577258%" headers="mcps1.1.4.1.3"><p id="p1776019584395">Provides definitions and descriptions of KScaNN APIs.</p></td>
</tr>
<tr id="row92097207RU01">
<td class="cellrowborder" valign="top" width="9.780978097809781%" headers="mcps1.1.4.1.1"><p id="p92097207RU01a">Patent</p></td>
<td class="cellrowborder" valign="top" width="17.64176417641764%" headers="mcps1.1.4.1.2"><p id="p92097207RU01b">Apparatus for Vector Retrieval via Adaptive Perception-Based Bucketing Optimization</p></td>
<td class="cellrowborder" valign="top" width="72.57725772577258%" headers="mcps1.1.4.1.3"><p id="p92097207RU01c">Patent Ref: 92097207RU01<br>Application No.: RU2025123028</p></td>
</tr>
</tbody>
</table>

## Disclaimer

This code repository contributes to the Google Research community's open-source projects solely for vector retrieval acceleration. It strictly adheres to the coding style and methods, as well as security design of the native open-source software. Any vulnerability and security issues of the software shall be resolved by the corresponding upstream communities according to their response mechanisms. Please pay attention to the notifications and version updates released by the upstream communities. The Kunpeng computing community does not assume any responsibility for software vulnerabilities and security issues.

## License

KScaNN is licensed under the Apache 2.0 License, which allows modification and redistribution of derivative works as open source.

The documentation of this project is licensed under the CC BY 4.0 License.

## Contribution Statement

We welcome your contributions to the community. If you have any questions/suggestions or want to provide feedback on feature requirements and bug reports, you can submit issues. For details, see the contribution guideline. You are also welcome to share insights in the [Discussions](https://gitcode.com/boostkit/community/discussions). Thank you for your support.

## Acknowledgments

Thank you to everyone in the community for your PRs. We warmly welcome contributions to KScaNN!
