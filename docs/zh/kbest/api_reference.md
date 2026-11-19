# API参考

本文档介绍KBest向量检索库的C++与Python接口，提供构造函数、索引构建、检索、持久化等核心功能的API说明与使用示例，适用于需要集成向量检索功能的开发者。

## C++

### 接口说明

KBest提供的C++接口如[**表 1** KBest提供的C++接口](#KBest提供的C++接口)所示。

**表 1** KBest提供的C++接口<a id="KBest提供的C++接口"></a>

<a name="table1194910128449"></a>

| 接口名称 | 接口作用 |
| --- | --- |
| KBest | 初始化构建图检索（有参构造、无参构造）。 |
| Add | 构建图索引。 |
| BuildSearcher | 构建检索器。 |
| Search | 图检索。 |
| SetEf | 设置检索时的候选节点列表大小。 |
| Save | 保存检索器到指定路径。 |
| Load | 从指定路径加载检索器。 |
| SaveGraph | 保存图索引到指定路径。 |
| LoadGraph | 从指定路径加载图索引。 |
| Serialize | 将检索器内容存储至数组内。 |
| Deserialize | 还原数组内的检索器内容。 |
| GetNTotal | 返回图索引内的底库数据量。 |
| GetDim | 返回图索引内的数据维度。 |
| SetEarlyStoppingParams | 设置早停优化点参数。 |

### 构造函数（有参构造）

**接口定义<a name="section172317194488"></a>**

KBest\(int dim, int R, int L, int A, const char \*metric, const std::string &init\_builder\_type\);

KBest\(int dim, int R, int L, float A, int graph\_opt\_iter, const std::string &metric, const std::string &init\_builder\_type, const std::string &index\_type\);

**接口用途<a name="section1153124784912"></a>**

初始化构建图检索。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>

| 参数名称 | 数据类型 | 描述 | 取值范围 |
| --- | --- | --- | --- |
| dim | int | 特征维度。 | [1,2999] |
| R | int | 邻居节点数。 | [11,499] |
| L | int | 构图时的候选节点列表大小。 | [11,1999] |
| A | int | 构图剪枝时的角度阈值。 | [11,360] |
| metric | const char * | 距离度量的方式。 | “L2”或“IP”。<br>“L2”为欧几里得距离。<br>“IP”为内积距离。 |
| init_builder_type | const std::string & | 构建k近邻图的算法。 | “RNNDescent”或“NNDescent”，表示两种不同的构建k近邻图的算法，推荐使用“RNNDescent”。 |
| graph_opt_iter | int | 图索引自我迭代的轮数。 | [0,30] |
| index_type | const std::string & | 选择邻居策略。 | “HNSW”或“NSG”或“TSDG”或“SSG”，表示四种不同的选择邻居策略。 |

**使用示例**

```c++
#include <iostream>
#include "kbest.h"

int main() {
    // 参数配置
    int dim = 128;              // 特征维度
    int R = 32;                 // 邻居节点数
    int L = 200;                // 构图时的候选节点列表大小
    int A = 60;                 // 构图剪枝时的角度阈值
    int graph_opt_iter = 2;     // 图索引自我迭代轮数
    
    // 方式1：简单构造
    KBest index1(dim, R, L, A, "L2", "RNNDescent");
    std::cout << "方式1：成功创建KBest索引，维度: " << index1.GetDim() << std::endl;
    
    // 方式2：完整构造（推荐）
    KBest index2(dim, R, L, A, graph_opt_iter, "L2", "RNNDescent", "HNSW");
    std::cout << "方式2：成功创建KBest索引，维度: " << index2.GetDim() << std::endl;
    
    return 0;
}
```

### 构造函数（无参构造）

**接口定义<a name="section172317194488"></a>**

KBest\(\);

**接口用途<a name="section1153124784912"></a>**

无参数初始化构建图检索。

使用该接口创建的实例不能进行除Load/Deserialize/LoadGraph外的其他操作。调用除上述接口外的其他接口时，返回值为-1。

**参数说明<a name="section157501312135019"></a>**

无入参。

**使用示例**

```c++
#include <iostream>
#include "kbest.h"

int main() {
    // 无参构造，用于后续加载已保存的索引
    KBest index;
    
    // 从文件加载检索器
    int ret = index.Load("./saved_index.bin");
    if (ret == 0) {
        std::cout << "成功加载索引" << std::endl;
        std::cout << "数据维度: " << index.GetDim() << std::endl;
        std::cout << "底库数据量: " << index.GetNTotal() << std::endl;
    }
    
    return 0;
}
```

### Add

**接口定义<a name="section172317194488"></a>**

int Add\(int nb, const float \*xb, int consecutive, int level\);

int Add\(int nb, const float \*xb, int consecutive, int reorder, int level\);

**接口用途<a name="section1153124784912"></a>**

构建图索引。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>

| 参数名称 | 数据类型 | 描述 | 取值范围 |
| --- | --- | --- | --- |
| nb | int | 向量底库数据量。 | 大于等于1。建议小于10亿。 |
| xb | const float * | 向量底库数据。 | 限制非空，长度应为nb \* dim（数据量 \* 特征维度）。 |
| consecutive | int | 块大小。 | [1,31] |
| level | int | 控制量化的等级。 | [0,3]<br>0：表示FP32量化。<br>1：表示SQ8U量化。<br>2：表示SQ4U量化。<br>3：表示FP16量化。 |
| reorder | int | 是否开启底库向量重排。 | 0或1。 |

**返回值<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>

| 数据类型 | 说明 |
| --- | --- |
| int | 若参数超出取值范围则返回-1，在调用Load/Deserialize/LoadGraph后调用该接口时返回-1，否则返回0。 |

**使用示例**

```c++
#include <iostream>
#include <vector>
#include <cstdlib>
#include "kbest.h"

int main() {
    int dim = 128;
    int nb = 10000;  // 底库向量数量
    
    // 创建索引
    KBest index(dim, 32, 200, 60, 2, "L2", "RNNDescent", "HNSW");
    
    // 准备底库数据
    std::vector<float> xb(nb * dim);
    for (int i = 0; i < nb * dim; i++) {
        xb[i] = static_cast<float>(rand()) / RAND_MAX;
    }
    
    // 构建图索引
    int consecutive = 16;  // 块大小
    int reorder = 1;       // 开启底库向量重排
    int level = 0;         // 不量化（FP32）
    
    int ret = index.Add(nb, xb.data(), consecutive, reorder, level);
    
    if (ret == 0) {
        std::cout << "成功构建图索引" << std::endl;
        std::cout << "底库数据量: " << index.GetNTotal() << std::endl;
    } else {
        std::cout << "构建图索引失败，错误码: " << ret << std::endl;
    }
    
    return 0;
}
```

### BuildSearcher

**接口定义<a name="section172317194488"></a>**

int BuildSearcher\(\);

**接口用途<a name="section1153124784912"></a>**

使用调用Add接口时输入的level参数为量化参数，构建检索器。

**参数说明<a name="section157501312135019"></a>**

无入参。

**返回值<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>

| 数据类型 | 说明 |
| --- | --- |
| int | 在调用Load/Deserialize/LoadGraph后调用该接口时返回-1，检索器不改变。 |

**使用示例**

```c++
#include <iostream>
#include <vector>
#include "kbest.h"

int main() {
    int dim = 128;
    int nb = 10000;
    
    // 创建索引
    KBest index(dim, 32, 200, 60, 2, "L2", "RNNDescent", "HNSW");
    
    // 准备并添加底库数据
    std::vector<float> xb(nb * dim);
    for (int i = 0; i < nb * dim; i++) {
        xb[i] = static_cast<float>(rand()) / RAND_MAX;
    }
    index.Add(nb, xb.data(), 16, 1, 0);
    
    // 构建检索器
    int ret = index.BuildSearcher();
    
    if (ret == 0) {
        std::cout << "成功构建检索器，可以开始检索" << std::endl;
    } else {
        std::cout << "构建检索器失败" << std::endl;
    }
    
    return 0;
}
```

### Search

**接口定义<a name="section172317194488"></a>**

int Search\(int nq, const float \*xq, int topk, float \*distances, int64\_t \*labels, int num\_thread\);

**接口用途<a name="section1153124784912"></a>**

图检索。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>

| 参数名称 | 数据类型 | 描述 | 取值范围 |
| --- | --- | --- | --- |
| nq | int | 查询向量集数据量。 | 大于等于1。建议小于10亿。 |
| xq | const float * | 查询向量集数据。 | 限制非空，期待长度为nq \* dim（数据量 \* 特征维度）。 |
| topk | int | 最近邻的数量。 | [1,nb]，其中“nb”为向量底库数据量大小。 |
| distances | float * | 距离数组。 | 限制非空，期待长度为nq * topk。 |
| labels | int64_t * | 检索结果的ID数组。 | 限制非空，期待长度为nq * topk。 |
| num_thread | int | 检索时使用的线程数。 | [1,std::thread::hardware_concurrency()]，其中std::thread::hardware_concurrency()为当前系统支持的并发线程数。 |

**返回值<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>

| 数据类型 | 说明 |
| --- | --- |
| int | 若参数超出取值范围则返回-1；在调用BuildSearcher或Load/Deserialize/LoadGraph前调用该接口时返回-1；否则返回0。 |

**使用示例**

```c++
#include <iostream>
#include <vector>
#include "kbest.h"

int main() {
    int dim = 128;
    int nb = 10000;
    int nq = 10;     // 查询向量数量
    int topk = 5;    // 返回最近的5个邻居
    
    // 创建并构建索引
    KBest index(dim, 32, 200, 60, 2, "L2", "RNNDescent", "HNSW");
    
    std::vector<float> xb(nb * dim);
    for (int i = 0; i < nb * dim; i++) {
        xb[i] = static_cast<float>(rand()) / RAND_MAX;
    }
    index.Add(nb, xb.data(), 16, 1, 0);
    index.BuildSearcher();
    
    // 准备查询向量
    std::vector<float> xq(nq * dim);
    for (int i = 0; i < nq * dim; i++) {
        xq[i] = static_cast<float>(rand()) / RAND_MAX;
    }
    
    // 准备结果数组
    std::vector<float> distances(nq * topk);
    std::vector<int64_t> labels(nq * topk);
    
    // 执行检索
    int num_thread = 4;
    int ret = index.Search(nq, xq.data(), topk, distances.data(), labels.data(), num_thread);
    
    if (ret == 0) {
        std::cout << "检索成功" << std::endl;
        // 输出第一个查询向量的结果
        std::cout << "查询向量0的最近邻:" << std::endl;
        for (int i = 0; i < topk; i++) {
            std::cout << "  ID: " << labels[i] << ", 距离: " << distances[i] << std::endl;
        }
    }
    
    return 0;
}
```

### SetEf

**接口定义<a name="section172317194488"></a>**

int SetEf\(int ef\);

**接口用途<a name="section1153124784912"></a>**

设置检索时的候选节点列表大小。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>

| 参数名称 | 数据类型 | 描述 | 取值范围 |
| --- | --- | --- | --- |
| ef | int | 检索时的候选节点列表大小。 | [1,nb]，其中“nb”为向量底库数据量大小。 |

**返回值<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>

| 数据类型 | 说明 |
| --- | --- |
| int | 若参数超出取值范围则返回-1；在调用BuildSearcher或Load/Deserialize/LoadGraph前调用该接口时返回-1；否则返回0。 |

**使用示例**

```c++
#include <iostream>
#include <vector>
#include "kbest.h"

int main() {
    int dim = 128;
    int nb = 10000;
    
    // 创建并构建索引
    KBest index(dim, 32, 200, 60, 2, "L2", "RNNDescent", "HNSW");
    
    std::vector<float> xb(nb * dim);
    for (int i = 0; i < nb * dim; i++) {
        xb[i] = static_cast<float>(rand()) / RAND_MAX;
    }
    index.Add(nb, xb.data(), 16, 1, 0);
    index.BuildSearcher();
    
    // 设置较小的ef值（速度快，精度可能较低）
    index.SetEf(50);
    std::cout << "ef=50时进行检索..." << std::endl;
    
    // 设置较大的ef值（速度慢，精度更高）
    int ret = index.SetEf(200);
    if (ret == 0) {
        std::cout << "成功设置ef=200" << std::endl;
    }
    
    return 0;
}
```

### Save

**接口定义<a name="section172317194488"></a>**

int Save\(const char \*path\) const;

**接口用途<a name="section1153124784912"></a>**

单进程保存检索器到指定路径。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>

| 参数名称 | 数据类型 | 描述 | 取值范围 |
| --- | --- | --- | --- |
| path | const char * | 检索器的保存路径。 | 取值长度小于199字符。 |

**返回值<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>

| 数据类型 | 说明 |
| --- | --- |
| int | 若参数超出取值范围或存在保存路径错误等IO问题时返回-1；在调用BuildSearcher前调用该接口时返回-1；否则返回0。 |

**使用示例**

```c++
#include <iostream>
#include <vector>
#include "kbest.h"

int main() {
    int dim = 128;
    int nb = 10000;
    
    // 创建并构建索引
    KBest index(dim, 32, 200, 60, 2, "L2", "RNNDescent", "HNSW");
    
    std::vector<float> xb(nb * dim);
    for (int i = 0; i < nb * dim; i++) {
        xb[i] = static_cast<float>(rand()) / RAND_MAX;
    }
    index.Add(nb, xb.data(), 16, 1, 0);
    index.BuildSearcher();
    
    // 保存检索器
    int ret = index.Save("./kbest_index.bin");
    
    if (ret == 0) {
        std::cout << "成功保存检索器到 ./kbest_index.bin" << std::endl;
    } else {
        std::cout << "保存检索器失败" << std::endl;
    }
    
    return 0;
}
```

### Load

**接口定义<a name="section172317194488"></a>**

int Load\(const char \*path\);

**接口用途<a name="section1153124784912"></a>**

从指定路径加载检索器。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>

| 参数名称 | 数据类型 | 描述 | 取值范围 |
| --- | --- | --- | --- |
| path | const char * | 检索器的加载路径。 | 取值长度小于199字符。 |

**返回值<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>

| 数据类型 | 说明 |
| --- | --- |
| int | 若参数超出取值范围或存在读取路径错误等IO问题时返回-1；否则返回0。 |

**使用示例**

```c++
#include <iostream>
#include <vector>
#include "kbest.h"

int main() {
    // 使用无参构造创建索引实例
    KBest index;
    
    // 从文件加载检索器
    int ret = index.Load("./kbest_index.bin");
    
    if (ret == 0) {
        std::cout << "成功加载检索器" << std::endl;
        std::cout << "数据维度: " << index.GetDim() << std::endl;
        std::cout << "底库数据量: " << index.GetNTotal() << std::endl;
        
        // 加载后可直接进行检索
        int nq = 1;
        int topk = 5;
        int dim = index.GetDim();
        
        std::vector<float> xq(nq * dim);
        for (int i = 0; i < nq * dim; i++) {
            xq[i] = static_cast<float>(rand()) / RAND_MAX;
        }
        
        std::vector<float> distances(nq * topk);
        std::vector<int64_t> labels(nq * topk);
        
        index.Search(nq, xq.data(), topk, distances.data(), labels.data(), 4);
    } else {
        std::cout << "加载检索器失败" << std::endl;
    }
    
    return 0;
}
```

### SaveGraph

**接口定义<a name="section172317194488"></a>**

int SaveGraph\(const char \*path\) const;

**接口用途<a name="section1153124784912"></a>**

单进程保存图索引到指定路径。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>

| 参数名称 | 数据类型 | 描述 | 取值范围 |
| --- | --- | --- | --- |
| path | const char * | 图索引的保存路径。 | 取值长度小于199字符。 |

**返回值<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>

| 数据类型 | 说明 |
| --- | --- |
| int | 若参数超出取值范围或存在保存路径错误等IO问题时返回-1；调用Add接口前调用该接口时返回-1；调用BuildSearcher或Load/Deserialize/LoadGraph后调用该接口时返回-1；否则返回0。 |

**使用示例**

```c++
#include <iostream>
#include <vector>
#include "kbest.h"

int main() {
    int dim = 128;
    int nb = 10000;
    
    // 创建索引并添加数据
    KBest index(dim, 32, 200, 60, 2, "L2", "RNNDescent", "HNSW");
    
    std::vector<float> xb(nb * dim);
    for (int i = 0; i < nb * dim; i++) {
        xb[i] = static_cast<float>(rand()) / RAND_MAX;
    }
    index.Add(nb, xb.data(), 16, 1, 0);
    
    // 在调用BuildSearcher之前保存图索引
    int ret = index.SaveGraph("./kbest_graph.bin");
    
    if (ret == 0) {
        std::cout << "成功保存图索引到 ./kbest_graph.bin" << std::endl;
    } else {
        std::cout << "保存图索引失败" << std::endl;
    }
    
    return 0;
}
```

### LoadGraph

**接口定义<a name="section172317194488"></a>**

int LoadGraph\(const char \*path, int level\);

**接口用途<a name="section1153124784912"></a>**

从指定路径加载检索器。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>

| 参数名称 | 数据类型 | 描述 | 取值范围 |
| --- | --- | --- | --- |
| path | const char * | 检索器的加载路径。 | 取值长度小于199字符。 |
| level | int | 控制量化的等级。 | [-1,3]<br>-1：默认值，表示SaveGraph时保存的量化等级。<br>0：表示FP32量化。<br>1：表示SQ8U量化。<br>2：表示SQ4U量化。<br>3：表示FP16量化。 |

**返回值<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>

| 数据类型 | 说明 |
| --- | --- |
| int | 若参数超出取值范围或存在读取路径错误等IO问题时返回-1；否则返回0。 |

**使用示例**

```c++
#include <iostream>
#include <vector>
#include "kbest.h"

int main() {
    // 使用无参构造创建索引实例
    KBest index;
    
    // 从文件加载图索引，使用保存时的量化等级
    int ret = index.LoadGraph("./kbest_graph.bin", -1);
    
    if (ret == 0) {
        std::cout << "成功加载图索引" << std::endl;
        std::cout << "数据维度: " << index.GetDim() << std::endl;
        std::cout << "底库数据量: " << index.GetNTotal() << std::endl;
        
        // 加载后可直接进行检索
        int nq = 1;
        int topk = 5;
        int dim = index.GetDim();
        
        std::vector<float> xq(nq * dim);
        for (int i = 0; i < nq * dim; i++) {
            xq[i] = static_cast<float>(rand()) / RAND_MAX;
        }
        
        std::vector<float> distances(nq * topk);
        std::vector<int64_t> labels(nq * topk);
        
        index.Search(nq, xq.data(), topk, distances.data(), labels.data(), 4);
    }
    
    return 0;
}
```

### Serialize

**接口定义<a name="section172317194488"></a>**

int Serialize\(uint8\_t \*&dataPtr, size\_t &dataLength\) const;

**接口用途<a name="section1153124784912"></a>**

将检索器内容存储至长度为dataLength字节的起始地址为dataPtr的uint8数组内。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>

| 参数名称 | 数据类型 | 描述 | 取值范围 |
| --- | --- | --- | --- |
| dataPtr | uint8_t *& | 存储检索器内容的数组的起始地址。 | 限制为空指针。 |
| dataLength | size_t & | 存储检索器内容的数组的长度。 | 限制为0。 |

**返回值<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>

| 数据类型 | 说明 |
| --- | --- |
| int | 若参数超出取值范围时返回-1；调用BuildSearcher或Load/Deserialize/LoadGraph后调用该接口时返回-1；否则返回0。 |

**使用示例**

```c++
#include <iostream>
#include <vector>
#include "kbest.h"

int main() {
    int dim = 128;
    int nb = 10000;
    
    // 创建索引并添加数据
    KBest index(dim, 32, 200, 60, 2, "L2", "RNNDescent", "HNSW");
    
    std::vector<float> xb(nb * dim);
    for (int i = 0; i < nb * dim; i++) {
        xb[i] = static_cast<float>(rand()) / RAND_MAX;
    }
    index.Add(nb, xb.data(), 16, 1, 0);
    
    // 序列化检索器内容到数组
    uint8_t* dataPtr = nullptr;
    size_t dataLength = 0;
    
    int ret = index.Serialize(dataPtr, dataLength);
    
    if (ret == 0) {
        std::cout << "序列化成功，数据长度: " << dataLength << " 字节" << std::endl;
        
        // ... 可以将dataPtr中的数据存储到数据库 ...
        
        // 使用完毕后释放内存
        delete[] dataPtr;
    }
    
    return 0;
}
```

### Deserialize

**接口定义<a name="section172317194488"></a>**

int Deserialize\(const uint8\_t \*dataPtr, const size\_t &dataLength\);

**接口用途<a name="section1153124784912"></a>**

给定填充检索器内容的数组dataPtr和数组长度dataLength，还原一个待检索的索引实例。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>

| 参数名称 | 数据类型 | 描述 | 取值范围 |
| --- | --- | --- | --- |
| dataPtr | const uint8_t * | 存储检索器内容的数组的起始地址。 | 限制非空。 |
| dataLength | const size_t & | 存储检索器内容的数组的长度。 | 限制为Serialize接口时保存的数组长度。 |

**返回值<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>

| 数据类型 | 说明 |
| --- | --- |
| int | 若参数超出取值范围时返回-1；否则返回0。<br>Serialize接口内部申请数组内存，请在调用本接口后使用delete []释放该资源。 |

**使用示例**

```c++
#include <iostream>
#include <vector>
#include "kbest.h"

int main() {
    int dim = 128;
    int nb = 10000;
    
    // 创建索引并序列化
    KBest index1(dim, 32, 200, 60, 2, "L2", "RNNDescent", "HNSW");
    
    std::vector<float> xb(nb * dim);
    for (int i = 0; i < nb * dim; i++) {
        xb[i] = static_cast<float>(rand()) / RAND_MAX;
    }
    index1.Add(nb, xb.data(), 16, 1, 0);
    
    uint8_t* dataPtr = nullptr;
    size_t dataLength = 0;
    index1.Serialize(dataPtr, dataLength);
    
    // 使用序列化数据还原索引
    KBest index2;
    int ret = index2.Deserialize(dataPtr, dataLength);
    
    if (ret == 0) {
        std::cout << "反序列化成功" << std::endl;
        std::cout << "还原后的索引维度: " << index2.GetDim() << std::endl;
        std::cout << "还原后的底库数据量: " << index2.GetNTotal() << std::endl;
        
        // 反序列化后可直接进行检索
    }
    
    // 释放序列化时申请的内存
    delete[] dataPtr;
    
    return 0;
}
```

### GetNTotal

**接口定义<a name="section172317194488"></a>**

int GetNTotal\(\) const;

**接口用途<a name="section1153124784912"></a>**

返回此时图索引内的底库数据量。

**参数说明<a name="section1521117111210"></a>**

无入参

**返回值<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>

| 数据类型 | 说明 |
| --- | --- |
| int | 不添加底库的场景下，默认返回值为0。 |

**使用示例**

```c++
#include <iostream>
#include <vector>
#include "kbest.h"

int main() {
    int dim = 128;
    int nb = 10000;
    
    KBest index(dim, 32, 200, 60, 2, "L2", "RNNDescent", "HNSW");
    
    // 添加数据前
    std::cout << "添加数据前，底库数据量: " << index.GetNTotal() << std::endl;
    
    // 添加数据
    std::vector<float> xb(nb * dim);
    for (int i = 0; i < nb * dim; i++) {
        xb[i] = static_cast<float>(rand()) / RAND_MAX;
    }
    index.Add(nb, xb.data(), 16, 1, 0);
    
    // 添加数据后
    std::cout << "添加数据后，底库数据量: " << index.GetNTotal() << std::endl;
    
    return 0;
}
```

### GetDim

**接口定义<a name="section172317194488"></a>**

int GetDim\(\) const;

**接口用途<a name="section1153124784912"></a>**

返回此时图索引内的数据维度。

**参数说明<a name="section1521117111210"></a>**

无入参

**返回值<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>

| 数据类型 | 说明 |
| --- | --- |
| int | 有参构建的场景下等于“dim”参数，无参构建的场景或有参构建后调用Load/Deserialize/LoadGraph接口后，返回值为读取的检索器/图索引中的数据的维度。 |

**使用示例**

```c++
#include <iostream>
#include "kbest.h"

int main() {
    int dim = 128;
    
    // 有参构造
    KBest index1(dim, 32, 200, 60, 2, "L2", "RNNDescent", "HNSW");
    std::cout << "有参构造后的维度: " << index1.GetDim() << std::endl;
    
    // 无参构造后加载
    KBest index2;
    index2.Load("./kbest_index.bin");
    std::cout << "从文件加载后的维度: " << index2.GetDim() << std::endl;
    
    return 0;
}
```

### SetEarlyStoppingParams

**接口定义<a name="section172317194488"></a>**

int SetEarlyStoppingParams\(int32\_t adding\_pref, int32\_t patience\)

**接口用途<a name="section1153124784912"></a>**

设置早停参数。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>

| 参数名称 | 数据类型 | 描述 | 取值范围 |
| --- | --- | --- | --- |
| adding_pref | int | 超参候选集插入阈值。 | 大于等于1。 |
| patience | int | 检索耐心值。 | 大于等于1。 |

**返回值<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>

| 数据类型 | 说明 |
| --- | --- |
| int | 若参数超出取值范围时返回-1；调用BuildSearcher或Load/Deserialize/LoadGraph后调用该接口时返回-1；否则返回0。 |

**使用示例**

```c++
#include <iostream>
#include <vector>
#include "kbest.h"

int main() {
    int dim = 128;
    int nb = 10000;
    
    KBest index(dim, 32, 200, 60, 2, "L2", "RNNDescent", "HNSW");
    
    std::vector<float> xb(nb * dim);
    for (int i = 0; i < nb * dim; i++) {
        xb[i] = static_cast<float>(rand()) / RAND_MAX;
    }
    index.Add(nb, xb.data(), 16, 1, 0);
    
    // 设置早停参数（在BuildSearcher之前调用）
    int adding_pref = 5;   // 超参候选集插入阈值
    int patience = 10;     // 检索耐心值
    
    int ret = index.SetEarlyStoppingParams(adding_pref, patience);
    
    if (ret == 0) {
        std::cout << "成功设置早停参数" << std::endl;
    }
    
    // 然后构建检索器
    index.BuildSearcher();
    
    return 0;
}
```

## Python

### 接口说明

KBest提供的Python接口如[**表 1** KBest提供的Python接口](#KBest提供的Python接口)所示。

**表 1** KBest提供的Python接口<a id="KBest提供的Python接口"></a>

<a name="table1194910128449"></a>

| 接口名称 | 接口作用 |
| --- | --- |
| KBest | 初始化构建图检索（有参构造、无参构造）。 |
| add | 构建图索引。 |
| buildSearcher | 构建检索器。 |
| search | 图检索。 |
| setEf | 设置检索时的候选节点列表大小。 |
| save | 保存检索器到指定路径。 |
| load | 从指定路径加载检索器。 |
| saveGraph | 保存图索引到指定路径。 |
| loadGraph | 从指定路径加载图索引。 |
| serialize | 将检索器内容存储至数组内。 |
| deserialize | 还原数组内的检索器内容。 |
| getNTotal | 返回图索引内的底库数据量。 |
| getDim | 返回图索引内的数据维度。 |
| setEarlyStoppingParams | 设置早停优化点参数。 |

### 构造函数（有参构造）

**接口定义<a name="section172317194488"></a>**

class KBest\(dim: int, R: int, L: int, A: int, graph\_opt\_iter:int, metric: string, init\_builder\_type: string, index\_type: string, numa\_enabled: bool, numa\_nodes\_number: int\)

**接口用途<a name="section1153124784912"></a>**

初始化构建图检索。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>

| 参数名称 | 数据类型 | 描述 | 取值范围 |
| --- | --- | --- | --- |
| dim | int | 特征维度。 | [1,2999] |
| R | int | 邻居节点数。 | [11,499] |
| L | int | 构图时的候选节点列表大小。 | [11,1999] |
| A | int | 构图剪枝时的角度阈值。 | [11,360] |
| graph_opt_iter | int | 图索引自我迭代的轮数。 | [0,30] |
| metric | 字符串 | 距离度量的方式。其中， | “L2”或“IP”。<br>“L2”为欧几里得距离。<br>“IP”为内积距离。 |
| init_builder_type | 字符串 | 构建k近邻图的算法。 | “RNNDescent”和“NNDescent”，表示两种不同的构建k近邻图的算法，推荐使用“RNNDescent”。 |
| index_type | 字符串 | 选择邻居策略。 | “HNSW”或“NSG”或“TSDG”或“SSG”，表示四种不同的选择邻居策略。 |
| numa_enabled | 布尔值 | 是否开启NUMA优化。 | - |
| numa_nodes_number | int | 使用的NUMA节点数量。 | 大于等于1。 |

**使用示例**

```python
import numpy as np
import kbest

# 参数配置
dim = 128              # 特征维度
R = 32                 # 邻居节点数
L = 200                # 构图时的候选节点列表大小
A = 60                 # 构图剪枝时的角度阈值
graph_opt_iter = 2     # 图索引自我迭代轮数

# 创建索引（不使用NUMA优化）
index = kbest.KBest(dim, R, L, A, graph_opt_iter, "L2", "RNNDescent", "HNSW", False, 1)

print(f"成功创建KBest索引，维度: {index.getDim()}")
```

### 构造函数（无参构造）

**接口定义<a name="section172317194488"></a>**

class KBest\(\)

**接口用途<a name="section1153124784912"></a>**

无参数初始化构建图检索。

**参数说明<a name="section157501312135019"></a>**

无入参。

**使用示例**

```python
import kbest

# 无参构造，用于后续加载已保存的索引
index = kbest.KBest()

# 从文件加载检索器
ret = index.load("./saved_index.bin")
if ret == 0:
    print("成功加载索引")
    print(f"数据维度: {index.getDim()}")
    print(f"底库数据量: {index.getNTotal()}")
```

### add

**接口定义<a name="section172317194488"></a>**

def add\(nb:int, xb: numpy.ndarray, consecutive: int, reorder: int, level: int\) -\> int

**接口用途<a name="section1153124784912"></a>**

构建图索引。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>

| 参数名称 | 数据类型 | 描述 | 取值范围 |
| --- | --- | --- | --- |
| nb | int | 向量底库数据量。 | 大于等于1。建议小于10亿。 |
| xb | numpy.ndarray | 向量底库数据。 | 限制非空，长度应为nb \* dim（数据量 \* 特征维度）。 |
| consecutive | int | 块大小。 | [1,31] |
| reorder | int | 是否开启底库向量重排。 | 0或1。 |
| level | int | 控制量化的等级。 | [0,3]<br>0：表示FP32量化。<br>1：表示SQ8U量化。<br>2：表示SQ4U量化。<br>3：表示FP16量化。 |

**返回值<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>

| 数据类型 | 说明 |
| --- | --- |
| int | 接口由底层C++接口封装而来。异常抛出由底层C++接口控制。 |

**使用示例**

```python
import numpy as np
import kbest

dim = 128
nb = 10000  # 底库向量数量

# 创建索引
index = kbest.KBest(dim, 32, 200, 60, 2, "L2", "RNNDescent", "HNSW", False, 1)

# 准备底库数据
xb = np.random.random((nb, dim)).astype(np.float32)

# 构建图索引
consecutive = 16  # 块大小
reorder = 1       # 开启底库向量重排
level = 0         # FP32量化

ret = index.add(nb, xb, consecutive, reorder, level)

if ret == 0:
    print("成功构建图索引")
    print(f"底库数据量: {index.getNTotal()}")
else:
    print(f"构建图索引失败，错误码: {ret}")
```

### buildSearcher

**接口定义<a name="section172317194488"></a>**

def buildSearcher\(\) -\> int

**接口用途<a name="section1153124784912"></a>**

使用调用add接口时输入的level参数为量化参数，构建检索器。

**参数说明<a name="section157501312135019"></a>**

无入参。

**返回值<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>

| 数据类型 | 说明 |
| --- | --- |
| int | 接口由底层C++接口封装而来，异常抛出由底层C++接口控制。 |

**使用示例**

```python
import numpy as np
import kbest

dim = 128
nb = 10000

# 创建索引
index = kbest.KBest(dim, 32, 200, 60, 2, "L2", "RNNDescent", "HNSW", False, 1)

# 添加底库数据
xb = np.random.random((nb, dim)).astype(np.float32)
index.add(nb, xb, 16, 1, 0)

# 构建检索器
ret = index.buildSearcher()

if ret == 0:
    print("成功构建检索器，可以开始检索")
else:
    print("构建检索器失败")
```

### search<a name="ZH-CN_TOPIC_0000002549873553"></a>

**接口定义<a name="section172317194488"></a>**

def search\(nq: int, xq: numpy.ndarray, topk: int, distances: numpy.ndarray, labels: numpy.ndarray, num\_threads: int\) -\> int

**接口用途<a name="section1153124784912"></a>**

图检索。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>

| 参数名称 | 数据类型 | 描述 | 取值范围 |
| --- | --- | --- | --- |
| nq | int | 查询向量集数据量。 | 大于等于1。建议小于10亿。 |
| xq | numpy.ndarray | 查询向量集数据。 | 限制非空，期待长度为nq \* dim（数据量 \* 特征维度）。 |
| topk | int | 最近邻的数量。 | [1,nb]，其中“nb”为向量底库数据量大小。 |
| distances | numpy.ndarray | 距离数组。 | 限制非空，期待长度为nq \* topk。 |
| labels | numpy.ndarray | 检索结果的ID数组。 | 限制非空，期待长度为nq \* topk。 |
| num_threads | int | 检索时使用的线程数。 | [1,std::thread::hardware_concurrency()]，其中std::thread::hardware_concurrency()为当前系统支持的并发线程数。 |

**返回值<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>

| 数据类型 | 说明 |
| --- | --- |
| int | 接口由底层C++接口封装而来，异常抛出由底层C++接口控制。 |

**使用示例**

```python
import numpy as np
import kbest

dim = 128
nb = 10000
nq = 10      # 查询向量数量
topk = 5     # 返回最近的5个邻居

# 创建并构建索引
index = kbest.KBest(dim, 32, 200, 60, 2, "L2", "RNNDescent", "HNSW", False, 1)

xb = np.random.random((nb, dim)).astype(np.float32)
index.add(nb, xb, 16, 1, 0)
index.buildSearcher()

# 准备查询向量
xq = np.random.random((nq, dim)).astype(np.float32)

# 准备结果数组
distances = np.zeros((nq, topk), dtype=np.float32)
labels = np.zeros((nq, topk), dtype=np.int64)

# 执行检索
num_threads = 4
ret = index.search(nq, xq, topk, distances, labels, num_threads)

if ret == 0:
    print("检索成功")
    print(f"查询向量0的最近邻:")
    for i in range(topk):
        print(f"  ID: {labels[0, i]}, 距离: {distances[0, i]}")
```

### setEf

**接口定义<a name="section172317194488"></a>**

def setEf\(ef: int\) -\> int

**接口用途<a name="section1153124784912"></a>**

设置检索时的候选节点列表大小。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>

| 参数名称 | 数据类型 | 描述 | 取值范围 |
| --- | --- | --- | --- |
| ef | int | 检索时的候选节点列表大小。 | [1,nb]，其中“nb”为向量底库数据量大小。 |

**返回值<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>

| 数据类型 | 说明 |
| --- | --- |
| int | 接口由底层C++接口封装而来，异常抛出由底层C++接口控制。 |

**使用示例**

```python
import numpy as np
import kbest

dim = 128
nb = 10000

# 创建并构建索引
index = kbest.KBest(dim, 32, 200, 60, 2, "L2", "RNNDescent", "HNSW", False, 1)

xb = np.random.random((nb, dim)).astype(np.float32)
index.add(nb, xb, 16, 1, 0)
index.buildSearcher()

# 设置较小的ef值（速度快，精度可能较低）
index.setEf(50)
print("ef=50时进行检索...")

# 设置较大的ef值（速度慢，精度更高）
ret = index.setEf(200)
if ret == 0:
    print("成功设置ef=200")
```

### save

**接口定义<a name="section172317194488"></a>**

def save\(path: string\) -\> int

**接口用途<a name="section1153124784912"></a>**

单进程保存检索器到指定路径。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>

| 参数名称 | 数据类型 | 描述 | 取值范围 |
| --- | --- | --- | --- |
| path | 字符串 | 检索器的保存路径。 | 取值长度小于199字符。 |

**返回值<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>

| 数据类型 | 说明 |
| --- | --- |
| int | 接口由底层C++接口封装而来，异常抛出由底层C++接口控制。 |

**使用示例**

```python
import numpy as np
import kbest

dim = 128
nb = 10000

# 创建并构建索引
index = kbest.KBest(dim, 32, 200, 60, 2, "L2", "RNNDescent", "HNSW", False, 1)

xb = np.random.random((nb, dim)).astype(np.float32)
index.add(nb, xb, 16, 1, 0)
index.buildSearcher()

# 保存检索器
ret = index.save("./kbest_index.bin")

if ret == 0:
    print("成功保存检索器到 ./kbest_index.bin")
else:
    print("保存检索器失败")
```

### load

**接口定义<a name="section172317194488"></a>**

def load\(path: string\) -\> int

**接口用途<a name="section1153124784912"></a>**

从指定路径加载检索器。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>

| 参数名称 | 数据类型 | 描述 | 取值范围 |
| --- | --- | --- | --- |
| path | 字符串 | 检索器的加载路径。 | 取值长度小于199字符。 |

**返回值<a name="section49971832106"></a>**

<a name="table17997635100"></a>

| 数据类型 | 说明 |
| --- | --- |
| int | 接口由底层C++接口封装而来，异常抛出由底层C++接口控制。 |

**使用示例**

```python
import numpy as np
import kbest

# 使用无参构造创建索引实例
index = kbest.KBest()

# 从文件加载检索器
ret = index.load("./kbest_index.bin")

if ret == 0:
    print("成功加载检索器")
    print(f"数据维度: {index.getDim()}")
    print(f"底库数据量: {index.getNTotal()}")
    
    # 加载后可直接进行检索
    nq = 1
    topk = 5
    dim = index.getDim()
    
    xq = np.random.random((nq, dim)).astype(np.float32)
    distances = np.zeros((nq, topk), dtype=np.float32)
    labels = np.zeros((nq, topk), dtype=np.int64)
    
    index.search(nq, xq, topk, distances, labels, 4)
else:
    print("加载检索器失败")
```

### saveGraph

**接口定义<a name="section172317194488"></a>**

def saveGraph\(path: string\) -\> int

**接口用途<a name="section1153124784912"></a>**

单进程保存图索引到指定路径。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>

| 参数名称 | 数据类型 | 描述 | 取值范围 |
| --- | --- | --- | --- |
| path | 字符串 | 图索引的保存路径。 | 取值长度小于199字符。 |

**返回值<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>

| 数据类型 | 说明 |
| --- | --- |
| int | 接口由底层C++接口封装而来，异常抛出由底层C++接口控制。 |

**使用示例**

```python
import numpy as np
import kbest

dim = 128
nb = 10000

# 创建索引并添加数据
index = kbest.KBest(dim, 32, 200, 60, 2, "L2", "RNNDescent", "HNSW", False, 1)

xb = np.random.random((nb, dim)).astype(np.float32)
index.add(nb, xb, 16, 1, 0)

# 在调用buildSearcher之前保存图索引
ret = index.saveGraph("./kbest_graph.bin")

if ret == 0:
    print("成功保存图索引到 ./kbest_graph.bin")
else:
    print("保存图索引失败")
```

### loadGraph

**接口定义<a name="section172317194488"></a>**

def load\(path: string, level: int\) -\> int

**接口用途<a name="section1153124784912"></a>**

从指定路径加载检索器。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>

| 参数名称 | 数据类型 | 描述 | 取值范围 |
| --- | --- | --- | --- |
| path | 字符串 | 检索器的加载路径。 | 取值长度小于199字符。 |
| level | int | 控制量化的等级。 | [-1,3]<br>-1：默认值，表示saveGraph时保存的量化等级。<br>0：表示FP32量化。<br>1：表示SQ8U量化。<br>2：表示SQ4U量化。<br>3：表示FP16量化。 |

**返回值<a name="section49971832106"></a>**

<a name="table17997635100"></a>

| 数据类型 | 说明 |
| --- | --- |
| int | 接口由底层C++接口封装而来，异常抛出由底层C++接口控制。 |

**使用示例**

```python
import numpy as np
import kbest

# 使用无参构造创建索引实例
index = kbest.KBest()

# 从文件加载图索引，使用保存时的量化等级
ret = index.loadGraph("./kbest_graph.bin", -1)

if ret == 0:
    print("成功加载图索引")
    print(f"数据维度: {index.getDim()}")
    print(f"底库数据量: {index.getNTotal()}")
    
    # 加载后可直接进行检索
    nq = 1
    topk = 5
    dim = index.getDim()
    
    xq = np.random.random((nq, dim)).astype(np.float32)
    distances = np.zeros((nq, topk), dtype=np.float32)
    labels = np.zeros((nq, topk), dtype=np.int64)
    
    index.search(nq, xq, topk, distances, labels, 4)
```

### serialize

**接口定义<a name="section172317194488"></a>**

def serialize\(\) -\> numpy.ndarray

**接口用途<a name="section1153124784912"></a>**

将检索器内容存储至数组内。

**参数说明<a name="section157501312135019"></a>**

无入参。

**返回值<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>

| 数据类型 | 说明 |
| --- | --- |
| numpy.ndarray | 存储检索器内容的数组。 |

**使用示例**

```python
import numpy as np
import kbest

dim = 128
nb = 10000

# 创建索引并添加数据
index = kbest.KBest(dim, 32, 200, 60, 2, "L2", "RNNDescent", "HNSW", False, 1)

xb = np.random.random((nb, dim)).astype(np.float32)
index.add(nb, xb, 16, 1, 0)

# 序列化检索器内容到数组
data_arr = index.serialize()

print(f"序列化成功，数据长度: {len(data_arr)} 字节")

# 可以将data_arr存储到数据库
```

### deserialize

**接口定义<a name="section172317194488"></a>**

def deserialize\(data\_arr: numpy.ndarray\) -\> int

**接口用途<a name="section1153124784912"></a>**

给定填充检索器内容的数组，还原一个待检索的索引实例。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>

| 参数名称 | 数据类型 | 描述 | 取值范围 |
| --- | --- | --- | --- |
| data_arr | numpy.ndarray | 存储检索器内容的数组。 | 存储检索器内容的数组的起始地址限制非空，存储检索器内容的数组的长度限制为serialize接口时保存的数组长度。 |

**返回值<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>

| 数据类型 | 说明 |
| --- | --- |
| int | 接口由底层C++接口封装而来，异常抛出由底层C++接口控制。 |

**使用示例**

```python
import numpy as np
import kbest

dim = 128
nb = 10000

# 创建索引并序列化
index1 = kbest.KBest(dim, 32, 200, 60, 2, "L2", "RNNDescent", "HNSW", False, 1)

xb = np.random.random((nb, dim)).astype(np.float32)
index1.add(nb, xb, 16, 1, 0)

data_arr = index1.serialize()

# 使用序列化数据还原索引
index2 = kbest.KBest()
ret = index2.deserialize(data_arr)

if ret == 0:
    print("反序列化成功")
    print(f"还原后的索引维度: {index2.getDim()}")
    print(f"还原后的底库数据量: {index2.getNTotal()}")
```

### getNTotal

**接口定义<a name="section172317194488"></a>**

def getNTotal\(\) -\> int

**接口用途<a name="section1153124784912"></a>**

返回此时图索引内的底库数据量。

**参数说明<a name="section1521117111210"></a>**

无入参。

**返回值<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>

| 数据类型 | 说明 |
| --- | --- |
| int | 不添加底库的场景下，默认返回值为0。 |

**使用示例**

```python
import numpy as np
import kbest

dim = 128
nb = 10000

index = kbest.KBest(dim, 32, 200, 60, 2, "L2", "RNNDescent", "HNSW", False, 1)

# 添加数据前
print(f"添加数据前，底库数据量: {index.getNTotal()}")

# 添加数据
xb = np.random.random((nb, dim)).astype(np.float32)
index.add(nb, xb, 16, 1, 0)

# 添加数据后
print(f"添加数据后，底库数据量: {index.getNTotal()}")
```

### getDim

**接口定义<a name="section172317194488"></a>**

def getDim\(\) -\> int

**接口用途<a name="section1153124784912"></a>**

返回此时图索引内的数据维度。

**参数说明<a name="section1521117111210"></a>**

无入参。

**返回值<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>

| 数据类型 | 说明 |
| --- | --- |
| int | 有参构建的场景下等于<span class="parmname" id="parmname8531896718"><a name="parmname8531896718"></a>“dim”</span>参数，无参构建的场景或有参构建后调用load/deserialize/loadGraph接口后，返回值为读取的检索器/图索引中的数据的维度。 |

**使用示例**

```python
import kbest

dim = 128

# 有参构造
index1 = kbest.KBest(dim, 32, 200, 60, 2, "L2", "RNNDescent", "HNSW", False, 1)
print(f"有参构造后的维度: {index1.getDim()}")

# 无参构造后加载
index2 = kbest.KBest()
index2.load("./kbest_index.bin")
print(f"从文件加载后的维度: {index2.getDim()}")
```

### setEarlyStoppingParams

**接口定义<a name="section172317194488"></a>**

def setEarlyStoppingParams\(adding\_pref: int, patience: int\) -\> int

**接口用途<a name="section1153124784912"></a>**

设置早停参数。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>

| 参数名称 | 数据类型 | 描述 | 取值范围 |
| --- | --- | --- | --- |
| adding_pref | int | 超参候选集插入阈值。 | 大于等于1。 |
| patience | int | 检索耐心值。 | 大于等于1。 |

**返回值<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>

| 数据类型 | 说明 |
| --- | --- |
| int | 接口由底层C++接口封装而来，异常抛出由底层C++接口控制。 |

**使用示例**

```python
import numpy as np
import kbest

dim = 128
nb = 10000

index = kbest.KBest(dim, 32, 200, 60, 2, "L2", "RNNDescent", "HNSW", False, 1)

xb = np.random.random((nb, dim)).astype(np.float32)
index.add(nb, xb, 16, 1, 0)

# 设置早停参数（在buildSearcher之前调用）
adding_pref = 5   # 超参候选集插入阈值
patience = 10     # 检索耐心值

ret = index.setEarlyStoppingParams(adding_pref, patience)

if ret == 0:
    print("成功设置早停参数")

# 然后构建检索器
index.buildSearcher()
```

## 修订记录

|文档版本|发布日期|修改说明|
|--|--|--|
|01|2025-12-30|第一次正式发布。|
