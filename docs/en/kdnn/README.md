# Introduction to KDNN

## Latest Updates

- [2026.03.30]: Added MatMul implementation for s8/u8 data types based on Matrix Multiply-Accumulate (MMLA) instructions, and added support for post-processing operations (post-ops) and for the FusedMatMul operator.
- [2025.12.30]: Added NEON-based MatMul implementation, added support for the custom thread pool mode in MatMul, and added Kunpeng platform support for Group Normalization and SparseGemm operators.
- [2025.06.30]: Added Kunpeng platform support for the Pool, Batch Normalization, Local Response Normalization, Reduction, PReLU, Binary, and RNN deep neural network operators. Added support for the new Kunpeng 920 processor model.
- [2024.12.30]: Added Kunpeng platform support for four deep neural network operators, including Reorder, Resampling, Concat, and Shuffle.

## Project Overview

Kunpeng AI Library (KAIL) is implemented using C/C++ and assembly language. It is a high-performance AI operator library optimized by Huawei for the Kunpeng platform. It includes the Kunpeng Deep Neural Network Library (KDNN) and Kunpeng Deep Neural Network Extension Library (KDNN_EXT) that contains operators such as softmax and random_choice. [Table 1](#table113613052017) describes KAIL components.

**Table 1** KDNN components
<div id="table113613052017"></div>
<table><thead align="left"><tr id="row237018052015">
<th class="cellrowborder" valign="top" width="13.83%" id="mcps1.2.5.1.2"><p id="p10370130112016"><a name="p10370130112016"></a><a name="p10370130112016"></a>Library</p>
</th>
<th class="cellrowborder" valign="top" width="44.11%" id="mcps1.2.5.1.3"><p id="p173704019205"><a name="p173704019205"></a><a name="p173704019205"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="36.059999999999995%" id="mcps1.2.5.1.4"><p id="p737019032019"><a name="p737019032019"></a><a name="p737019032019"></a>Application Scenario</p>
</th>
</tr>
</thead>
<tbody><tr id="row737011016208">
<td class="cellrowborder" valign="top" width="13.83%" headers="mcps1.2.5.1.2 "><p id="p1237011013202"><a name="p1237011013202"></a><a name="p1237011013202"></a>KDNN</p>
</td>
<td class="cellrowborder" valign="top" width="44.11%" headers="mcps1.2.5.1.3 "><p id="p193701909209"><a name="p193701909209"></a><a name="p193701909209"></a>A deep neural network library that contains AI operators optimized based on the Kunpeng processor microarchitecture and software optimizations. It can be integrated into open-source oneDNN as an operator library plugin.</p>
</td>
<td class="cellrowborder" valign="top" width="36.059999999999995%" headers="mcps1.2.5.1.4 "><p id="p153707032017"><a name="p153707032017"></a><a name="p153707032017"></a>Suitable for various machine learning applications, including image classification, object detection, and speech recognition. It can be integrated with various deep learning frameworks, such as TensorFlow and PyTorch.</p>
</td>
</tr>
<tr id="row163701804202">
<td class="cellrowborder" valign="top" width="13.83%" headers="mcps1.2.5.1.2 "><p id="p163704072014"><a name="p163704072014"></a><a name="p163704072014"></a>KDNN_EXT</p>
</td>
<td class="cellrowborder" valign="top" width="44.11%" headers="mcps1.2.5.1.3 "><p id="p73701209208"><a name="p73701209208"></a><a name="p73701209208"></a>A deep neural network extension library that contains operators such as softmax and random_choice. They are encapsulated as Python interfaces.</p>
</td>
<td class="cellrowborder" valign="top" width="36.059999999999995%" headers="mcps1.2.5.1.4 "><p id="p1237015014202"><a name="p1237015014202"></a><a name="p1237015014202"></a>Suitable for scenarios including multi-classification and random selection. It can be integrated with various deep learning frameworks, such as TensorFlow and PyTorch.</p>
</td>
</tr>
</tbody>
</table>

KDNN is available only for Kunpeng processors.

To achieve the optimal performance, KDNN interfaces do not verify all input parameters. The validity of input parameters is ensured by the service that calls the interfaces,

**Application Scenarios<a name="section1957994882217"></a>**

KDNN is mainly used in the following scenarios:

- Deep learning acceleration: image classification, object detection and segmentation, natural language processing, and recommendation systems
- HPC: meteorology, life sciences, manufacturing, and education and scientific research
- Big data: machine learning algorithms

## Release Notes

For details about the KDNN version updates, see the <a href="release_notes.md">Release Notes</a>.

## Compatibility Information

To use KDNN smoothly and securely, ensure that your environment is one of the verified environments.

**Table 1** Verified KDNN environments

<a name="table7471331132318"></a>
<table><thead align="left"><tr id="row757143152315"><th class="cellrowborder" valign="top" width="12.15%" id="mcps1.2.7.1.1"><p id="p457831192313"><a name="p457831192313"></a><a name="p457831192313"></a>Component</p>
</th>
<th class="cellrowborder" valign="top" width="19.97%" id="mcps1.2.7.1.2"><p id="p5571831182318"><a name="p5571831182318"></a><a name="p5571831182318"></a>OS</p>
</th>
<th class="cellrowborder" valign="top" width="22.32%" id="mcps1.2.7.1.3"><p id="p55733113238"><a name="p55733113238"></a><a name="p55733113238"></a>CPU</p>
</th>
<th class="cellrowborder" valign="top" width="18.94%" id="mcps1.2.7.1.4"><p id="p35713152318"><a name="p35713152318"></a><a name="p35713152318"></a>Compiler</p>
</th>
<th class="cellrowborder" valign="top" width="11.07%" id="mcps1.2.7.1.5"><p id="p135718319231"><a name="p135718319231"></a><a name="p135718319231"></a>Build Tool</p>
</th>
<th class="cellrowborder" valign="top" width="15.55%" id="mcps1.2.7.1.6"><p id="p657153142317"><a name="p657153142317"></a><a name="p657153142317"></a>Python Interpreter</p>
</th>
</tr>
</thead>
<tbody><tr id="row165716316236"><td class="cellrowborder" valign="top" width="12.15%" headers="mcps1.2.7.1.1 "><p id="p4571531192317"><a name="p4571531192317"></a><a name="p4571531192317"></a>KDNN</p>
</td>
<td class="cellrowborder" valign="top" width="19.97%" headers="mcps1.2.7.1.2 "><p id="p45713315237"><a name="p45713315237"></a><a name="p45713315237"></a>openEuler 22.03 LTS SP3</p>
</td>
<td class="cellrowborder" valign="top" width="22.32%" headers="mcps1.2.7.1.3 "><p id="p2057631172312"><a name="p2057631172312"></a><a name="p2057631172312"></a>Kunpeng 920 processors</p>
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
<p id="p105793172319"><a name="p105793172319"></a><a name="p105793172319"></a>(The kernel version is later than 5.10.0-228.0.0.127.)</p>
</td>
<td class="cellrowborder" valign="top" width="22.32%" headers="mcps1.2.7.1.3 "><p id="p65733172315"><a name="p65733172315"></a><a name="p65733172315"></a>New Kunpeng 920 processor model</p>
</td>
<td class="cellrowborder" valign="top" width="18.94%" headers="mcps1.2.7.1.4 "><p id="p1757183162316"><a name="p1757183162316"></a><a name="p1757183162316"></a>GCC 12.3.1/BiSheng 4.2.0</p>
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
<td class="cellrowborder" valign="top" width="22.32%" headers="mcps1.2.7.1.3 "><p id="p7571931162318"><a name="p7571931162318"></a><a name="p7571931162318"></a>Kunpeng 920 processors</p>
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

## Related Documents

<a name="table11320174415582"></a>
<table><thead align="left"><tr id="row532024445820">
<th class="cellrowborder" valign="top" width="28.012801280128013%" id="mcps1.1.4.1.2"><p id="p14321184425814"><a name="p14321184425814"></a><a name="p14321184425814"></a>Resource Name</p>
</th>
<th class="cellrowborder" valign="top" width="57.18571857185718%" id="mcps1.1.4.1.3"><p id="p1932112447589"><a name="p1932112447589"></a><a name="p1932112447589"></a>Resource Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row183211844195812">
<td class="cellrowborder" valign="top" width="28.012801280128013%" headers="mcps1.1.4.1.2 "><p id="p132119442580"><a name="p132119442580"></a><a name="p132119442580"></a><a href="release_notes.md"> Release Notes</a></p>
</td>
<td class="cellrowborder" valign="top" width="57.18571857185718%" headers="mcps1.1.4.1.3 "><p id="p13321194412589"><a name="p13321194412589"></a><a name="p13321194412589"></a>Provides basic information and feature updates for each KDNN version.</p>
</td>
</tr>
<tr id="row4533125512117">
<td class="cellrowborder" valign="top" width="28.012801280128013%" headers="mcps1.1.4.1.2 "><p id="p032144418580"><a name="p032144418580"></a><a name="p032144418580"></a><a href="quick_start.md">Quick Start</a> </p>
</td>
<td class="cellrowborder" valign="top" width="57.18571857185718%" headers="mcps1.1.4.1.3 "><p id="p83216449586"><a name="p83216449586"></a><a name="p83216449586"></a>Provides guidance for getting started with KDNN.</p>
</td>
</tr>
<tr id="row6321164455815">
<td class="cellrowborder" valign="top" width="28.012801280128013%" headers="mcps1.1.4.1.2 "><p id="p14321104418585"><a name="p14321104418585"></a><a name="p14321104418585"></a><a href="installation_guide.md">Installation Guide</a></p>
</td>
<td class="cellrowborder" valign="top" width="57.18571857185718%" headers="mcps1.1.4.1.3 "><p id="p1332134420587"><a name="p1332134420587"></a><a name="p1332134420587"></a>Provides detailed instructions for compiling and installing KDNN.</p>
</td>
</tr>
<tr id="row13219448585">
<td class="cellrowborder" valign="top" width="28.012801280128013%" headers="mcps1.1.4.1.2 "><p id="p5321124418587"><a name="p5321124418587"></a><a name="p5321124418587"></a><a href="api_reference.md">API Reference</a></p>
</td>
<td class="cellrowborder" valign="top" width="57.18571857185718%" headers="mcps1.1.4.1.3 "><p id="p53214445588"><a name="p53214445588"></a><a name="p53214445588"></a>Provides definitions, descriptions, and calling examples of KDNN APIs.</p>
</td>
</tr>
<tr id="row1632118447589">
<td class="cellrowborder" valign="top" width="28.012801280128013%" headers="mcps1.1.4.1.2 "><p id="p183213445582"><a name="p183213445582"></a><a name="p183213445582"></a><a href="best_practices.md">Best Practices</a></p>
</td>
<td class="cellrowborder" valign="top" width="57.18571857185718%" headers="mcps1.1.4.1.3 "><p id="p232174455818"><a name="p232174455818"></a><a name="p232174455818"></a>Provides best practices of using KDNN.</p>
</td>
</tr>
</tbody>
</table>

## Disclaimer

**To users of this project**

- This project is intended solely for debugging and development. You are responsible for any risks and should carefully review the following information:
  - Data processing and deletion: Users are responsible for managing and deleting any data generated while using this tool. Users are advised to delete such data promptly after use to prevent information leakage.
  - Data confidentiality and transmission: Users understand and agree not to share or transmit any data generated by this tool. Neither the tool nor its developers are responsible for any information leaks, data breaches, or other negative consequences.
  - User input security: Users are responsible for the security of any commands they enter and for any risks or losses resulting from improper input. The tool and its developers are not liable for issues caused by incorrect command usage.

- Disclaimer scope: This disclaimer applies to all individuals and entities using this tool. By using the tool, you acknowledge and accept this statement and assume all risks and responsibilities arising from its use. If you do not agree, please stop using the tool immediately.
- Before using this tool, **please read and understand the preceding disclaimer**. If you have any questions, contact the developer.

**To data owners**

If you do not want your model or dataset to be mentioned in this project, or if you wish to update its description, please submit an issue on GitCode. We will delete or update your description according to your request. Thank you for your understanding and contribution to this project.

## License

The documents of this project are licensed under CC-BY 4.0. For details, see [LICENSE](LICENSE).

## Contribution Statement

We welcome your contributions to the community. If you have any questions/suggestions or want to provide feedback on feature requirements and bug reports, you can submit issues. For details, see the contribution guideline. You are also welcome to share insights in the [Discussions](https://gitcode.com/boostkit/community/discussions). Thank you for your support.

## Acknowledgments

Thank you to everyone in the community for your PRs. We warmly welcome contributions to KDNN!
