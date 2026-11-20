# KScaNN介绍

本文档介绍KScaNN（Kunpeng Scalable Nearest Neighbors），基于倒排索引结合鲲鹏架构深度优化的向量检索算法，适用于鲲鹏处理器向量检索用户。

## 最新消息

- \[2025-12-30\]：KScaNN新增鲲鹏950 7592C处理器兼容。
- \[2025-06-30\]：优化算法性能；新增对接Milvus使用。
- \[2024-12-30\]：新增基于鲲鹏架构深度优化索引布局和算法流程，鲲鹏亲和的自研算法体系KScaNN。

## 项目介绍

KScaNN（Kunpeng Scalable Nearest Neighbors）是基于倒排索引，结合鲲鹏架构深度优化索引布局、算法流程和计算流程，充分挖掘芯片潜力形成的向量检索算法。

KScaNN适用于鲲鹏920 7282C处理器与鲲鹏950 7592C处理器，支持NEON指令（128位宽）和SVE指令（256位宽）。

## 版本说明

关于KScaNN的版本更新情况请参见《[版本说明书](./release_notes.md)》。

## 学习文档

| 学习文档名称 | 学习文档简介 |
| --- | --- |
| 《[版本说明书](./release_notes.md)》 | 提供KScaNN每个发布版本的基础信息和特性更新信息。 |
| 《[快速入门](./quick_start.md)》 | 提供KScaNN快速入门指导。 |
| 《[安装指南](./installation_guide.md)》 | 提供KScaNN编译安装方法指导。 |
| 《[最佳实践](./best_practices.md)》 | 提供KScaNN的使用实践案例。 |
| 《[API参考](./api_reference.md)》 | 提供KScaNN的API接口定义和接口说明。 |

## 免责声明

此代码仓计划参与GoogleResearch社区开源，仅作用于向量检索加速，编码风格遵照开源软件，继承开源软件安全设计，不破坏开源软件设计及编码风格和方式，软件的任何漏洞与安全问题，均由相应的上游社区根据其漏洞和安全响应机制解决。请密切关注上游社区发布的通知和版本更新。鲲鹏计算社区对软件的漏洞及安全问题不承担任何责任。

## License

KScaNN采用Apache 2.0 License许可证授权，支持修改代码和再开源。具体请参见[LICENSE](../../../LICENSE)文件。

本项目的文档适用CC-BY 4.0许可证，具体请参见[LICENSE](../../LICENSE)文件。

## 贡献声明

欢迎大家为社区做贡献，如果使用过程中有任何问题/建议，或者需要反馈特性需求和bug报告，可以提交[Issues](https://gitcode.com/boostkit/community/blob/master/docs/contributor/issue-submit.md)联系我们，具体贡献方法可参考[贡献指南](https://gitcode.com/boostkit/community/blob/master/docs/contributor/contributing.md)。同时也欢迎大家在[讨论专区](https://gitcode.com/boostkit/community/discussions)展开讨论交流。感谢您的支持。

## 致谢

感谢来自社区的每一个PR，欢迎贡献KScaNN！
