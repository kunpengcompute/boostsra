# BoostSRA鲲鹏搜推广使能套件
鲲鹏BoostKit搜推广使能套件旨在为互联网搜索、推荐、广告业务场景提供基于鲲鹏平台的应用层加速能力，组件涵盖召回场景核心检索算法、排序场景模型推理软件框架优化。
## 架构图
![image.png](https://raw.gitcode.com/user-images/assets/7311696/d58030cc-4e12-4ffc-b802-70a75114db65/image.png 'image.png')

## 社区
* 鲲鹏社区搜推广首页
  * https://www.hikunpeng.com/developer/boostkit/sra
## 召回算法
* KBest召回算法
  * Kunpeng Blazing-fast embedding similarity search thruster，是鲲鹏自研的高性能图检索算法，专为大规模嵌入相似性搜索场景设计。
  * [待开源]
* KScaNN召回算法
  * Kunpeng Scalable Nearest Neighbors，鲲鹏向量检索算法，基于倒排索引，结合鲲鹏架构深度优化索引布局和算法流程，充分挖掘芯片潜力形成的向量检索算法。
  * [待开源]
* KRL检索算子库
  * Kunpeng Retrieval Library，鲲鹏检索算子库，基于鲲鹏平台优化的用于加速向量检索的算子库，KRL可通过替换算子的形式对faiss原生的HNSW、PQFS、IVFPQ和IVFPQFS等算法进行加速。
  * [待开源]
* KVecTurbo召回向量检索加速组件
  * KVecTurbo是鲲鹏自研的向量检索加速组件，可对接openGauss向量数据库使用。KVecTurbo通过将高维向量量化压缩，快速获取query的近邻，同时使用SIMD指令集加速距离计算，用于多维向量最近邻搜索。
  * https://gitcode.com/boostkit/kvecturbo

## 召回算法扩展
*  [Pfordelta](https://github.com/diegocaro/compression)扩展
   * 基于鲲鹏SIMD指令集的召回场景倒排索引PForDelta解压缩加速优化。
   * https://gitcode.com/boostkit/knewpfordelta

## 排序推理
* KDNN算子库
  * Kunpeng Deep Neural Network Library，鲲鹏深度神经网络算子库，结合鲲鹏处理器微架构特性，通过向量化、汇编、算法优化等手段，提升DNN核心算子性能。
  * [待开源]
* ANNC编译器
  * ANNC（Accelerated Neural Network Compiler）是专注于加速神经网络计算的编译器，聚焦于通过计算图优化，高性能融合算子生成和对接技术以及高效代码生成和优化能力，加速推荐和大模型的推理性能，支持主流开源推理框架接入。
  * https://gitee.com/src-openeuler/ANNC

## 排序推理扩展 
* [TensorFlow](https://github.com/tensorflow/tensorflow) 扩展
  * TensorFlow框架鲲鹏亲和优化，包含TF原生算子优化等特性。
  * https://gitcode.com/boostkit/tensorflow
* [TensorFlow serving](https://github.com/tensorflow/serving) 扩展
  * TensorFlow serving框架鲲鹏亲和优化，包含线程调度优化等特性。
  * https://gitcode.com/boostkit/tensorflow-serving
* [TVM](https://github.com/apache/tvm) 扩展
  * TVM框架鲲鹏亲和优化，包含softmax算子优化等特性。
  * https://gitee.com/openeuler/sra_tvm_adapter
* [oneDNN](https://github.com/uxlfoundation/oneDNN) 扩展
  * KDNN算子库通过插件化形式对接开源oneDNN库提供完整能力
  * https://gitee.com/openeuler/kail_dnn_adapter

## 工具
### Benchmark
* 搜推模型推理性能Benchmark
  * 包含DLRM、Wide & Deep等多个模型的排序推理性能Benchmark
  * https://gitee.com/openeuler/sra_benchmark

## 文档
* 鲲鹏BoostKit搜推广使能套件特性列表
  * https://www.hikunpeng.com/document/detail/zh/SRA/overview/kunpengsra.html

## 讨论
如果发现问题，请进入[讨论](https://gitcode.com/BoostKit/BoostSRA/discussions)与我们联系。

## 许可协议
使用本领域源码及其附带软件，即视为您已阅读、理解并同意相关软件许可协议条款与条件的约束。