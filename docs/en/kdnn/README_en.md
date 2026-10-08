# Introduction to KDNN

English|[简体中文](../../zh/kdnn/README.md)

## Latest News

- [2026.09.30]: Added thread pool parallelism support for SparseGemm and optimized small-matrix GEMM, and continued to optimize the performance of MatMul and convolution operators on the Kunpeng platform.

- [2026.03.30]: Added MatMul implementation for s8/u8 data types based on Matrix Multiply-Accumulate (MMLA) instructions, and added support for post-processing operations (post-ops) and for the FusedMatMul operator.

- [2025.12.30]: Added NEON-based MatMul implementation, added support for the custom thread pool mode in MatMul, and added Kunpeng platform support for Group Normalization and SparseGemm operators.

- [2025.06.30]: Added Kunpeng platform support for the Pool, Batch Normalization, Local Response Normalization, Reduction, PReLU, Binary, and RNN deep neural network operators. Added support for the new Kunpeng 920 processor model.

- [2024.12.30]: Added Kunpeng platform support for four deep neural network operators, including Reorder, Resampling, Concat, and Shuffle; added Kunpeng platform support for the random_choice and softmax operators in KDNN_EXT.

## Project Overview

Kunpeng AI Library (KAIL) is a high-performance AI operator library optimized for the Kunpeng platform. It is implemented using C/C++ and assembly languages. It includes the Kunpeng Deep Neural Network Library (KDNN) and Kunpeng Deep Neural Network Extension Library (KDNN_EXT) that contains operators such as softmax and random_choice. [Table 1](#table113613052017) describes KAIL components.

**Table 1**  KAIL components

<a name="table113613052017"></a>

| No. | Library | Description | Application Scenario |
| --- | --- | --- | --- |
| 1 | KDNN | A deep neural network library that contains AI operators optimized based on the Kunpeng processor microarchitecture and software optimizations. It can be integrated into open-source oneDNN as an operator library plugin. | Suitable for various machine learning applications, including image classification, object detection, and speech recognition. It can be integrated with various deep learning frameworks, such as TensorFlow and PyTorch. |
| 2 | KDNN_EXT | A deep neural network extension library that contains operators such as softmax and random_choice. They are encapsulated as Python interfaces. | Suitable for scenarios including multi-classification and random selection. It can be integrated with various deep learning frameworks, such as TensorFlow and PyTorch. |

KDNN is available only for Kunpeng processors.

To achieve the optimal performance, KDNN interfaces do not verify all input parameters. The validity of input parameters is ensured by the service that calls the interfaces.

**Application Scenarios<a name="section1957994882217"></a>**

KDNN is mainly used in the following scenarios:

- Deep learning acceleration: image classification, object detection and segmentation, natural language processing, and recommendation systems

- HPC: meteorology, life sciences, manufacturing, and education and scientific research

- Big data: machine learning algorithms

## Release Notes

For details about the KDNN version updates, see [Release Notes](release_notes.md).

## Compatibility Information

To use KDNN smoothly and securely, ensure that your environment is one of the verified environments.

**Table 1** Verified KDNN environments

<a name="table7471331132318"></a>

| Component | OS | CPU | Compiler | Build Tool | Python Interpreter |
| --- | --- | --- | --- | --- | --- |
| KDNN | openEuler 22.03 LTS SP3 | New Kunpeng 920 processor model | GCC 10.3.1 | CMake 3.22.0 | Python 3.9.21 |
| KDNN | openEuler 22.03 LTS SP4<br>(The kernel version is later than 5.10.0-228.0.0.127.) | New Kunpeng 920 processor model | GCC 12.3.1/BiSheng 4.2.0 | CMake 3.22.0 | Python 3.9.21 |
| KDNN_EXT | openEuler 22.03 LTS SP3 | Kunpeng 920 processors | GCC 10.3.1 | CMake 3.22.0 | Python 3.9.21 |

## Related Documents

<a name="table11320174415582"></a>

| Document Name | Content Description |
| --- | --- |
| [Release Notes](release_notes.md) | Provides basic information and feature updates for each KDNN version. |
| [Quick Start](quick_start.md) | Provides guidance for getting started with KDNN. |
| [Installation Guide](installation_guide.md) | Provides detailed instructions for compiling and installing KDNN. |
| [API Reference](api_reference.md) | Provides definitions, descriptions, and calling examples of KDNN APIs. |
| [Best Practices](best_practices.md) | Provides best practices of using KDNN. |

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

We welcome your contributions to the community. If you have any questions/suggestions or want to provide feedback on feature requirements and bug reports, you can submit [issues](https://gitcode.com/boostkit/community/blob/master/docs/contributor/issue-submit.md). For details, see the [contribution guideline](https://gitcode.com/boostkit/community/blob/master/docs/contributor/contributing.md). You are also welcome to share insights in the [Discussions](https://gitcode.com/boostkit/community/discussions). Thank you for your support.

## Acknowledgments

Thank you to everyone in the community for your PRs. We warmly welcome contributions to KDNN!
