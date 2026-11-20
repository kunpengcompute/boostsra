# 版本说明书

## 版本配套说明

### 产品版本信息

<a name="table62675726"></a>

|  项目| 内容 |
| --- | --- |
| 产品名称 | Kunpeng BoostKit |
| 产品版本 | 25.3.0 |
| 软件名称 | KBest |

### 与操作系统、编译器和CPU配套说明

**表 1** KBest已验证环境<a id="KBest已验证环境"></a>

<a name="table59918346913"></a>

| 操作系统 | CPU类型 | 内存 | 编译器 | 其他 |
| --- | --- | --- | --- | --- |
| openEuler 22.03 LTS SP3 | 鲲鹏920 7282C处理器 | 16*32GB | GCC 12.3.1 | CMake>=3.22.0<br>GLIBCXX>=3.4.29<br>Python 3.9.x |
| openEuler 22.03 LTS SP3 | 鲲鹏920 7282C处理器 | 16*32GB | GCC 10.3.1 | CMake>=3.22.0<br>GLIBCXX>=3.4.28<br>Python 3.9.x |
| openEuler 24.03 LTS SP1 | 鲲鹏920 7282C处理器 | 16*32GB | GCC 12.3.1 | CMake>=3.22.0<br>GLIBCXX>=3.4.29<br>Python 3.9.x |
| openEuler 24.03 LTS SP3 | 鲲鹏950 7592C处理器 | 24*64GB | GCC 12.3.1 | CMake>=3.22.0<br>GLIBCXX>=3.4.29<br>Python 3.9.x |

### 病毒扫描结果

本软件包、版本文档、产品文档经过防病毒软件扫描，未发现病毒。详细信息如下：

<a name="table1980419519233"></a>

| 防病毒软件名称 | 防病毒软件版本 | 病毒库版本 | 扫描时间 | 扫描结果 |
| --- | --- | --- | --- | --- |
| QiAnXin | 8.0.5.5260 | 2025-06-27 08:00:00.0 | 2025-06-28 17:37:20 | OK |
| Bitdefender | 7.0.3.2038 | 7.99075 | 2025-06-28 17:37:27 | OK |
| Kaspersky | 12.0.0.6672 | 2025-06-27 02:05:00 | 2025-06-28 17:37:17 | OK |

## 版本使用注意事项

### 使用注意事项

请参见《[安装指南](./installation_guide.md)》。

## V25.3.0

### 更新说明

**新增特性<a name="section11862975"></a>**

KBest新增鲲鹏950 7592C处理器兼容。

**修改特性<a name="section16450949161512"></a>**

无

**删除特性<a name="section9218125814159"></a>**

无

### 已解决的问题

无

### 遗留问题

无

## V25.2.RC1

### 更新说明

25.2.RC1版本为鲲鹏BoostKit版本号，该版本之后的组件版本号不再进行更新（即BoostKit-SRA\_Recall\_1.2.0.zip中的1.2.0不会再升级）。

**新增特性<a name="section11862975"></a>**

KBest本次未更新，代码尚未开源，请您通过《KBest安装指南》获取BoostKit-SRA\_Recall\_1.2.0.zip安装并使用。

**修改特性<a name="section16450949161512"></a>**

无

**删除特性<a name="section9218125814159"></a>**

无

### 已解决的问题

无

### 遗留问题

无

## V1.2.0

### 更新说明

**新增特性<a name="section11862975"></a>**

<a name="table41916133"></a>

| 算法名称 | 更新说明 |
| --- | --- |
| KBest | 优化算法性能；新增SetEarlyStoppingParams接口，修改Add接口和构造函数。 |

**修改特性<a name="section16450949161512"></a>**

无

**删除特性<a name="section9218125814159"></a>**

无

### 已解决的问题

无

### 遗留问题

无

## V1.1.0

### 更新说明

**新增特性<a name="section11862975"></a>**

<a name="table41916133"></a>

| 算法名称 | 更新说明 |
| --- | --- |
| KBest | 新增SaveGraph/LoadGraph接口、Serialize/Deserialize接口、BuildSearcher及GetNTotal和GetDim接口，并且修改Add、Save和Load接口，目前已对接Milvus使用。 |

**修改特性<a name="section16450949161512"></a>**

无

**删除特性<a name="section9218125814159"></a>**

无

### 已解决的问题

无

### 遗留问题

无

## V1.0.0

### 更新说明

**新增特性<a name="section11862975"></a>**

<a name="table41916133"></a>

| 算法名称 | 更新说明 |
| --- | --- |
| KBest | 新增鲲鹏自研的高效的图检索算法KBest（Kunpeng Blazing-fast embedding similarity search thruster）。 |

**修改特性<a name="section16450949161512"></a>**

无

**删除特性<a name="section9218125814159"></a>**

无

### 已解决的问题

无

### 遗留问题

无

## 版本配套文档

### V25.3.0版本配套文档<a name="ZH-CN_TOPIC_0000002518393700"></a>

<a name="table41916133"></a>

| 文档名称 | 内容简介 | 交付形式 |
| --- | --- | --- |
| 《版本说明书》 | 本文档提供KBest的版本发布信息。 | 开源仓 |
| 《快速入门》 | 本文档提供KBest快速入门指导。 | 开源仓 |
| 《安装指南》 | 本文档提供KBest安装、部署指导。 | 开源仓 |
| 《最佳实践》 | 本文档提供KBest典型场景使用实践。 | 开源仓 |
| 《API参考》 | 本文档提供KBest对外提供的API接口详细说明。 | 开源仓 |

### 获取文档的方法<a name="ZH-CN_TOPIC_0000002518393680"></a>

您可以通过访问[开源仓](https://gitcode.com/boostkit/boostsra/blob/master/docs/zh/kbest/README.md)浏览和获取相关文档。
