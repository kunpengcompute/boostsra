# API参考

本文档介绍KScaNN API参考，提供Python和C++接口的详细使用说明，适用于需要使用KScaNN进行向量检索的用户。

## Python接口

### 接口说明

KScaNN不提供对外接口，基于开源ScaNN算法做侵入式修改，对开源接口有新增。为获得最优性能，KScaNN接口内部不做完整入参校验，入参合法性由调用方业务来保证。KScaNN侵入式修改后的ScaNN所提供的Python接口如[**表 1** KScaNN修改后的Python接口](#KScaNN修改后的Python接口)所示。

**表 1** KScaNN修改后的Python接口<a id="KScaNN修改后的Python接口"></a>

<a name="table1194910128449"></a>

| 接口名称 | 接口作用 |
| --- | --- |
| set_num_threads | 配置搜索时启用线程数（相比开源算法新增的接口）。 |
| search_additional_params | 用于扩展ScaNN检索功能，提供额外的检索参数配置接口（相比开源算法新增的接口）。 |
| search | 单query搜索接口，单线程执行（与开源算法保持一致）。 |
| search_batched | 批量query搜索接口，单线程执行（与开源算法保持一致）。 |
| search_batched_parallel | 并行批量query搜索接口，多线程并发执行（与开源算法保持一致）。 |
| builder | 用于开始构建（与开源算法保持一致）。 |
| tree | 添加IVF分区的相关参数（与开源算法保持一致）。 |
| score_ah | 添加PQ分区量化的相关参数（与开源算法保持一致）。 |
| reorder | 添加重排的相关参数（与开源算法保持一致）。 |
| build | 用于构建索引（与开源算法保持一致）。 |
| serialize_to_mem | 将构建好的索引储存在数组中（相比开源算法新增的接口）。 |
| deserialize_from_mem | 给定存储序列化内容的数组，还原一个检索器的索引实例（相比开源算法新增的接口）。 |
| get_num | 获取底库向量的数量（相比开源算法新增的接口）。 |
| get_dim | 获取底库向量的维度（相比开源算法新增的接口）。 |
| create_searcher | 基于入参构建索引并返回ScannSearcher（与开源算法相比增加filter_thr和filter_type参数）。 |

### set\_num\_threads

**接口定义<a name="section172317194488"></a>**

def set\_num\_threads\(num\_threads: int\) -\> None

**接口用途<a name="section1153124784912"></a>**

配置搜索时启用线程数（相比开源算法新增的接口）。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>

| 参数名称 | 数据类型 | 描述 | 取值范围 |
| --- | --- | --- | --- |
| num_threads | int | 线程数量。 | 大于等于2，推荐配置为运行时CPU核数。 |

### search\_additional\_param

**接口定义<a name="section172317194488"></a>**

def search\_additional\_params \(adp\_threshold: float, refine\_prm: float, adp\_refined: int, leaves\_to\_search: int\) -\> bool

**接口用途<a name="section1153124784912"></a>**

用于扩展ScaNN检索功能，提供额外的检索参数配置接口（相比开源算法新增的接口）。应在索引构建后、检索前调用设置，接口参数具备缓存功能，一次设置，后续检索均生效。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>

| 参数名称 | 数据类型 | 描述 | 取值范围 |
| --- | --- | --- | --- |
| adp_threshold | float | 决策阈值，典型值0.3。 | [0.1, 0.8] |
| refine_prm | float | 精细化控制过滤策略，典型值0.2，值越大则过滤的子空间个数越少，精度越高，但性能会下降。 | [0.0, 1.0]，默认为0.0。 |
| adp_refined | int | 简单query所采用的子空间个数，典型值0，为训练自适应值（75分位点）。 | [0, leaves_to_search]，其中“leaves_to_search”表示复杂query所采用的子空间个数。 |
| leaves_to_search | int | 复杂query所采用的子空间个数，应与实际检索（search*）接口参数一致。 | [1, num_leaves]，其中“num_leaves”表示IVF（Inverted File）倒排索引分区总子空间个数。 |

**返回值<a name="section49971832106"></a>**

<a name="table17997635100"></a>

| 数据类型 | 说明 |
| --- | --- |
| bool | 算法库加载成功，根据设置功能激活时返回True；否则返回False。 |

### search

**接口定义<a name="section172317194488"></a>**

def search\(q: numpy.ndarray, final\_num\_neighbors: int, pre\_reorder\_num\_neighbors: int, leaves\_to\_search: int\) -\> tuple\(idx, dist\)

**接口用途<a name="section1153124784912"></a>**

单query搜索接口，单线程执行（与开源算法保持一致）。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>

| 参数名称 | 数据类型 | 描述 | 取值范围 |
| --- | --- | --- | --- |
| q | numpy.ndarray | Query。 | 限制非空。 |
| final_num_neighbors | int | 最终返回结果数量，TopK。 | 大于等于1。 |
| pre_reorder_num_neighbors | int | 重排前保存结果数量。 | 大于等于final_num_neighbors，其中“final_num_neighbors”为最终返回结果数量。 |
| leaves_to_search | int | 搜索子空间数量。 | [1, num_leaves]，其中“num_leaves”为IVF倒排索引分区总子空间个数。 |

**返回值<a name="section49971832106"></a>**

<a name="table17997635100"></a>

| 数据类型 | 说明 |
| --- | --- |
| tuple(idx, dist) | idx为包含final_num_neighbors个底库ID的numpy.ndarray；dist为包含final_num_neighbors个距离的numpy.ndarray。 |

### search\_batched

**接口定义<a name="section172317194488"></a>**

def search\_batched\(queries: numpy.ndarray, final\_num\_neighbors: int, pre\_reorder\_num\_neighbors: int, leaves\_to\_search: int\) -\> tuple\(idx, dist\)

**接口用途<a name="section1153124784912"></a>**

批量query搜索接口，单线程执行（与开源算法保持一致）。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>

| 参数名称 | 数据类型 | 描述 | 取值范围 |
| --- | --- | --- | --- |
| queries | numpy.ndarray | 批次内的Queries。 | 限制非空。 |
| final_num_neighbors | int | 最终返回结果数量。 | 大于等于1。 |
| pre_reorder_num_neighbors | int | 重排前保存结果数量。 | 大于等于final_num_neighbors，其中“final_num_neighbors”为最终返回结果数量。 |
| leaves_to_search | int | 搜索子空间数量。 | [1, num_leaves]，其中“num_leaves”为IVF倒排索引分区总子空间个数。 |

**返回值<a name="section49971832106"></a>**

<a name="table17997635100"></a>

| 数据类型 | 说明 |
| --- | --- |
| tuple(idx, dist) | idx为包含final_num_neighbors个底库ID的numpy.ndarray；dist为包含final_num_neighbors个距离的numpy.ndarray。 |

### search\_batched\_parallel

**接口定义<a name="section172317194488"></a>**

def search\_batched\_parallel\(queries: numpy.ndarray, final\_num\_neighbors: int, pre\_reorder\_num\_neighbors:int, leaves\_to\_search: int, batch\_size: int\) -\> tuple\(idx, dist\)

**接口用途<a name="section1153124784912"></a>**

并行批量query搜索接口，多线程并发执行（与开源算法保持一致）。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>

| 参数名称 | 数据类型 | 描述 | 取值范围 |
| --- | --- | --- | --- |
| queries | numpy.ndarray | 批次内的Queries。 | 限制非空。 |
| final_num_neighbors | int | 最终返回结果数量，TopK。 | 大于等于1。 |
| pre_reorder_num_neighbors | int | 重排前保存结果数量。 | 大于等于final_num_neighbors，其中“final_num_neighbors”为最终返回结果数量。 |
| leaves_to_search | int | 搜索子空间数量。 | [1, num_leaves]，其中“num_leaves”为IVF倒排索引分区总子空间个数。 |
| batch_size | int | 并行自动分批时优先批次大小，默认值256。 | 大于等于1。 |

**返回值<a name="section49971832106"></a>**

<a name="table17997635100"></a>

| 数据类型 | 说明 |
| --- | --- |
| tuple(idx, dist) | idx为包含final_num_neighbors个底库ID的numpy.ndarray；dist为包含final_num_neighbors个距离的numpy.ndarray。 |

### builder

**接口定义<a name="section172317194488"></a>**

def builder\(db: numpy.ndarray, num\_neighbors: int, distance\_measure: string\) -\> scann.scann\_ops.py.scann\_builder.ScannBuilder

**接口用途<a name="section1153124784912"></a>**

用于开始构建（与开源算法保持一致）。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>

| 参数名称 | 数据类型 | 描述 | 取值范围 |
| --- | --- | --- | --- |
| db | numpy.ndarray | 底库向量。 | 限制非空。 |
| num_neighbors | int | 最终返回结果数量，TopK。 | 大于等于1。 |
| distance_measure | 字符串 | 距离度量的方式。 | “dot_product”或“squared_l2” |

**返回值<a name="section49971832106"></a>**

<a name="table17997635100"></a>

| 数据类型 | 说明 |
| --- | --- |
| scann.scann_ops.py.scann_builder.ScannBuilder | ScannBuilder类用于接收构建参数。 |

### tree

**接口定义<a name="section172317194488"></a>**

def tree\(num\_leaves: int, num\_leaves\_to\_search: int, training\_sample\_size: int, min\_partition\_size: int, training\_iterations: int, spherical: bool, quantize\_centroids: bool, random\_init: bool, soar\_lambda: float, overretrieve\_factor: float, distance\_measure: string\)  -\> scann.scann\_ops.py.scann\_builder.ScannBuilder

**接口用途<a name="section1153124784912"></a>**

添加IVF（Inverted File）倒排索引分区的相关参数（与开源算法保持一致）。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>

| 参数名称 | 数据类型 | 描述 | 取值范围 |
| --- | --- | --- | --- |
| num_leaves | int | IVF分区总子空间个数。 | 大于等于1。 |
| num_leaves_to_search | int | 默认搜索子空间个数。 | [1, num_leaves]，其中“num_leaves”为IVF倒排索引分区总子空间个数。 |
| training_sample_size | int | 分区训练时底库抽样个数。 | [0, 底库数量] |
| min_partition_size | int | 最小分区包含的底库向量个数。 | [0, 底库数量] |
| training_iterations | int | 训练循环次数。 | 大于等于1。 |
| spherical | 布尔值 | 分区类型是否为spherical。 | - |
| quantize_centroids | 布尔值 | 是否量化桶中心。 | - |
| random_init | 布尔值 | 训练时是否随机开始。 | - |
| soar_lambda | float | 控制正交性的参数，仅对IP(dot_product)数据集生效。 | 大于0，当值为-1时表示不开启此参数。 |
| overretrieve_factor | float | 指定过检索因子，与“soar_lambda”一起使用，仅对IP(dot_product)数据集生效。 | [1,2]，当值为-1时表示不开启此参数。 |
| distance_measure | 字符串 | 向量的距离类型。 | “dot_product”或“squared_l2” |

**返回值<a name="section49971832106"></a>**

<a name="table17997635100"></a>

| 数据类型 | 说明 |
| --- | --- |
| scann.scann_ops.py.scann_builder.ScannBuilder | ScannBuilder类用于接收构建参数。 |

### score\_ah

**接口定义<a name="section172317194488"></a>**

def score\_ah\(dimensions\_per\_block: int, anisotropic\_quantization\_threshold: float, training\_sample\_size: int, min\_cluster\_size: int, hash\_type: string, training\_iterations: int\) -\> scann.scann\_ops.py.scann\_builder.ScannBuilder

**接口用途<a name="section1153124784912"></a>**

添加PQ分区量化的相关参数（与开源算法保持一致）。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>

| 参数名称 | 数据类型 | 描述 | 取值范围 |
| --- | --- | --- | --- |
| dimensions_per_block | int | PQ量化合并维度数。 | [1, 数据维度] |
| anisotropic_quantization_threshold | float | 不对称分桶参数，仅对L2(squared_l2)数据集生效。 | [0, 1] |
| training_sample_size | int | PQ分区训练时底库抽样个数。 | [0, 底库数量] |
| min_cluster_size | int | 最小PQ分区包含的底库向量个数。 | [0, 底库数量] |
| hash_type | 字符串 | PQ量化类型。 | “lut16”或“lut256”。 |
| training_iterations | int | 训练循环次数。 | 大于等于1。 |

**返回值<a name="section49971832106"></a>**

<a name="table17997635100"></a>

| 数据类型 | 说明 |
| --- | --- |
| scann.scann_ops.py.scann_builder.ScannBuilder | ScannBuilder类用于接收构建参数。 |

### reorder

**接口定义<a name="section172317194488"></a>**

def reorder\(reordering\_num\_neighbors: int, quantize: bool\) -\> scann.scann\_ops.py.scann\_builder.ScannBuilder

**接口用途<a name="section1153124784912"></a>**

添加重排的相关参数（与开源算法保持一致）。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>

| 参数名称 | 数据类型 | 描述 | 取值范围 |
| --- | --- | --- | --- |
| reordering_num_neighbors | int | 进入重排的数量。 | [0, 底库数量] |
| quantize | 布尔值 | 是否量化。 | - |

**返回值<a name="section49971832106"></a>**

<a name="table17997635100"></a>

| 数据类型 | 说明 |
| --- | --- |
| scann.scann_ops.py.scann_builder.ScannBuilder | ScannBuilder类用于接收构建参数。 |

### build

**接口定义<a name="section172317194488"></a>**

def build\(\) -\> scann.scann\_ops.ScannSearcher

**接口用途<a name="section1153124784912"></a>**

用于构建索引（与开源算法保持一致）。

**参数说明<a name="section157501312135019"></a>**

无入参。

**返回值<a name="section49971832106"></a>**

<a name="table17997635100"></a>

| 数据类型 | 说明 |
| --- | --- |
| scann.scann_ops.ScannSearcher | 开始构建并返回构建好的ScannSearcher。 |

### serialize\_to\_mem

**接口定义<a name="section172317194488"></a>**

def serialize\_to\_mem\(\) -\> numpy.ndarray

**接口用途<a name="section1153124784912"></a>**

将构建好的索引储存在数组中（相比开源算法新增的接口）。

**参数说明<a name="section157501312135019"></a>**

无入参。

**返回值<a name="section49971832106"></a>**

<a name="table17997635100"></a>

| 数据类型 | 说明 |
| --- | --- |
| numpy.ndarray | 存储序列化内容的数组。 |

### deserialize\_from\_mem

**接口定义<a name="section172317194488"></a>**

def deserialize\_to\_mem\(serialize\_data: numpy.ndarray\) -\> int

**接口用途<a name="section1153124784912"></a>**

给定存储序列化内容的数组，还原一个检索器的索引实例（相比开源算法新增的接口）。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>

| 参数名称 | 数据类型 | 描述 | 取值范围 |
| --- | --- | --- | --- |
| serialize_data | numpy.ndarray | 存储序列化内容的数组。 | 限制非空。 |

**返回值<a name="section49971832106"></a>**

<a name="table17997635100"></a>

| 数据类型 | 说明 |
| --- | --- |
| int | 接口由底层C++接口封装而来，异常抛出由底层C++接口控制。 |

### get\_num

**接口定义<a name="section172317194488"></a>**

def get\_num\(\) -\> int

**接口用途<a name="section1153124784912"></a>**

获取底库向量的数量（相比开源算法新增的接口）。

**参数说明<a name="section157501312135019"></a>**

无入参。

**返回值<a name="section49971832106"></a>**

<a name="table17997635100"></a>

| 数据类型 | 说明 |
| --- | --- |
| int | 返回底库向量的数量。 |

### get\_dim

**接口定义<a name="section172317194488"></a>**

def get\_dim\(\) -\> int

**接口用途<a name="section1153124784912"></a>**

获取底库向量的维度（相比开源算法新增的接口）。

**参数说明<a name="section157501312135019"></a>**

无入参。

**返回值<a name="section49971832106"></a>**

<a name="table17997635100"></a>

| 数据类型 | 说明 |
| --- | --- |
| int | 返回底库向量的维度。 |

### create\_searcher

**接口定义<a name="section172317194488"></a>**

def create\_searcher\(db: numpy.ndarray, scann\_config: str, training\_threads: int, docids: numpy.ndarray, kmopt\_pq\_iter: int, kmopt\_pq\_sample: int, kmopt\_pq\_init: int, kmopt\_ivf\_iter: int, kmopt\_ivf\_sample: int, kmopt\_ivf\_init: int, filter\_thr: float, filter\_type: int\) -\> scann.scann\_ops.ScannSearcher

**接口用途<a name="section1153124784912"></a>**

基于入参构建索引并返回ScannSearcher（与开源算法相比增加filter\_thr和filter\_type参数）。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>

| 参数名称 | 数据类型 | 描述 | 取值范围 |
| --- | --- | --- | --- |
| db | numpy.ndarray | 底库向量。 | 限制非空。 |
| scann_config | 字符串 | 构建索引所需的配置文件，包含所有配置参数。 | - |
| training_threads | int | 设置用于索引构建的线程数。 | [0, MAXINT]，默认为0。 |
| docids | numpy.ndarray | 文档ID。 | 默认None |
| kmopt_pq_iter | int | PQ中Kmeans迭代次数。 | [0, MAXINT]，默认为0。 |
| kmopt_pq_sample | int | PQ中KMeans聚类采样子集大小。 | [0, MAXINT]，默认为0。 |
| kmopt_pq_init | int | PQ中KMeans初始化类型。 | {0,1,2,3}，默认为0。<br>1：基于“平均距离”初始化。<br>2：K-Means++ 初始化。<br>3：随机初始化。<br>0：不开启PQ中KMeans优化。 |
| kmopt_ivf_iter | int | IVF中Kmeans迭代次数。 | [0, MAXINT]，默认为0。 |
| kmopt_ivf_sample | int | IVF中KMeans聚类采样子集大小。 | [0, MAXINT]，默认为0。 |
| kmopt_ivf_init | int | IVF中KMeans初始化类型。 | {0,1,2,3}，默认为0。<br>1：基于“平均距离”初始化。<br>2：K-Means++ 初始化。<br>3：随机初始化。<br>0：不开启IVF中KMeans优化。 |
| filter_thr | float | 过滤阈值。 | [0, 1]，默认为0。 |
| filter_type | int | 过滤类型。 | 0 或 1，默认为0。<br>0：根据向量中0的元素个数进行过滤<br>1：根据向量中各个数与均值偏差大小进行过滤 |

**返回值<a name="section19841444181515"></a>**

<a name="table17997635100"></a>

| 数据类型 | 说明 |
| --- | --- |
| scann.scann_ops.ScannSearcher | 开始构建并返回构建好的ScannSearcher。 |

## C++接口

### 接口说明

KScaNN不提供对外接口，基于开源ScaNN算法做侵入式修改，对开源核心工具类ScannInterface里的类方法有新增。为获得最优性能，KScaNN接口内部不做完整入参校验，入参合法性由调用方业务来保证。KScaNN侵入式修改后的ScannInterface类方法如[**表 1** KScaNN修改后的ScannInterface类方法](#KScaNN修改后的ScannInterface类方法)所示。

**表 1** KScaNN修改后的ScannInterface类方法<a id="KScaNN修改后的ScannInterface类方法"></a>

<a name="table1194910128449"></a>

| 接口名称 | 接口作用 |
| --- | --- |
| SetNumThreads | 配置搜索时启用线程数（相比开源算法新增方法）。 |
| SearchAdditionalParams | 用于扩展ScaNN检索功能，提供额外的检索参数配置方法（相比开源算法新增方法）。 |
| Search | 单query搜索方法，单线程执行（与开源算法方法保持一致）。 |
| SearchBatched | 批量query搜索方法，单线程执行（与开源算法方法保持一致）。 |
| SearchBatchedParallel | 并行批量query搜索方法，多线程并发执行（与开源算法方法保持一致）。 |
| Initialize | 用于构建索引（与开源算法方法保持一致）。 |
| SerializeToMemory | 将索引序列化储存在内存中（相比开源算法新增方法）。 |
| LoadFromMemory | 从内存中还原索引实例（相比开源算法新增方法）。 |
| GetNum | 获取底库向量的数量（相比开源算法新增方法）。 |
| GetDim | 获取底库向量的维度（相比开源算法新增方法）。 |

### SetNumThreads

**接口定义<a name="section194415111419"></a>**

void ScannInterface::SetNumThreads\(int num\_threads\);

**接口用途<a name="section1153124784912"></a>**

配置搜索时启用线程数（相比开源算法新增方法）。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>

| 参数名称 | 数据类型 | 描述 | 取值范围 |
| --- | --- | --- | --- |
| num_threads | int | 线程数量。 | 大于等于2。推荐设置为运行时CPU核数。 |

### SearchAdditionalParams

**接口定义<a name="section172317194488"></a>**

void ScannInterface::SearchAdditionalParams\(float adp\_threshold, float refine\_prm, int adp\_refined, int leaves\_to\_search\);

**接口用途<a name="section1153124784912"></a>**

用于扩展ScaNN检索功能，提供额外的检索参数配置接口（相比开源算法新增方法）。应在索引构建后、检索前调用设置，接口参数具备缓存功能，一次设置，后续检索均生效。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>

| 参数名称 | 数据类型 | 描述 | 取值范围 |
| --- | --- | --- | --- |
| adp_threshold | float | 决策阈值，典型值0.3。 | [0.1, 0.8] |
| refine_prm | float | 精细化控制过滤策略，典型值0.2。 | [0.0, 1.0]，默认为0.0。值越大则过滤的子空间个数越少，精度越高，但性能会下降。 |
| adp_refined | int | 简单query所采用的子空间个数，典型值0，为训练自适应值（75分位点）。 | [0, leaves_to_search]，其中“leaves_to_search”表示复杂query所采用的子空间个数。 |
| leaves_to_search | int | 复杂query所采用的子空间个数，应与实际检索（Search*）接口参数一致。 | [1, num_leaves]，其中“num_leaves”表示IVF（Inverted File）倒排索引分区总子空间个数。 |

### Search

**接口定义<a name="section172317194488"></a>**

Status ScannInterface::Search\(const DatapointPtr<float\> query, NNResultsVector\* res, int final\_nn, int pre\_reorder\_nn, int leaves\) const;

**接口用途<a name="section1153124784912"></a>**

单query搜索接口，单线程执行（与开源算法方法保持一致）。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>

| 参数名称 | 数据类型 | 描述 | 取值范围 |
| --- | --- | --- | --- |
| query | `const DatapointPtr<float>` | Query。 | 限制非空。 |
| res | NNResultsVector* | 用于存储最终需要的结果（labals, distances），每一项长度为final_nn，其中“final_nn”为最终返回结果数量。 | 限制非空，长度为查询向量的数量。 |
| final_nn | int | 最终返回结果数量，TopK。 | 大于等于1，与构建时保持一致。 |
| pre_reorder_nn | int | 重排前保存结果数量。 | 大于等于final_nn，其中“final_nn”为最终返回结果数量。 |
| leaves | int | 搜索子空间数量。 | [1, n_leaves]，其中“n_leaves”为IVF倒排索引分区总子空间个数。 |

**返回值<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>

| 数据类型 | 说明 |
| --- | --- |
| Status | 表示方法执行状态，通过status.ok()判断是否成功。 |

### SearchBatched

**接口定义<a name="section172317194488"></a>**

Status ScannInterface::SearchBatched\(const DenseDataset<float\>& queries, MutableSpan<NNResultsVector\> res, int final\_nn, int pre\_reorder\_nn, int leaves\) const;

**接口用途<a name="section1153124784912"></a>**

批量query搜索接口，单线程执行（与开源算法方法保持一致）。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>

| 参数名称 | 数据类型 | 描述 | 取值范围 |
| --- | --- | --- | --- |
| queries | `const DatapointPtr<float>&` | 批次内的Queries。 | 限制非空。 |
| res | `MutableSpan<NNResultsVector>` | 用于存储最终需要的结果（labals, distances），每一项长度为final_nn，其中“final_nn”为最终返回结果数量。 | 限制非空，长度为查询向量的数量。 |
| final_nn | int | 最终返回结果数量，TopK。 | 大于等于1，与构建时保持一致。 |
| pre_reorder_nn | int | 重排前保存结果数量。 | 大于等于final_nn，其中“final_nn”为最终返回结果数量。 |
| leaves | int | 搜索子空间数量。 | [1, n_leaves]，其中“n_leaves”为IVF倒排索引分区总子空间个数。 |

**返回值<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>

| 数据类型 | 说明 |
| --- | --- |
| Status | 表示方法执行状态，通过status.ok()判断是否成功。 |

### SearchBatchedParallel

**接口定义<a name="section172317194488"></a>**

- Status ScannInterface::SearchBatchedParallel\(const DenseDataset<float\>& queries, MutableSpan<NNResultsVector\> res, int final\_nn, int pre\_reorder\_nn, int leaves, int batch\_size\) const;

- Status ScannInterface::SearchBatchedParallel\(const DenseDataset<float\>& queries, const std::vector<int64\_t\>& indices, MutableSpan<NNResultsVector\> res, int final\_nn, int pre\_reorder\_nn, int leaves, int batch\_size\) const;

**接口用途<a name="section1153124784912"></a>**

- 并行批量query搜索接口，多线程并发执行（与开源算法方法保持一致）。
- 并行批量query搜索重载函数，开启component filtering后需要引入过滤元素的索引列表（相比开源算法新增方法）。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>

| 参数名称 | 数据类型 | 描述 | 取值范围 |
| --- | --- | --- | --- |
| queries | `const DatapointPtr<float>&` | 批次内的Queries。 | 限制非空。 |
| res | `MutableSpan<NNResultsVector>` | 用于存储最终需要的结果（labals, distances），每一项长度为final_nn，其中“final_nn”为最终返回结果数量。 | 限制非空，长度为查询向量的数量。 |
| final_nn | int | 最终返回结果数量。 | 大于等于1，与构建时保持一致。 |
| pre_reorder_nn | int | 重排前保存结果数量。 | 大于等于final_nn，其中“final_nn”为最终返回结果数量。 |
| leaves | int | 搜索子空间数量。 | [1, n_leaves]，其中“n_leaves”为IVF倒排索引分区总子空间个数。 |
| indices | const std::vector<int64_t>& | 过滤元素的索引。 | 限制非空。 |
| batch_size | int | 批量搜索大小。 | [1, MAXINT]，默认为256。 |

**返回值<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>

| 数据类型 | 说明 |
| --- | --- |
| Status | 表示方法执行状态，通过status.ok()判断是否成功。 |

### Initialize

**接口定义<a name="section172317194488"></a>**

- Status ScannInterface::Initialize\(ConstSpan<float\> dataset, DatapointIndex n\_points, const std::string& config, int training\_threads\);
- Status ScannInterface::Initialize\(ConstSpan<float\> dataset, DatapointIndex n\_points, const std::string& config, int training\_threads, GmmUtils::KMeansParams kmOpt\);
- Status ScannInterface::Initialize\(ConstSpan<float\> dataset, DatapointIndex n\_points, const std::string& config, int training\_threads, GmmUtils::KMeansParams kmOpt, float filter\_thr, int filter\_type\);

**接口用途<a name="section1153124784912"></a>**

- 用于构建索引（与开源算法方法保持一致）。
- 用于构建索引，第2种Initialize重载函数，为IVF和PQ中的KMeans聚类设置额外参数用于调优（相比开源算法新增方法）。
- 用于构建索引，第3种Initialize重载函数，为IVF和PQ中的KMeans聚类和Component filtering设置额外参数（相比开源算法新增方法）。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>

| 参数名称 | 数据类型 | 描述 | 取值范围 |
| --- | --- | --- | --- |
| dataset | `ConstSpan<float>` | 底库向量。 | 限制非空。 |
| n_points | DatapointIndex | 底库向量的数量。 | 限制与dataset的长度保持一致，其中“dataset”表示底库向量。 |
| config | const std::string& | 构建索引所需的配置文件，包含所有配置参数。 | - |
| training_threads | int | 构建索引时的线程数。 | 大于等于1。 |
| kmOpt | GmmUtils::KMeansParams | 配置KMeans的调优参数。 | - |
| filter_thr | float | 过滤阈值。 | [0, 1]，默认为0。 |
| filter_type | int | 过滤类型。 | 0：根据向量中0的元素个数进行过滤。默认为0。<br>1：根据向量中各个数与均值偏差大小进行过滤。 |
| config_pbtxt | const std::string& | 加载索引所需的配置文件。 | - |
| scann_assets_pbtxt | const std::string& | 索引文件列表。 | - |

其中，“kmOpt“的结构体KMeansParams包含以下参数，参数说明如[**表 1** KMeansParams包含的参数说明](#KMeansParams包含的参数说明)所示。

```c++
struct KMeansTunableExtraParams {
        int32_t iter;
        int32_t sample;
        int32_t init; 
};

struct KMeansParams { 
        KMeansTunableExtraParams ivf; 
        KMeansTunableExtraParams pq; 
};
```

**表 1** KMeansParams包含的参数说明<a id="KMeansParams包含的参数说明"></a>

<a name="table11265104575315"></a>

| 参数名称 | 数据类型 | 描述 | 取值范围 |
| --- | --- | --- | --- |
| iter | int32_t | 表示K-Means算法的迭代次数。 | [0, MAXINT]，默认为0。 |
| sample | int32_t | 表示采样子集的大小。 | - |
| init | int32_t | 表示K-Means聚类中心的初始化方式。 | {0,1,2,3}，默认为0。<br>1：基于“平均距离”初始化。<br>2：K-Means++初始化。<br>3：随机初始化。<br>0：不开启PQ中KMeans优化。 |

“config“由create\_config.py结合如[**表 2** 参数说明](#参数说明)所示的参数生成。

**表 2** 参数说明<a id="参数说明"></a>

<a name="table7549205762512"></a>

| 参数名称 | 数据类型 | 描述 | 取值范围 |
| --- | --- | --- | --- |
| n_leaves | int | IVF分区总子空间个数。 | 大于等于1。 |
| nb | int32_t | 底库向量的数量。 | 限制与dataset的长度保持一致，其中“dataset”表示底库向量。 |
| metricType | std::string | 向量的距离类型。 | “dot_product”或“squared_l2” |
| dims_per_block | int | PQ量化合并维度数。 | [1, dim]，其中“dim”表示底库向量的维度。 |
| avq_threshold | float | 不对称分桶参数，仅对L2（squared_l2）数据集生效。 | [0,1] |
| dim | int32_t | 底库向量的维度。 | 限制与dataset的维度保持一致，其中“dataset”表示底库向量。 |
| topK | int | 最终返回结果数量。 | 大于等于1。 |
| soar_lambda | float | 控制正交性的参数，仅对IP（dot product）数据集生效。 | 大于0，当值为“-1”时表示不开启此参数。 |
| overretrieve_factor | float | 指定过检索因子，与“soar_lambda”一起使用，仅对IP（dot_product）数据集生效。 | [1,2]，当值为“-1”时表示不开启此参数。 |

>![note](public_sys-resources/icon-note.gif) **说明：** 
>“config“生成指令如下：
>
>```cpp
>python create_config.py  + std::to_string(n_leaves) + " "
>                         + std::to_string(nb) + " "
>                         + metricType + " "
>                         + std::to_string(dims_per_block) + " "
>                         + std::to_string(avq_threshold) + " "
>                         + std::to_string(dim) + " "
>                         + std::to_string(topK) + " "
>                         + std::to_string(soar_lambda) + " "
>                         + std::to_string(overretrieve_factor)
>```

**返回值<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>

| 数据类型 | 说明 |
| --- | --- |
| Status | 表示方法执行状态，通过status.ok()判断是否成功。 |

### SerializeToMemory

**接口定义<a name="section172317194488"></a>**

int ScannInterface::SerializeToMemory\(uint8\_t\*& dataPtr, size\_t& Length\);

**接口用途<a name="section1153124784912"></a>**

将索引序列化储存在内存中，内存长度为Length字节，起始地址为dataPtr（相比开源算法新增方法）。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>

| 参数名称 | 数据类型 | 描述 | 取值范围 |
| --- | --- | --- | --- |
| dataPtr | uint8_t*& | 指向存储序列化数据的内存的起始地址。 | 限制为空指针。 |
| Length | size_t& | 存储序列化数据的内存的长度。 | 限制为0。 |

**返回值<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>

| 数据类型 | 说明 |
| --- | --- |
| int | 执行成功返回0，否则返回-1。 |

### LoadFromMemory

**接口定义<a name="section172317194488"></a>**

int ScannInterface::LoadFromMemory\(uint8\_t\*& dataPtr, size\_t& Length\);

**接口用途<a name="section1153124784912"></a>**

从内存中还原索引实例（相比开源算法新增方法）。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>

| 参数名称 | 数据类型 | 描述 | 取值范围 |
| --- | --- | --- | --- |
| dataPtr | uint8_t*& | 指向存储序列化数据的内存的起始地址。 | 限制为非空指针。 |
| Length | size_t& | 存储序列化数据的内存的长度。 | 限制为非0。 |

**返回值<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>

| 数据类型 | 说明 |
| --- | --- |
| int | 执行成功返回0，否则返回-1。 |

### GetNum

**接口定义<a name="section172317194488"></a>**

int GetNum\(\) const;

**接口用途<a name="section1153124784912"></a>**

返回底库向量的数量（相比开源算法新增方法）。

**参数说明<a name="section157501312135019"></a>**

无入参。

**返回值<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>

| 数据类型 | 说明 |
| --- | --- |
| int | 返回底库向量的数量。 |

### GetDim

**接口定义<a name="section172317194488"></a>**

int GetDim\(\) const;

**接口用途<a name="section1153124784912"></a>**

返回底库向量的维度（相比开源算法新增方法）。

**参数说明<a name="section157501312135019"></a>**

无入参。

**返回值<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>

| 数据类型 | 说明 |
| --- | --- |
| int | 返回底库向量的维度。 |

## 修订记录

|文档版本|发布日期|修改说明|
|--|--|--|
|01|2025-12-30|第一次正式发布。|
