# API参考

## C++

### 接口说明

KBest提供的C++接口如[**表 1** KBest提供的C++接口](#KBest提供的C++接口)所示。

**表 1** KBest提供的C++接口<a id="KBest提供的C++接口"></a>

<a name="table1194910128449"></a>
<table><thead align="left"><tr id="row99491812134412"><th class="cellrowborder" valign="top" width="34.38%" id="mcps1.2.3.1.1"><p id="p1794951224415"><a name="p1794951224415"></a><a name="p1794951224415"></a>接口名称</p>
</th>
<th class="cellrowborder" valign="top" width="65.62%" id="mcps1.2.3.1.2"><p id="p6949612124415"><a name="p6949612124415"></a><a name="p6949612124415"></a>接口作用</p>
</th>
</tr>
</thead>
<tbody><tr id="row119491112174414"><td class="cellrowborder" valign="top" width="34.38%" headers="mcps1.2.3.1.1 "><p id="p1494931224410"><a name="p1494931224410"></a><a name="p1494931224410"></a>KBest</p>
</td>
<td class="cellrowborder" valign="top" width="65.62%" headers="mcps1.2.3.1.2 "><p id="p3949012174411"><a name="p3949012174411"></a><a name="p3949012174411"></a>初始化构建图检索（有参构造、无参构造）。</p>
</td>
</tr>
<tr id="row9949131219443"><td class="cellrowborder" valign="top" width="34.38%" headers="mcps1.2.3.1.1 "><p id="p1094921294415"><a name="p1094921294415"></a><a name="p1094921294415"></a>Add</p>
</td>
<td class="cellrowborder" valign="top" width="65.62%" headers="mcps1.2.3.1.2 "><p id="p1794941284418"><a name="p1794941284418"></a><a name="p1794941284418"></a>构建图索引。</p>
</td>
</tr>
<tr id="row379293619370"><td class="cellrowborder" valign="top" width="34.38%" headers="mcps1.2.3.1.1 "><p id="p10792123618373"><a name="p10792123618373"></a><a name="p10792123618373"></a>BuildSearcher</p>
</td>
<td class="cellrowborder" valign="top" width="65.62%" headers="mcps1.2.3.1.2 "><p id="p379243633713"><a name="p379243633713"></a><a name="p379243633713"></a>构建检索器。</p>
</td>
</tr>
<tr id="row1594913120443"><td class="cellrowborder" valign="top" width="34.38%" headers="mcps1.2.3.1.1 "><p id="p4949012144417"><a name="p4949012144417"></a><a name="p4949012144417"></a>Search</p>
</td>
<td class="cellrowborder" valign="top" width="65.62%" headers="mcps1.2.3.1.2 "><p id="p594911128445"><a name="p594911128445"></a><a name="p594911128445"></a>图检索。</p>
</td>
</tr>
<tr id="row6949131274416"><td class="cellrowborder" valign="top" width="34.38%" headers="mcps1.2.3.1.1 "><p id="p594971224411"><a name="p594971224411"></a><a name="p594971224411"></a>SetEf</p>
</td>
<td class="cellrowborder" valign="top" width="65.62%" headers="mcps1.2.3.1.2 "><p id="p794971214414"><a name="p794971214414"></a><a name="p794971214414"></a>设置检索时的候选节点列表大小。</p>
</td>
</tr>
<tr id="row694916124445"><td class="cellrowborder" valign="top" width="34.38%" headers="mcps1.2.3.1.1 "><p id="p8949131214448"><a name="p8949131214448"></a><a name="p8949131214448"></a>Save</p>
</td>
<td class="cellrowborder" valign="top" width="65.62%" headers="mcps1.2.3.1.2 "><p id="p894941210443"><a name="p894941210443"></a><a name="p894941210443"></a>保存检索器到指定路径。</p>
</td>
</tr>
<tr id="row159491712174414"><td class="cellrowborder" valign="top" width="34.38%" headers="mcps1.2.3.1.1 "><p id="p894991214449"><a name="p894991214449"></a><a name="p894991214449"></a>Load</p>
</td>
<td class="cellrowborder" valign="top" width="65.62%" headers="mcps1.2.3.1.2 "><p id="p2094917128448"><a name="p2094917128448"></a><a name="p2094917128448"></a>从指定路径加载检索器。</p>
</td>
</tr>
<tr id="row184131856399"><td class="cellrowborder" valign="top" width="34.38%" headers="mcps1.2.3.1.1 "><p id="p935410178398"><a name="p935410178398"></a><a name="p935410178398"></a>SaveGraph</p>
</td>
<td class="cellrowborder" valign="top" width="65.62%" headers="mcps1.2.3.1.2 "><p id="p113548174390"><a name="p113548174390"></a><a name="p113548174390"></a>保存图索引到指定路径。</p>
</td>
</tr>
<tr id="row1587810973913"><td class="cellrowborder" valign="top" width="34.38%" headers="mcps1.2.3.1.1 "><p id="p0355121763910"><a name="p0355121763910"></a><a name="p0355121763910"></a>LoadGraph</p>
</td>
<td class="cellrowborder" valign="top" width="65.62%" headers="mcps1.2.3.1.2 "><p id="p12355117103918"><a name="p12355117103918"></a><a name="p12355117103918"></a>从指定路径加载图索引。</p>
</td>
</tr>
<tr id="row78159104213"><td class="cellrowborder" valign="top" width="34.38%" headers="mcps1.2.3.1.1 "><p id="p108461119154212"><a name="p108461119154212"></a><a name="p108461119154212"></a>Serialize</p>
</td>
<td class="cellrowborder" valign="top" width="65.62%" headers="mcps1.2.3.1.2 "><p id="p1584621994217"><a name="p1584621994217"></a><a name="p1584621994217"></a>将检索器内容存储至数组内。</p>
</td>
</tr>
<tr id="row123946122423"><td class="cellrowborder" valign="top" width="34.38%" headers="mcps1.2.3.1.1 "><p id="p2846119204220"><a name="p2846119204220"></a><a name="p2846119204220"></a>Deserialize</p>
</td>
<td class="cellrowborder" valign="top" width="65.62%" headers="mcps1.2.3.1.2 "><p id="p3403194411458"><a name="p3403194411458"></a><a name="p3403194411458"></a>还原数组内的检索器内容。</p>
</td>
</tr>
<tr id="row968819494476"><td class="cellrowborder" valign="top" width="34.38%" headers="mcps1.2.3.1.1 "><p id="p7688749124717"><a name="p7688749124717"></a><a name="p7688749124717"></a>GetNTotal</p>
</td>
<td class="cellrowborder" valign="top" width="65.62%" headers="mcps1.2.3.1.2 "><p id="p668874918478"><a name="p668874918478"></a><a name="p668874918478"></a>返回图索引内的底库数据量。</p>
</td>
</tr>
<tr id="row89311814810"><td class="cellrowborder" valign="top" width="34.38%" headers="mcps1.2.3.1.1 "><p id="p09312186486"><a name="p09312186486"></a><a name="p09312186486"></a>GetDim</p>
</td>
<td class="cellrowborder" valign="top" width="65.62%" headers="mcps1.2.3.1.2 "><p id="p39310182489"><a name="p39310182489"></a><a name="p39310182489"></a>返回图索引内的数据维度。</p>
</td>
</tr>
<tr id="row170810446223"><td class="cellrowborder" valign="top" width="34.38%" headers="mcps1.2.3.1.1 "><p id="p227124617229"><a name="p227124617229"></a><a name="p227124617229"></a>SetEarlyStoppingParams</p>
</td>
<td class="cellrowborder" valign="top" width="65.62%" headers="mcps1.2.3.1.2 "><p id="p87099445228"><a name="p87099445228"></a><a name="p87099445228"></a>设置早停优化点参数。</p>
</td>
</tr>
</tbody>
</table>

### 构造函数（有参构造）

**接口定义<a name="section172317194488"></a>**

KBest\(int dim, int R, int L, int A, const char \*metric, const std::string &init\_builder\_type\);

KBest\(int dim, int R, int L, float A, int graph\_opt\_iter, const std::string &metric, const std::string &init\_builder\_type, const std::string &index\_type\);

**接口用途<a name="section1153124784912"></a>**

初始化构建图检索。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.56155615561556%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="13.06130613061306%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="35.52355235523553%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>dim</p>
</td>
<td class="cellrowborder" valign="top" width="13.06130613061306%" headers="mcps1.1.5.1.2 "><p id="p98931015893"><a name="p98931015893"></a><a name="p98931015893"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="35.52355235523553%" headers="mcps1.1.5.1.3 "><p id="p182303331508"><a name="p182303331508"></a><a name="p182303331508"></a>特征维度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>[1,2999]</p>
</td>
</tr>
<tr id="row11230173385019"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p22301333165015"><a name="p22301333165015"></a><a name="p22301333165015"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="13.06130613061306%" headers="mcps1.1.5.1.2 "><p id="p5893141517919"><a name="p5893141517919"></a><a name="p5893141517919"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="35.52355235523553%" headers="mcps1.1.5.1.3 "><p id="p10230433115013"><a name="p10230433115013"></a><a name="p10230433115013"></a>邻居节点数。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p129897813251"><a name="p129897813251"></a><a name="p129897813251"></a>[11,499]</p>
</td>
</tr>
<tr id="row1368063274610"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p116802032174613"><a name="p116802032174613"></a><a name="p116802032174613"></a>L</p>
</td>
<td class="cellrowborder" valign="top" width="13.06130613061306%" headers="mcps1.1.5.1.2 "><p id="p489312151893"><a name="p489312151893"></a><a name="p489312151893"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="35.52355235523553%" headers="mcps1.1.5.1.3 "><p id="p268013224617"><a name="p268013224617"></a><a name="p268013224617"></a>构图时的候选节点列表大小。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p6989158192510"><a name="p6989158192510"></a><a name="p6989158192510"></a>[11,1999]</p>
</td>
</tr>
<tr id="row8597534164617"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p4597734184616"><a name="p4597734184616"></a><a name="p4597734184616"></a>A</p>
</td>
<td class="cellrowborder" valign="top" width="13.06130613061306%" headers="mcps1.1.5.1.2 "><p id="p178931015394"><a name="p178931015394"></a><a name="p178931015394"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="35.52355235523553%" headers="mcps1.1.5.1.3 "><p id="p65975343465"><a name="p65975343465"></a><a name="p65975343465"></a>构图剪枝时的角度阈值。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p16989883251"><a name="p16989883251"></a><a name="p16989883251"></a>[11,360]</p>
</td>
</tr>
<tr id="row523013315504"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p10230123316509"><a name="p10230123316509"></a><a name="p10230123316509"></a>metric</p>
</td>
<td class="cellrowborder" valign="top" width="13.06130613061306%" headers="mcps1.1.5.1.2 "><p id="p2894215596"><a name="p2894215596"></a><a name="p2894215596"></a>const char *</p>
</td>
<td class="cellrowborder" valign="top" width="35.52355235523553%" headers="mcps1.1.5.1.3 "><p id="p102301133105015"><a name="p102301133105015"></a><a name="p102301133105015"></a>距离度量的方式。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p16989188132515"><a name="p16989188132515"></a><a name="p16989188132515"></a><span class="parmvalue" id="parmvalue12115517324"><a name="parmvalue12115517324"></a><a name="parmvalue12115517324"></a>“L2”</span>或<span class="parmvalue" id="parmvalue18251015195114"><a name="parmvalue18251015195114"></a><a name="parmvalue18251015195114"></a>“IP”</span>。</p>
<a name="ul396901541013"></a><a name="ul396901541013"></a><ul id="ul396901541013"><li><span class="parmvalue" id="parmvalue28857185517"><a name="parmvalue28857185517"></a><a name="parmvalue28857185517"></a>“L2”</span>为欧几里得距离。</li><li><span class="parmvalue" id="parmvalue1928610244515"><a name="parmvalue1928610244515"></a><a name="parmvalue1928610244515"></a>“IP”</span>为内积距离。</li></ul>
</td>
</tr>
<tr id="row1523083315012"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p10230433105020"><a name="p10230433105020"></a><a name="p10230433105020"></a>init_builder_type</p>
</td>
<td class="cellrowborder" valign="top" width="13.06130613061306%" headers="mcps1.1.5.1.2 "><p id="p15894141519917"><a name="p15894141519917"></a><a name="p15894141519917"></a>const std::string &amp;</p>
</td>
<td class="cellrowborder" valign="top" width="35.52355235523553%" headers="mcps1.1.5.1.3 "><p id="p623053365015"><a name="p623053365015"></a><a name="p623053365015"></a>构建k近邻图的算法。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1946832961016"><a name="p1946832961016"></a><a name="p1946832961016"></a><span class="parmvalue" id="parmvalue176672813511"><a name="parmvalue176672813511"></a><a name="parmvalue176672813511"></a>“RNNDescent”</span>或<span class="parmvalue" id="parmvalue4621549165112"><a name="parmvalue4621549165112"></a><a name="parmvalue4621549165112"></a>“NNDescent”</span>，表示两种不同的构建k近邻图的算法，推荐使用<span class="parmvalue" id="parmvalue534725412518"><a name="parmvalue534725412518"></a><a name="parmvalue534725412518"></a>“RNNDescent”</span>。</p>
</td>
</tr>
<tr id="row387211011106"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p2023791201011"><a name="p2023791201011"></a><a name="p2023791201011"></a>graph_opt_iter</p>
</td>
<td class="cellrowborder" valign="top" width="13.06130613061306%" headers="mcps1.1.5.1.2 "><p id="p198722006101"><a name="p198722006101"></a><a name="p198722006101"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="35.52355235523553%" headers="mcps1.1.5.1.3 "><p id="p10237212111013"><a name="p10237212111013"></a><a name="p10237212111013"></a>图索引自我迭代的轮数。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p8872207100"><a name="p8872207100"></a><a name="p8872207100"></a>[0,30]</p>
</td>
</tr>
<tr id="row7131153011107"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p1546185591017"><a name="p1546185591017"></a><a name="p1546185591017"></a>index_type</p>
</td>
<td class="cellrowborder" valign="top" width="13.06130613061306%" headers="mcps1.1.5.1.2 "><p id="p19131103031011"><a name="p19131103031011"></a><a name="p19131103031011"></a><span>const std::string </span><span>&amp;</span></p>
</td>
<td class="cellrowborder" valign="top" width="35.52355235523553%" headers="mcps1.1.5.1.3 "><p id="p55461255161011"><a name="p55461255161011"></a><a name="p55461255161011"></a>选择邻居策略。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p213293001016"><a name="p213293001016"></a><a name="p213293001016"></a><span class="parmvalue" id="parmvalue3260403116"><a name="parmvalue3260403116"></a><a name="parmvalue3260403116"></a>“HNSW”</span><span>或</span><span class="parmvalue" id="parmvalue41171544161114"><a name="parmvalue41171544161114"></a><a name="parmvalue41171544161114"></a>“NSG”</span><span>或</span><span class="parmvalue" id="parmvalue1739675061118"><a name="parmvalue1739675061118"></a><a name="parmvalue1739675061118"></a>“TSDG”</span><span>或</span><span class="parmvalue" id="parmvalue5852453141117"><a name="parmvalue5852453141117"></a><a name="parmvalue5852453141117"></a>“SSG”</span>，表示四种不同的选择邻居策略。</p>
</td>
</tr>
</tbody>
</table>

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
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="14.528547145285472%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="18.488151184881513%" id="mcps1.1.5.1.2"><p id="p18620101081116"><a name="p18620101081116"></a><a name="p18620101081116"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="21.14788521147885%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="45.83541645835416%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="14.528547145285472%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>nb</p>
</td>
<td class="cellrowborder" valign="top" width="18.488151184881513%" headers="mcps1.1.5.1.2 "><p id="p15620161014116"><a name="p15620161014116"></a><a name="p15620161014116"></a><span>int</span></p>
</td>
<td class="cellrowborder" valign="top" width="21.14788521147885%" headers="mcps1.1.5.1.3 "><p id="p182303331508"><a name="p182303331508"></a><a name="p182303331508"></a>向量底库数据量。</p>
</td>
<td class="cellrowborder" valign="top" width="45.83541645835416%" headers="mcps1.1.5.1.4 "><p id="p1151275553412"><a name="p1151275553412"></a><a name="p1151275553412"></a>大于等于1。建议小于10亿。</p>
</td>
</tr>
<tr id="row11230173385019"><td class="cellrowborder" valign="top" width="14.528547145285472%" headers="mcps1.1.5.1.1 "><p id="p22301333165015"><a name="p22301333165015"></a><a name="p22301333165015"></a>xb</p>
</td>
<td class="cellrowborder" valign="top" width="18.488151184881513%" headers="mcps1.1.5.1.2 "><p id="p362011011112"><a name="p362011011112"></a><a name="p362011011112"></a>const float *</p>
</td>
<td class="cellrowborder" valign="top" width="21.14788521147885%" headers="mcps1.1.5.1.3 "><p id="p10230433115013"><a name="p10230433115013"></a><a name="p10230433115013"></a>向量底库数据。</p>
</td>
<td class="cellrowborder" valign="top" width="45.83541645835416%" headers="mcps1.1.5.1.4 "><p id="p15512135514343"><a name="p15512135514343"></a><a name="p15512135514343"></a>限制非空，长度应为nb * dim（数据量 * 特征维度）。</p>
</td>
</tr>
<tr id="row92309336505"><td class="cellrowborder" valign="top" width="14.528547145285472%" headers="mcps1.1.5.1.1 "><p id="p162309336505"><a name="p162309336505"></a><a name="p162309336505"></a>consecutive</p>
</td>
<td class="cellrowborder" valign="top" width="18.488151184881513%" headers="mcps1.1.5.1.2 "><p id="p0620310181118"><a name="p0620310181118"></a><a name="p0620310181118"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="21.14788521147885%" headers="mcps1.1.5.1.3 "><p id="p92301933165017"><a name="p92301933165017"></a><a name="p92301933165017"></a>块大小。</p>
</td>
<td class="cellrowborder" valign="top" width="45.83541645835416%" headers="mcps1.1.5.1.4 "><p id="p1151265503419"><a name="p1151265503419"></a><a name="p1151265503419"></a>[1,31]</p>
</td>
</tr>
<tr id="row523013315504"><td class="cellrowborder" valign="top" width="14.528547145285472%" headers="mcps1.1.5.1.1 "><p id="p10230123316509"><a name="p10230123316509"></a><a name="p10230123316509"></a>level</p>
</td>
<td class="cellrowborder" valign="top" width="18.488151184881513%" headers="mcps1.1.5.1.2 "><p id="p126201910161110"><a name="p126201910161110"></a><a name="p126201910161110"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="21.14788521147885%" headers="mcps1.1.5.1.3 "><p id="p102301133105015"><a name="p102301133105015"></a><a name="p102301133105015"></a>控制量化的等级。</p>
</td>
<td class="cellrowborder" valign="top" width="45.83541645835416%" headers="mcps1.1.5.1.4 "><p id="p19544111913232"><a name="p19544111913232"></a><a name="p19544111913232"></a>[0,3]</p>
<a name="ul1454195619238"></a><a name="ul1454195619238"></a><ul id="ul1454195619238"><li>0：表示FP32量化。</li><li>1：表示SQ8U量化。</li><li>2：表示SQ4U量化。</li><li>3：表示FP16量化。</li></ul>
</td>
</tr>
<tr id="row1836863331311"><td class="cellrowborder" valign="top" width="14.528547145285472%" headers="mcps1.1.5.1.1 "><p id="p1830838111320"><a name="p1830838111320"></a><a name="p1830838111320"></a>reorder</p>
</td>
<td class="cellrowborder" valign="top" width="18.488151184881513%" headers="mcps1.1.5.1.2 "><p id="p73681333191314"><a name="p73681333191314"></a><a name="p73681333191314"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="21.14788521147885%" headers="mcps1.1.5.1.3 "><p id="p1083016385138"><a name="p1083016385138"></a><a name="p1083016385138"></a>是否开启底库向量重排。</p>
</td>
<td class="cellrowborder" valign="top" width="45.83541645835416%" headers="mcps1.1.5.1.4 "><p id="p53681533101319"><a name="p53681533101319"></a><a name="p53681533101319"></a>0或1。</p>
</td>
</tr>
</tbody>
</table>

**返回值<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>
<table><thead align="left"><tr id="row1569152711463"><th class="cellrowborder" valign="top" width="34.599999999999994%" id="mcps1.1.3.1.1"><p id="p146911527174618"><a name="p146911527174618"></a><a name="p146911527174618"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="65.4%" id="mcps1.1.3.1.2"><p id="p136911627194618"><a name="p136911627194618"></a><a name="p136911627194618"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row769192744612"><td class="cellrowborder" valign="top" width="34.599999999999994%" headers="mcps1.1.3.1.1 "><p id="p106910272463"><a name="p106910272463"></a><a name="p106910272463"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="65.4%" headers="mcps1.1.3.1.2 "><p id="p2611111352313"><a name="p2611111352313"></a><a name="p2611111352313"></a>若参数超出取值范围则返回-1，在调用Load/Deserialize/LoadGraph后调用该接口时返回-1，否则返回0。</p>
</td>
</tr>
</tbody>
</table>

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
<table><thead align="left"><tr id="row1569152711463"><th class="cellrowborder" valign="top" width="34.599999999999994%" id="mcps1.1.3.1.1"><p id="p146911527174618"><a name="p146911527174618"></a><a name="p146911527174618"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="65.4%" id="mcps1.1.3.1.2"><p id="p136911627194618"><a name="p136911627194618"></a><a name="p136911627194618"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row769192744612"><td class="cellrowborder" valign="top" width="34.599999999999994%" headers="mcps1.1.3.1.1 "><p id="p106910272463"><a name="p106910272463"></a><a name="p106910272463"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="65.4%" headers="mcps1.1.3.1.2 "><p id="p2611111352313"><a name="p2611111352313"></a><a name="p2611111352313"></a>在调用Load/Deserialize/LoadGraph后调用该接口时返回-1，检索器不改变。</p>
</td>
</tr>
</tbody>
</table>

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
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="12.73%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="18.2%" id="mcps1.1.5.1.2"><p id="p1521112495121"><a name="p1521112495121"></a><a name="p1521112495121"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="29.79%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="39.28%" id="mcps1.1.5.1.4"><p id="p84604435401"><a name="p84604435401"></a><a name="p84604435401"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="12.73%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>nq</p>
</td>
<td class="cellrowborder" valign="top" width="18.2%" headers="mcps1.1.5.1.2 "><p id="p1521194918129"><a name="p1521194918129"></a><a name="p1521194918129"></a><span>int</span></p>
</td>
<td class="cellrowborder" valign="top" width="29.79%" headers="mcps1.1.5.1.3 "><p id="p182303331508"><a name="p182303331508"></a><a name="p182303331508"></a>查询向量集数据量。</p>
</td>
<td class="cellrowborder" valign="top" width="39.28%" headers="mcps1.1.5.1.4 "><p id="p1446074319406"><a name="p1446074319406"></a><a name="p1446074319406"></a>大于等于1。建议小于10亿。</p>
</td>
</tr>
<tr id="row11230173385019"><td class="cellrowborder" valign="top" width="12.73%" headers="mcps1.1.5.1.1 "><p id="p22301333165015"><a name="p22301333165015"></a><a name="p22301333165015"></a>xq</p>
</td>
<td class="cellrowborder" valign="top" width="18.2%" headers="mcps1.1.5.1.2 "><p id="p321144921213"><a name="p321144921213"></a><a name="p321144921213"></a>const float *</p>
</td>
<td class="cellrowborder" valign="top" width="29.79%" headers="mcps1.1.5.1.3 "><p id="p10230433115013"><a name="p10230433115013"></a><a name="p10230433115013"></a>查询向量集数据。</p>
</td>
<td class="cellrowborder" valign="top" width="39.28%" headers="mcps1.1.5.1.4 "><p id="p19460943204013"><a name="p19460943204013"></a><a name="p19460943204013"></a>限制非空，期待长度为nq * dim（数据量 * 特征维度）。</p>
</td>
</tr>
<tr id="row92309336505"><td class="cellrowborder" valign="top" width="12.73%" headers="mcps1.1.5.1.1 "><p id="p162309336505"><a name="p162309336505"></a><a name="p162309336505"></a>topk</p>
</td>
<td class="cellrowborder" valign="top" width="18.2%" headers="mcps1.1.5.1.2 "><p id="p122111249101212"><a name="p122111249101212"></a><a name="p122111249101212"></a><span>int</span></p>
</td>
<td class="cellrowborder" valign="top" width="29.79%" headers="mcps1.1.5.1.3 "><p id="p92301933165017"><a name="p92301933165017"></a><a name="p92301933165017"></a>最近邻的数量。</p>
</td>
<td class="cellrowborder" valign="top" width="39.28%" headers="mcps1.1.5.1.4 "><p id="p1178758184115"><a name="p1178758184115"></a><a name="p1178758184115"></a>[1,nb]，其中<span class="parmname" id="parmname15768691767"><a name="parmname15768691767"></a><a name="parmname15768691767"></a>“nb”</span>为向量底库数据量大小。</p>
</td>
</tr>
<tr id="row523013315504"><td class="cellrowborder" valign="top" width="12.73%" headers="mcps1.1.5.1.1 "><p id="p10230123316509"><a name="p10230123316509"></a><a name="p10230123316509"></a>distances</p>
</td>
<td class="cellrowborder" valign="top" width="18.2%" headers="mcps1.1.5.1.2 "><p id="p5211114910120"><a name="p5211114910120"></a><a name="p5211114910120"></a>float *</p>
</td>
<td class="cellrowborder" valign="top" width="29.79%" headers="mcps1.1.5.1.3 "><p id="p102301133105015"><a name="p102301133105015"></a><a name="p102301133105015"></a>距离数组。</p>
</td>
<td class="cellrowborder" valign="top" width="39.28%" headers="mcps1.1.5.1.4 "><p id="p124318194133"><a name="p124318194133"></a><a name="p124318194133"></a>限制非空，<span>期待长度为nq * topk</span>。</p>
</td>
</tr>
<tr id="row1523083315012"><td class="cellrowborder" valign="top" width="12.73%" headers="mcps1.1.5.1.1 "><p id="p10230433105020"><a name="p10230433105020"></a><a name="p10230433105020"></a>labels</p>
</td>
<td class="cellrowborder" valign="top" width="18.2%" headers="mcps1.1.5.1.2 "><p id="p1921118495123"><a name="p1921118495123"></a><a name="p1921118495123"></a>int64_t *</p>
</td>
<td class="cellrowborder" valign="top" width="29.79%" headers="mcps1.1.5.1.3 "><p id="p33565281418"><a name="p33565281418"></a><a name="p33565281418"></a>检索结果的ID数组。</p>
</td>
<td class="cellrowborder" valign="top" width="39.28%" headers="mcps1.1.5.1.4 "><p id="p124602043204018"><a name="p124602043204018"></a><a name="p124602043204018"></a>限制非空，<span>期待长度为nq * topk</span>。</p>
</td>
</tr>
<tr id="row177151948121320"><td class="cellrowborder" valign="top" width="12.73%" headers="mcps1.1.5.1.1 "><p id="p3715448191319"><a name="p3715448191319"></a><a name="p3715448191319"></a>num_thread</p>
</td>
<td class="cellrowborder" valign="top" width="18.2%" headers="mcps1.1.5.1.2 "><p id="p4211249101218"><a name="p4211249101218"></a><a name="p4211249101218"></a><span>int</span></p>
</td>
<td class="cellrowborder" valign="top" width="29.79%" headers="mcps1.1.5.1.3 "><p id="p137151148161319"><a name="p137151148161319"></a><a name="p137151148161319"></a>检索时使用的线程数。</p>
</td>
<td class="cellrowborder" valign="top" width="39.28%" headers="mcps1.1.5.1.4 "><p id="p95801533174311"><a name="p95801533174311"></a><a name="p95801533174311"></a>[1,std::thread::hardware_concurrency()]，其中std::thread::hardware_concurrency()为<span>当前系统支持的并发线程数</span>。</p>
</td>
</tr>
</tbody>
</table>

**返回值<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>
<table><thead align="left"><tr id="row1569152711463"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p146911527174618"><a name="p146911527174618"></a><a name="p146911527174618"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p136911627194618"><a name="p136911627194618"></a><a name="p136911627194618"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row769192744612"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p106910272463"><a name="p106910272463"></a><a name="p106910272463"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p2611111352313"><a name="p2611111352313"></a><a name="p2611111352313"></a>若参数超出取值范围则返回-1；在调用BuildSearcher或Load/Deserialize/LoadGraph前调用该接口时返回-1；否则返回0。</p>
</td>
</tr>
</tbody>
</table>

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
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="14.280000000000001%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="15.64%" id="mcps1.1.5.1.2"><p id="p82341657161314"><a name="p82341657161314"></a><a name="p82341657161314"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="34.54%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="35.54%" id="mcps1.1.5.1.4"><p id="p1440932116441"><a name="p1440932116441"></a><a name="p1440932116441"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="14.280000000000001%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>ef</p>
</td>
<td class="cellrowborder" valign="top" width="15.64%" headers="mcps1.1.5.1.2 "><p id="p9234135711132"><a name="p9234135711132"></a><a name="p9234135711132"></a><span>int</span></p>
</td>
<td class="cellrowborder" valign="top" width="34.54%" headers="mcps1.1.5.1.3 "><p id="p39711451181514"><a name="p39711451181514"></a><a name="p39711451181514"></a>检索时的候选节点列表大小。</p>
</td>
<td class="cellrowborder" valign="top" width="35.54%" headers="mcps1.1.5.1.4 "><p id="p1178758184115"><a name="p1178758184115"></a><a name="p1178758184115"></a>[1,nb]，其中<span class="parmname" id="parmname163388165617"><a name="parmname163388165617"></a><a name="parmname163388165617"></a>“nb”</span>为向量底库数据量大小。</p>
</td>
</tr>
</tbody>
</table>

**返回值<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>
<table><thead align="left"><tr id="row1569152711463"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p146911527174618"><a name="p146911527174618"></a><a name="p146911527174618"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p136911627194618"><a name="p136911627194618"></a><a name="p136911627194618"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row769192744612"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p106910272463"><a name="p106910272463"></a><a name="p106910272463"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p2611111352313"><a name="p2611111352313"></a><a name="p2611111352313"></a>若参数超出取值范围则返回-1；在调用BuildSearcher或Load/Deserialize/LoadGraph前调用该接口时返回-1；否则返回0。</p>
</td>
</tr>
</tbody>
</table>

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
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="16.06%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="15.18%" id="mcps1.1.5.1.2"><p id="p17714142111149"><a name="p17714142111149"></a><a name="p17714142111149"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="34.239999999999995%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="34.52%" id="mcps1.1.5.1.4"><p id="p1440932116441"><a name="p1440932116441"></a><a name="p1440932116441"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="16.06%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>path</p>
</td>
<td class="cellrowborder" valign="top" width="15.18%" headers="mcps1.1.5.1.2 "><p id="p171412119148"><a name="p171412119148"></a><a name="p171412119148"></a>const char *</p>
</td>
<td class="cellrowborder" valign="top" width="34.239999999999995%" headers="mcps1.1.5.1.3 "><p id="p39711451181514"><a name="p39711451181514"></a><a name="p39711451181514"></a>检索器的保存路径。</p>
</td>
<td class="cellrowborder" valign="top" width="34.52%" headers="mcps1.1.5.1.4 "><p id="p20167131514510"><a name="p20167131514510"></a><a name="p20167131514510"></a>取值长度小于199字符。</p>
</td>
</tr>
</tbody>
</table>

**返回值<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>
<table><thead align="left"><tr id="row1569152711463"><th class="cellrowborder" valign="top" width="38.95%" id="mcps1.1.3.1.1"><p id="p146911527174618"><a name="p146911527174618"></a><a name="p146911527174618"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="61.050000000000004%" id="mcps1.1.3.1.2"><p id="p136911627194618"><a name="p136911627194618"></a><a name="p136911627194618"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row769192744612"><td class="cellrowborder" valign="top" width="38.95%" headers="mcps1.1.3.1.1 "><p id="p106910272463"><a name="p106910272463"></a><a name="p106910272463"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="61.050000000000004%" headers="mcps1.1.3.1.2 "><p id="p2611111352313"><a name="p2611111352313"></a><a name="p2611111352313"></a>若参数超出取值范围或存在保存路径错误等IO问题时返回-1；在<span>调用BuildSearcher前调用该接口</span>时返回-1；否则返回0。</p>
</td>
</tr>
</tbody>
</table>

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
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="16.13161316131613%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="15.441544154415443%" id="mcps1.1.5.1.2"><p id="p2138751201416"><a name="p2138751201416"></a><a name="p2138751201416"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="35.34353435343534%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="33.083308330833084%" id="mcps1.1.5.1.4"><p id="p1440932116441"><a name="p1440932116441"></a><a name="p1440932116441"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="16.13161316131613%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>path</p>
</td>
<td class="cellrowborder" valign="top" width="15.441544154415443%" headers="mcps1.1.5.1.2 "><p id="p11381051141410"><a name="p11381051141410"></a><a name="p11381051141410"></a>const char *</p>
</td>
<td class="cellrowborder" valign="top" width="35.34353435343534%" headers="mcps1.1.5.1.3 "><p id="p39711451181514"><a name="p39711451181514"></a><a name="p39711451181514"></a>检索器的加载路径。</p>
</td>
<td class="cellrowborder" valign="top" width="33.083308330833084%" headers="mcps1.1.5.1.4 "><p id="p20167131514510"><a name="p20167131514510"></a><a name="p20167131514510"></a>取值长度小于199字符。</p>
</td>
</tr>
</tbody>
</table>

**返回值<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>
<table><thead align="left"><tr id="row1569152711463"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p146911527174618"><a name="p146911527174618"></a><a name="p146911527174618"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p136911627194618"><a name="p136911627194618"></a><a name="p136911627194618"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row769192744612"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p106910272463"><a name="p106910272463"></a><a name="p106910272463"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p2611111352313"><a name="p2611111352313"></a><a name="p2611111352313"></a>若参数超出取值范围或存在读取路径错误等IO问题时返回-1；否则返回0。</p>
</td>
</tr>
</tbody>
</table>

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
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="13.63%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.48%" id="mcps1.1.5.1.2"><p id="p13945191217156"><a name="p13945191217156"></a><a name="p13945191217156"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="34.510000000000005%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="34.38%" id="mcps1.1.5.1.4"><p id="p1440932116441"><a name="p1440932116441"></a><a name="p1440932116441"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="13.63%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>path</p>
</td>
<td class="cellrowborder" valign="top" width="17.48%" headers="mcps1.1.5.1.2 "><p id="p8945111231510"><a name="p8945111231510"></a><a name="p8945111231510"></a>const char *</p>
</td>
<td class="cellrowborder" valign="top" width="34.510000000000005%" headers="mcps1.1.5.1.3 "><p id="p39711451181514"><a name="p39711451181514"></a><a name="p39711451181514"></a>图索引的保存路径。</p>
</td>
<td class="cellrowborder" valign="top" width="34.38%" headers="mcps1.1.5.1.4 "><p id="p20167131514510"><a name="p20167131514510"></a><a name="p20167131514510"></a>取值长度小于199字符。</p>
</td>
</tr>
</tbody>
</table>

**返回值<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>
<table><thead align="left"><tr id="row1569152711463"><th class="cellrowborder" valign="top" width="38.9%" id="mcps1.1.3.1.1"><p id="p146911527174618"><a name="p146911527174618"></a><a name="p146911527174618"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="61.1%" id="mcps1.1.3.1.2"><p id="p136911627194618"><a name="p136911627194618"></a><a name="p136911627194618"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row769192744612"><td class="cellrowborder" valign="top" width="38.9%" headers="mcps1.1.3.1.1 "><p id="p106910272463"><a name="p106910272463"></a><a name="p106910272463"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="61.1%" headers="mcps1.1.3.1.2 "><p id="p2611111352313"><a name="p2611111352313"></a><a name="p2611111352313"></a>若参数超出取值范围或存在保存路径错误等IO问题时返回-1；调用Add接口前调用该接口时返回-1；调用BuildSearcher或Load/Deserialize/LoadGraph后调用该接口时返回-1；否则返回0。</p>
</td>
</tr>
</tbody>
</table>

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
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="10.73%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="20.990000000000002%" id="mcps1.1.5.1.2"><p id="p16585143220155"><a name="p16585143220155"></a><a name="p16585143220155"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="25.66%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="42.620000000000005%" id="mcps1.1.5.1.4"><p id="p1440932116441"><a name="p1440932116441"></a><a name="p1440932116441"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="10.73%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>path</p>
</td>
<td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.1.5.1.2 "><p id="p17585193281515"><a name="p17585193281515"></a><a name="p17585193281515"></a>const char *</p>
</td>
<td class="cellrowborder" valign="top" width="25.66%" headers="mcps1.1.5.1.3 "><p id="p39711451181514"><a name="p39711451181514"></a><a name="p39711451181514"></a>检索器的加载路径。</p>
</td>
<td class="cellrowborder" valign="top" width="42.620000000000005%" headers="mcps1.1.5.1.4 "><p id="p20167131514510"><a name="p20167131514510"></a><a name="p20167131514510"></a>取值长度小于199字符。</p>
</td>
</tr>
<tr id="row641410102301"><td class="cellrowborder" valign="top" width="10.73%" headers="mcps1.1.5.1.1 "><p id="p19414810153017"><a name="p19414810153017"></a><a name="p19414810153017"></a>level</p>
</td>
<td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.1.5.1.2 "><p id="p195851932131517"><a name="p195851932131517"></a><a name="p195851932131517"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="25.66%" headers="mcps1.1.5.1.3 "><p id="p5414151014309"><a name="p5414151014309"></a><a name="p5414151014309"></a>控制量化的等级。</p>
</td>
<td class="cellrowborder" valign="top" width="42.620000000000005%" headers="mcps1.1.5.1.4 "><p id="p14665102215"><a name="p14665102215"></a><a name="p14665102215"></a>[-1,3]</p>
<a name="ul1454195619238"></a><a name="ul1454195619238"></a><ul id="ul1454195619238"><li>-1：默认值，表示SaveGraph时保存的量化等级。</li><li>0：表示FP32量化。</li><li>1：表示SQ8U量化。</li><li>2：表示SQ4U量化。</li><li>3：表示FP16量化。</li></ul>
</td>
</tr>
</tbody>
</table>

**返回值<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>
<table><thead align="left"><tr id="row1569152711463"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p146911527174618"><a name="p146911527174618"></a><a name="p146911527174618"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p136911627194618"><a name="p136911627194618"></a><a name="p136911627194618"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row769192744612"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p106910272463"><a name="p106910272463"></a><a name="p106910272463"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p2611111352313"><a name="p2611111352313"></a><a name="p2611111352313"></a>若参数超出取值范围或存在读取路径错误等IO问题时返回-1；否则返回0。</p>
</td>
</tr>
</tbody>
</table>

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
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="14.23%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="16.619999999999997%" id="mcps1.1.5.1.2"><p id="p1475418561158"><a name="p1475418561158"></a><a name="p1475418561158"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="36.84%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="32.31%" id="mcps1.1.5.1.4"><p id="p1440932116441"><a name="p1440932116441"></a><a name="p1440932116441"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="14.23%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>dataPtr</p>
</td>
<td class="cellrowborder" valign="top" width="16.619999999999997%" headers="mcps1.1.5.1.2 "><p id="p57541756181511"><a name="p57541756181511"></a><a name="p57541756181511"></a>uint8_t *&amp;</p>
</td>
<td class="cellrowborder" valign="top" width="36.84%" headers="mcps1.1.5.1.3 "><p id="p39711451181514"><a name="p39711451181514"></a><a name="p39711451181514"></a>存储检索器内容的数组的起始地址。</p>
</td>
<td class="cellrowborder" valign="top" width="32.31%" headers="mcps1.1.5.1.4 "><p id="p20167131514510"><a name="p20167131514510"></a><a name="p20167131514510"></a>限制为空指针。</p>
</td>
</tr>
<tr id="row641410102301"><td class="cellrowborder" valign="top" width="14.23%" headers="mcps1.1.5.1.1 "><p id="p19414810153017"><a name="p19414810153017"></a><a name="p19414810153017"></a>dataLength</p>
</td>
<td class="cellrowborder" valign="top" width="16.619999999999997%" headers="mcps1.1.5.1.2 "><p id="p57541256161516"><a name="p57541256161516"></a><a name="p57541256161516"></a>size_t &amp;</p>
</td>
<td class="cellrowborder" valign="top" width="36.84%" headers="mcps1.1.5.1.3 "><p id="p5414151014309"><a name="p5414151014309"></a><a name="p5414151014309"></a>存储检索器内容的数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="32.31%" headers="mcps1.1.5.1.4 "><p id="p44144105305"><a name="p44144105305"></a><a name="p44144105305"></a>限制为0。</p>
</td>
</tr>
</tbody>
</table>

**返回值<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>
<table><thead align="left"><tr id="row1569152711463"><th class="cellrowborder" valign="top" width="36.96%" id="mcps1.1.3.1.1"><p id="p146911527174618"><a name="p146911527174618"></a><a name="p146911527174618"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="63.04%" id="mcps1.1.3.1.2"><p id="p136911627194618"><a name="p136911627194618"></a><a name="p136911627194618"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row769192744612"><td class="cellrowborder" valign="top" width="36.96%" headers="mcps1.1.3.1.1 "><p id="p106910272463"><a name="p106910272463"></a><a name="p106910272463"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="63.04%" headers="mcps1.1.3.1.2 "><p id="p2611111352313"><a name="p2611111352313"></a><a name="p2611111352313"></a>若参数超出取值范围时返回-1；调用BuildSearcher或Load/Deserialize/LoadGraph后调用该接口时返回-1；否则返回0。</p>
</td>
</tr>
</tbody>
</table>

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
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="14.54854514548545%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="18.44815518448155%" id="mcps1.1.5.1.2"><p id="p8993101991611"><a name="p8993101991611"></a><a name="p8993101991611"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="32.436756324367565%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="34.56654334566544%" id="mcps1.1.5.1.4"><p id="p1440932116441"><a name="p1440932116441"></a><a name="p1440932116441"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="14.54854514548545%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>dataPtr</p>
</td>
<td class="cellrowborder" valign="top" width="18.44815518448155%" headers="mcps1.1.5.1.2 "><p id="p199331913161"><a name="p199331913161"></a><a name="p199331913161"></a>const uint8_t *</p>
</td>
<td class="cellrowborder" valign="top" width="32.436756324367565%" headers="mcps1.1.5.1.3 "><p id="p39711451181514"><a name="p39711451181514"></a><a name="p39711451181514"></a>存储检索器内容的数组的起始地址。</p>
</td>
<td class="cellrowborder" valign="top" width="34.56654334566544%" headers="mcps1.1.5.1.4 "><p id="p20167131514510"><a name="p20167131514510"></a><a name="p20167131514510"></a>限制非空。</p>
</td>
</tr>
<tr id="row641410102301"><td class="cellrowborder" valign="top" width="14.54854514548545%" headers="mcps1.1.5.1.1 "><p id="p19414810153017"><a name="p19414810153017"></a><a name="p19414810153017"></a>dataLength</p>
</td>
<td class="cellrowborder" valign="top" width="18.44815518448155%" headers="mcps1.1.5.1.2 "><p id="p2993101915163"><a name="p2993101915163"></a><a name="p2993101915163"></a>const size_t &amp;</p>
</td>
<td class="cellrowborder" valign="top" width="32.436756324367565%" headers="mcps1.1.5.1.3 "><p id="p5414151014309"><a name="p5414151014309"></a><a name="p5414151014309"></a>存储检索器内容的数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="34.56654334566544%" headers="mcps1.1.5.1.4 "><p id="p44144105305"><a name="p44144105305"></a><a name="p44144105305"></a>限制为Serialize接口时保存的数组长度。</p>
</td>
</tr>
</tbody>
</table>

**返回值<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>
<table><thead align="left"><tr id="row1569152711463"><th class="cellrowborder" valign="top" width="36.96%" id="mcps1.1.3.1.1"><p id="p146911527174618"><a name="p146911527174618"></a><a name="p146911527174618"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="63.04%" id="mcps1.1.3.1.2"><p id="p136911627194618"><a name="p136911627194618"></a><a name="p136911627194618"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row769192744612"><td class="cellrowborder" valign="top" width="36.96%" headers="mcps1.1.3.1.1 "><p id="p106910272463"><a name="p106910272463"></a><a name="p106910272463"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="63.04%" headers="mcps1.1.3.1.2 "><p id="p249262275018"><a name="p249262275018"></a><a name="p249262275018"></a>若参数超出取值范围时返回-1；否则返回0。</p>
<p id="p2611111352313"><a name="p2611111352313"></a><a name="p2611111352313"></a>Serialize接口内部申请数组内存，请在调用本接口后使用delete []释放该资源。</p>
</td>
</tr>
</tbody>
</table>

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
<table><thead align="left"><tr id="row1569152711463"><th class="cellrowborder" valign="top" width="36.96%" id="mcps1.1.3.1.1"><p id="p146911527174618"><a name="p146911527174618"></a><a name="p146911527174618"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="63.04%" id="mcps1.1.3.1.2"><p id="p136911627194618"><a name="p136911627194618"></a><a name="p136911627194618"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row769192744612"><td class="cellrowborder" valign="top" width="36.96%" headers="mcps1.1.3.1.1 "><p id="p106910272463"><a name="p106910272463"></a><a name="p106910272463"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="63.04%" headers="mcps1.1.3.1.2 "><p id="p2611111352313"><a name="p2611111352313"></a><a name="p2611111352313"></a>不添加底库的场景下，默认返回值为0。</p>
</td>
</tr>
</tbody>
</table>

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
<table><thead align="left"><tr id="row1569152711463"><th class="cellrowborder" valign="top" width="36.96%" id="mcps1.1.3.1.1"><p id="p146911527174618"><a name="p146911527174618"></a><a name="p146911527174618"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="63.04%" id="mcps1.1.3.1.2"><p id="p136911627194618"><a name="p136911627194618"></a><a name="p136911627194618"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row769192744612"><td class="cellrowborder" valign="top" width="36.96%" headers="mcps1.1.3.1.1 "><p id="p106910272463"><a name="p106910272463"></a><a name="p106910272463"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="63.04%" headers="mcps1.1.3.1.2 "><p id="p2611111352313"><a name="p2611111352313"></a><a name="p2611111352313"></a>有参构建的场景下等于<span class="parmname" id="parmname8379143211611"><a name="parmname8379143211611"></a><a name="parmname8379143211611"></a>“dim”</span>参数，无参构建的场景或有参构建后调用Load/Deserialize/LoadGraph接口后，返回值为读取的检索器/图索引中的数据的维度。</p>
</td>
</tr>
</tbody>
</table>

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
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.2984701529847%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.698230176982303%" id="mcps1.1.5.1.2"><p id="p8993101991611"><a name="p8993101991611"></a><a name="p8993101991611"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="32.436756324367565%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="34.56654334566544%" id="mcps1.1.5.1.4"><p id="p1440932116441"><a name="p1440932116441"></a><a name="p1440932116441"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.2984701529847%" headers="mcps1.1.5.1.1 "><p id="p6904143931516"><a name="p6904143931516"></a><a name="p6904143931516"></a>adding_pref</p>
</td>
<td class="cellrowborder" valign="top" width="17.698230176982303%" headers="mcps1.1.5.1.2 "><p id="p199331913161"><a name="p199331913161"></a><a name="p199331913161"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="32.436756324367565%" headers="mcps1.1.5.1.3 "><p id="p29041739131510"><a name="p29041739131510"></a><a name="p29041739131510"></a>超参候选集插入阈值。</p>
</td>
<td class="cellrowborder" valign="top" width="34.56654334566544%" headers="mcps1.1.5.1.4 "><p id="p20167131514510"><a name="p20167131514510"></a><a name="p20167131514510"></a>大于等于1。</p>
</td>
</tr>
<tr id="row641410102301"><td class="cellrowborder" valign="top" width="15.2984701529847%" headers="mcps1.1.5.1.1 "><p id="p11712134791515"><a name="p11712134791515"></a><a name="p11712134791515"></a>patience</p>
</td>
<td class="cellrowborder" valign="top" width="17.698230176982303%" headers="mcps1.1.5.1.2 "><p id="p2993101915163"><a name="p2993101915163"></a><a name="p2993101915163"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="32.436756324367565%" headers="mcps1.1.5.1.3 "><p id="p8712247141513"><a name="p8712247141513"></a><a name="p8712247141513"></a>检索耐心值。</p>
</td>
<td class="cellrowborder" valign="top" width="34.56654334566544%" headers="mcps1.1.5.1.4 "><p id="p57702186162"><a name="p57702186162"></a><a name="p57702186162"></a>大于等于1。</p>
</td>
</tr>
</tbody>
</table>

**返回值<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>
<table><thead align="left"><tr id="row1569152711463"><th class="cellrowborder" valign="top" width="36.09%" id="mcps1.1.3.1.1"><p id="p146911527174618"><a name="p146911527174618"></a><a name="p146911527174618"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="63.91%" id="mcps1.1.3.1.2"><p id="p136911627194618"><a name="p136911627194618"></a><a name="p136911627194618"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row769192744612"><td class="cellrowborder" valign="top" width="36.09%" headers="mcps1.1.3.1.1 "><p id="p106910272463"><a name="p106910272463"></a><a name="p106910272463"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="63.91%" headers="mcps1.1.3.1.2 "><p id="p2611111352313"><a name="p2611111352313"></a><a name="p2611111352313"></a>若参数超出取值范围时返回-1；调用BuildSearcher或Load/Deserialize/LoadGraph后调用该接口时返回-1；否则返回0。</p>
</td>
</tr>
</tbody>
</table>

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
<table><thead align="left"><tr id="row99491812134412"><th class="cellrowborder" valign="top" width="31.269999999999996%" id="mcps1.2.3.1.1"><p id="p1794951224415"><a name="p1794951224415"></a><a name="p1794951224415"></a>接口名称</p>
</th>
<th class="cellrowborder" valign="top" width="68.73%" id="mcps1.2.3.1.2"><p id="p6949612124415"><a name="p6949612124415"></a><a name="p6949612124415"></a>接口作用</p>
</th>
</tr>
</thead>
<tbody><tr id="row119491112174414"><td class="cellrowborder" valign="top" width="31.269999999999996%" headers="mcps1.2.3.1.1 "><p id="p1494931224410"><a name="p1494931224410"></a><a name="p1494931224410"></a>KBest</p>
</td>
<td class="cellrowborder" valign="top" width="68.73%" headers="mcps1.2.3.1.2 "><p id="p3949012174411"><a name="p3949012174411"></a><a name="p3949012174411"></a>初始化构建图检索（有参构造、无参构造）。</p>
</td>
</tr>
<tr id="row9949131219443"><td class="cellrowborder" valign="top" width="31.269999999999996%" headers="mcps1.2.3.1.1 "><p id="p1094921294415"><a name="p1094921294415"></a><a name="p1094921294415"></a>add</p>
</td>
<td class="cellrowborder" valign="top" width="68.73%" headers="mcps1.2.3.1.2 "><p id="p1794941284418"><a name="p1794941284418"></a><a name="p1794941284418"></a>构建图索引。</p>
</td>
</tr>
<tr id="row1511111561717"><td class="cellrowborder" valign="top" width="31.269999999999996%" headers="mcps1.2.3.1.1 "><p id="p10792123618373"><a name="p10792123618373"></a><a name="p10792123618373"></a>buildSearcher</p>
</td>
<td class="cellrowborder" valign="top" width="68.73%" headers="mcps1.2.3.1.2 "><p id="p379243633713"><a name="p379243633713"></a><a name="p379243633713"></a>构建检索器。</p>
</td>
</tr>
<tr id="row1594913120443"><td class="cellrowborder" valign="top" width="31.269999999999996%" headers="mcps1.2.3.1.1 "><p id="p4949012144417"><a name="p4949012144417"></a><a name="p4949012144417"></a>search</p>
</td>
<td class="cellrowborder" valign="top" width="68.73%" headers="mcps1.2.3.1.2 "><p id="p594911128445"><a name="p594911128445"></a><a name="p594911128445"></a>图检索。</p>
</td>
</tr>
<tr id="row6949131274416"><td class="cellrowborder" valign="top" width="31.269999999999996%" headers="mcps1.2.3.1.1 "><p id="p594971224411"><a name="p594971224411"></a><a name="p594971224411"></a>setEf</p>
</td>
<td class="cellrowborder" valign="top" width="68.73%" headers="mcps1.2.3.1.2 "><p id="p794971214414"><a name="p794971214414"></a><a name="p794971214414"></a>设置检索时的候选节点列表大小。</p>
</td>
</tr>
<tr id="row694916124445"><td class="cellrowborder" valign="top" width="31.269999999999996%" headers="mcps1.2.3.1.1 "><p id="p8949131214448"><a name="p8949131214448"></a><a name="p8949131214448"></a>save</p>
</td>
<td class="cellrowborder" valign="top" width="68.73%" headers="mcps1.2.3.1.2 "><p id="p894941210443"><a name="p894941210443"></a><a name="p894941210443"></a>保存检索器到指定路径。</p>
</td>
</tr>
<tr id="row159491712174414"><td class="cellrowborder" valign="top" width="31.269999999999996%" headers="mcps1.2.3.1.1 "><p id="p894991214449"><a name="p894991214449"></a><a name="p894991214449"></a>load</p>
</td>
<td class="cellrowborder" valign="top" width="68.73%" headers="mcps1.2.3.1.2 "><p id="p2094917128448"><a name="p2094917128448"></a><a name="p2094917128448"></a>从指定路径加载检索器。</p>
</td>
</tr>
<tr id="row1673619410185"><td class="cellrowborder" valign="top" width="31.269999999999996%" headers="mcps1.2.3.1.1 "><p id="p935410178398"><a name="p935410178398"></a><a name="p935410178398"></a>saveGraph</p>
</td>
<td class="cellrowborder" valign="top" width="68.73%" headers="mcps1.2.3.1.2 "><p id="p113548174390"><a name="p113548174390"></a><a name="p113548174390"></a>保存图索引到指定路径。</p>
</td>
</tr>
<tr id="row12461646151811"><td class="cellrowborder" valign="top" width="31.269999999999996%" headers="mcps1.2.3.1.1 "><p id="p0355121763910"><a name="p0355121763910"></a><a name="p0355121763910"></a>loadGraph</p>
</td>
<td class="cellrowborder" valign="top" width="68.73%" headers="mcps1.2.3.1.2 "><p id="p12355117103918"><a name="p12355117103918"></a><a name="p12355117103918"></a>从指定路径加载图索引。</p>
</td>
</tr>
<tr id="row55914831817"><td class="cellrowborder" valign="top" width="31.269999999999996%" headers="mcps1.2.3.1.1 "><p id="p108461119154212"><a name="p108461119154212"></a><a name="p108461119154212"></a>serialize</p>
</td>
<td class="cellrowborder" valign="top" width="68.73%" headers="mcps1.2.3.1.2 "><p id="p1584621994217"><a name="p1584621994217"></a><a name="p1584621994217"></a>将检索器内容存储至数组内。</p>
</td>
</tr>
<tr id="row169601149121817"><td class="cellrowborder" valign="top" width="31.269999999999996%" headers="mcps1.2.3.1.1 "><p id="p2846119204220"><a name="p2846119204220"></a><a name="p2846119204220"></a>deserialize</p>
</td>
<td class="cellrowborder" valign="top" width="68.73%" headers="mcps1.2.3.1.2 "><p id="p3403194411458"><a name="p3403194411458"></a><a name="p3403194411458"></a>还原数组内的检索器内容。</p>
</td>
</tr>
<tr id="row26944513185"><td class="cellrowborder" valign="top" width="31.269999999999996%" headers="mcps1.2.3.1.1 "><p id="p7688749124717"><a name="p7688749124717"></a><a name="p7688749124717"></a>getNTotal</p>
</td>
<td class="cellrowborder" valign="top" width="68.73%" headers="mcps1.2.3.1.2 "><p id="p668874918478"><a name="p668874918478"></a><a name="p668874918478"></a>返回图索引内的底库数据量。</p>
</td>
</tr>
<tr id="row13483105413186"><td class="cellrowborder" valign="top" width="31.269999999999996%" headers="mcps1.2.3.1.1 "><p id="p09312186486"><a name="p09312186486"></a><a name="p09312186486"></a>getDim</p>
</td>
<td class="cellrowborder" valign="top" width="68.73%" headers="mcps1.2.3.1.2 "><p id="p39310182489"><a name="p39310182489"></a><a name="p39310182489"></a>返回图索引内的数据维度。</p>
</td>
</tr>
<tr id="row53311836151712"><td class="cellrowborder" valign="top" width="31.269999999999996%" headers="mcps1.2.3.1.1 "><p id="p227124617229"><a name="p227124617229"></a><a name="p227124617229"></a>setEarlyStoppingParams</p>
</td>
<td class="cellrowborder" valign="top" width="68.73%" headers="mcps1.2.3.1.2 "><p id="p87099445228"><a name="p87099445228"></a><a name="p87099445228"></a>设置早停优化点参数。</p>
</td>
</tr>
</tbody>
</table>

### 构造函数（有参构造）

**接口定义<a name="section172317194488"></a>**

class KBest\(dim: int, R: int, L: int, A: int, graph\_opt\_iter:int, metric: string, init\_builder\_type: string, index\_type: string, numa\_enabled: bool, numa\_nodes\_number: int\)

**接口用途<a name="section1153124784912"></a>**

初始化构建图检索。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="18.099999999999998%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="15.36%" id="mcps1.1.5.1.2"><p id="p124241910191712"><a name="p124241910191712"></a><a name="p124241910191712"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="28.470000000000002%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="38.07%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="18.099999999999998%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>dim</p>
</td>
<td class="cellrowborder" valign="top" width="15.36%" headers="mcps1.1.5.1.2 "><p id="p164249104172"><a name="p164249104172"></a><a name="p164249104172"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="28.470000000000002%" headers="mcps1.1.5.1.3 "><p id="p182303331508"><a name="p182303331508"></a><a name="p182303331508"></a>特征维度。</p>
</td>
<td class="cellrowborder" valign="top" width="38.07%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>[1,2999]</p>
</td>
</tr>
<tr id="row11230173385019"><td class="cellrowborder" valign="top" width="18.099999999999998%" headers="mcps1.1.5.1.1 "><p id="p22301333165015"><a name="p22301333165015"></a><a name="p22301333165015"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="15.36%" headers="mcps1.1.5.1.2 "><p id="p942481041718"><a name="p942481041718"></a><a name="p942481041718"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="28.470000000000002%" headers="mcps1.1.5.1.3 "><p id="p10230433115013"><a name="p10230433115013"></a><a name="p10230433115013"></a>邻居节点数。</p>
</td>
<td class="cellrowborder" valign="top" width="38.07%" headers="mcps1.1.5.1.4 "><p id="p129897813251"><a name="p129897813251"></a><a name="p129897813251"></a>[11,499]</p>
</td>
</tr>
<tr id="row14667192918485"><td class="cellrowborder" valign="top" width="18.099999999999998%" headers="mcps1.1.5.1.1 "><p id="p116802032174613"><a name="p116802032174613"></a><a name="p116802032174613"></a>L</p>
</td>
<td class="cellrowborder" valign="top" width="15.36%" headers="mcps1.1.5.1.2 "><p id="p1242415108176"><a name="p1242415108176"></a><a name="p1242415108176"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="28.470000000000002%" headers="mcps1.1.5.1.3 "><p id="p268013224617"><a name="p268013224617"></a><a name="p268013224617"></a>构图时的候选节点列表大小。</p>
</td>
<td class="cellrowborder" valign="top" width="38.07%" headers="mcps1.1.5.1.4 "><p id="p6989158192510"><a name="p6989158192510"></a><a name="p6989158192510"></a>[11,1999]</p>
</td>
</tr>
<tr id="row17551732134814"><td class="cellrowborder" valign="top" width="18.099999999999998%" headers="mcps1.1.5.1.1 "><p id="p4597734184616"><a name="p4597734184616"></a><a name="p4597734184616"></a>A</p>
</td>
<td class="cellrowborder" valign="top" width="15.36%" headers="mcps1.1.5.1.2 "><p id="p2424101041714"><a name="p2424101041714"></a><a name="p2424101041714"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="28.470000000000002%" headers="mcps1.1.5.1.3 "><p id="p65975343465"><a name="p65975343465"></a><a name="p65975343465"></a>构图剪枝时的角度阈值。</p>
</td>
<td class="cellrowborder" valign="top" width="38.07%" headers="mcps1.1.5.1.4 "><p id="p16989883251"><a name="p16989883251"></a><a name="p16989883251"></a>[11,360]</p>
</td>
</tr>
<tr id="row188092073209"><td class="cellrowborder" valign="top" width="18.099999999999998%" headers="mcps1.1.5.1.1 "><p id="p9161114132017"><a name="p9161114132017"></a><a name="p9161114132017"></a>graph_opt_iter</p>
</td>
<td class="cellrowborder" valign="top" width="15.36%" headers="mcps1.1.5.1.2 "><p id="p18809137102014"><a name="p18809137102014"></a><a name="p18809137102014"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="28.470000000000002%" headers="mcps1.1.5.1.3 "><p id="p51611714162017"><a name="p51611714162017"></a><a name="p51611714162017"></a>图索引自我迭代的轮数。</p>
</td>
<td class="cellrowborder" valign="top" width="38.07%" headers="mcps1.1.5.1.4 "><p id="p180911714202"><a name="p180911714202"></a><a name="p180911714202"></a>[0,30]</p>
</td>
</tr>
<tr id="row523013315504"><td class="cellrowborder" valign="top" width="18.099999999999998%" headers="mcps1.1.5.1.1 "><p id="p10230123316509"><a name="p10230123316509"></a><a name="p10230123316509"></a>metric</p>
</td>
<td class="cellrowborder" valign="top" width="15.36%" headers="mcps1.1.5.1.2 "><p id="p19424710151712"><a name="p19424710151712"></a><a name="p19424710151712"></a>字符串</p>
</td>
<td class="cellrowborder" valign="top" width="28.470000000000002%" headers="mcps1.1.5.1.3 "><p id="p102301133105015"><a name="p102301133105015"></a><a name="p102301133105015"></a>距离度量的方式。其中，</p>
</td>
<td class="cellrowborder" valign="top" width="38.07%" headers="mcps1.1.5.1.4 "><p id="p16989188132515"><a name="p16989188132515"></a><a name="p16989188132515"></a><span class="parmvalue" id="parmvalue07091746125712"><a name="parmvalue07091746125712"></a><a name="parmvalue07091746125712"></a>“L2”</span>或<span class="parmvalue" id="parmvalue112105525575"><a name="parmvalue112105525575"></a><a name="parmvalue112105525575"></a>“IP”</span>。</p>
<a name="ul194922278186"></a><a name="ul194922278186"></a><ul id="ul194922278186"><li><span class="parmvalue" id="parmvalue14698175535715"><a name="parmvalue14698175535715"></a><a name="parmvalue14698175535715"></a>“L2”</span>为欧几里得距离。</li><li><span class="parmvalue" id="parmvalue20513559115717"><a name="parmvalue20513559115717"></a><a name="parmvalue20513559115717"></a>“IP”</span>为内积距离。</li></ul>
</td>
</tr>
<tr id="row1523083315012"><td class="cellrowborder" valign="top" width="18.099999999999998%" headers="mcps1.1.5.1.1 "><p id="p10230433105020"><a name="p10230433105020"></a><a name="p10230433105020"></a>init_builder_type</p>
</td>
<td class="cellrowborder" valign="top" width="15.36%" headers="mcps1.1.5.1.2 "><p id="p34241210171720"><a name="p34241210171720"></a><a name="p34241210171720"></a>字符串</p>
</td>
<td class="cellrowborder" valign="top" width="28.470000000000002%" headers="mcps1.1.5.1.3 "><p id="p623053365015"><a name="p623053365015"></a><a name="p623053365015"></a>构建k近邻图的算法。</p>
</td>
<td class="cellrowborder" valign="top" width="38.07%" headers="mcps1.1.5.1.4 "><p id="p9989158112520"><a name="p9989158112520"></a><a name="p9989158112520"></a><span class="parmvalue" id="parmvalue122210335814"><a name="parmvalue122210335814"></a><a name="parmvalue122210335814"></a>“RNNDescent”</span>和<span class="parmvalue" id="parmvalue1521813710584"><a name="parmvalue1521813710584"></a><a name="parmvalue1521813710584"></a>“NNDescent”</span>，表示两种不同的构建k近邻图的算法，推荐使用<span class="parmvalue" id="parmvalue47521111175812"><a name="parmvalue47521111175812"></a><a name="parmvalue47521111175812"></a>“RNNDescent”</span>。</p>
</td>
</tr>
<tr id="row19521191612225"><td class="cellrowborder" valign="top" width="18.099999999999998%" headers="mcps1.1.5.1.1 "><p id="p1546185591017"><a name="p1546185591017"></a><a name="p1546185591017"></a>index_type</p>
</td>
<td class="cellrowborder" valign="top" width="15.36%" headers="mcps1.1.5.1.2 "><p id="p19131103031011"><a name="p19131103031011"></a><a name="p19131103031011"></a>字符串</p>
</td>
<td class="cellrowborder" valign="top" width="28.470000000000002%" headers="mcps1.1.5.1.3 "><p id="p55461255161011"><a name="p55461255161011"></a><a name="p55461255161011"></a>选择邻居策略。</p>
</td>
<td class="cellrowborder" valign="top" width="38.07%" headers="mcps1.1.5.1.4 "><p id="p213293001016"><a name="p213293001016"></a><a name="p213293001016"></a><span class="parmvalue" id="parmvalue3260403116"><a name="parmvalue3260403116"></a><a name="parmvalue3260403116"></a>“HNSW”</span><span>或</span><span class="parmvalue" id="parmvalue41171544161114"><a name="parmvalue41171544161114"></a><a name="parmvalue41171544161114"></a>“NSG”</span><span>或</span><span class="parmvalue" id="parmvalue1739675061118"><a name="parmvalue1739675061118"></a><a name="parmvalue1739675061118"></a>“TSDG”</span><span>或</span><span class="parmvalue" id="parmvalue5852453141117"><a name="parmvalue5852453141117"></a><a name="parmvalue5852453141117"></a>“SSG”</span>，表示四种不同的选择邻居策略。</p>
</td>
</tr>
<tr id="row167566217421"><td class="cellrowborder" valign="top" width="18.099999999999998%" headers="mcps1.1.5.1.1 "><p id="p1575610224213"><a name="p1575610224213"></a><a name="p1575610224213"></a>numa_enabled</p>
</td>
<td class="cellrowborder" valign="top" width="15.36%" headers="mcps1.1.5.1.2 "><p id="p16424121021718"><a name="p16424121021718"></a><a name="p16424121021718"></a>布尔值</p>
</td>
<td class="cellrowborder" valign="top" width="28.470000000000002%" headers="mcps1.1.5.1.3 "><p id="p87563211420"><a name="p87563211420"></a><a name="p87563211420"></a>是否开启NUMA优化。</p>
</td>
<td class="cellrowborder" valign="top" width="38.07%" headers="mcps1.1.5.1.4 "><p id="p1262653354620"><a name="p1262653354620"></a><a name="p1262653354620"></a>-</p>
</td>
</tr>
<tr id="row1020145194211"><td class="cellrowborder" valign="top" width="18.099999999999998%" headers="mcps1.1.5.1.1 "><p id="p1620145194210"><a name="p1620145194210"></a><a name="p1620145194210"></a>numa_nodes_number</p>
</td>
<td class="cellrowborder" valign="top" width="15.36%" headers="mcps1.1.5.1.2 "><p id="p4424410171711"><a name="p4424410171711"></a><a name="p4424410171711"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="28.470000000000002%" headers="mcps1.1.5.1.3 "><p id="p13201125144212"><a name="p13201125144212"></a><a name="p13201125144212"></a>使用的NUMA节点数量。</p>
</td>
<td class="cellrowborder" valign="top" width="38.07%" headers="mcps1.1.5.1.4 "><p id="p13626333134613"><a name="p13626333134613"></a><a name="p13626333134613"></a>大于等于1。</p>
</td>
</tr>
</tbody>
</table>

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
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="18.05%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.75%" id="mcps1.1.5.1.2"><p id="p117938514184"><a name="p117938514184"></a><a name="p117938514184"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="26.69%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="37.51%" id="mcps1.1.5.1.4"><p id="p18686165314813"><a name="p18686165314813"></a><a name="p18686165314813"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="18.05%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>nb</p>
</td>
<td class="cellrowborder" valign="top" width="17.75%" headers="mcps1.1.5.1.2 "><p id="p679315141818"><a name="p679315141818"></a><a name="p679315141818"></a><span>int</span></p>
</td>
<td class="cellrowborder" valign="top" width="26.69%" headers="mcps1.1.5.1.3 "><p id="p182303331508"><a name="p182303331508"></a><a name="p182303331508"></a>向量底库数据量。</p>
</td>
<td class="cellrowborder" valign="top" width="37.51%" headers="mcps1.1.5.1.4 "><p id="p1151275553412"><a name="p1151275553412"></a><a name="p1151275553412"></a>大于等于1。建议小于10亿。</p>
</td>
</tr>
<tr id="row11230173385019"><td class="cellrowborder" valign="top" width="18.05%" headers="mcps1.1.5.1.1 "><p id="p22301333165015"><a name="p22301333165015"></a><a name="p22301333165015"></a>xb</p>
</td>
<td class="cellrowborder" valign="top" width="17.75%" headers="mcps1.1.5.1.2 "><p id="p4793135121812"><a name="p4793135121812"></a><a name="p4793135121812"></a>numpy.ndarray</p>
</td>
<td class="cellrowborder" valign="top" width="26.69%" headers="mcps1.1.5.1.3 "><p id="p10230433115013"><a name="p10230433115013"></a><a name="p10230433115013"></a>向量底库数据。</p>
</td>
<td class="cellrowborder" valign="top" width="37.51%" headers="mcps1.1.5.1.4 "><p id="p1218364610343"><a name="p1218364610343"></a><a name="p1218364610343"></a>限制非空，长度应为nb * dim（数据量 * 特征维度）。</p>
</td>
</tr>
<tr id="row92309336505"><td class="cellrowborder" valign="top" width="18.05%" headers="mcps1.1.5.1.1 "><p id="p162309336505"><a name="p162309336505"></a><a name="p162309336505"></a>consecutive</p>
</td>
<td class="cellrowborder" valign="top" width="17.75%" headers="mcps1.1.5.1.2 "><p id="p3793145191818"><a name="p3793145191818"></a><a name="p3793145191818"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="26.69%" headers="mcps1.1.5.1.3 "><p id="p92301933165017"><a name="p92301933165017"></a><a name="p92301933165017"></a>块大小。</p>
</td>
<td class="cellrowborder" valign="top" width="37.51%" headers="mcps1.1.5.1.4 "><p id="p1151265503419"><a name="p1151265503419"></a><a name="p1151265503419"></a>[1,31]</p>
</td>
</tr>
<tr id="row11317866249"><td class="cellrowborder" valign="top" width="18.05%" headers="mcps1.1.5.1.1 "><p id="p1231811620244"><a name="p1231811620244"></a><a name="p1231811620244"></a><span>reorder</span></p>
</td>
<td class="cellrowborder" valign="top" width="17.75%" headers="mcps1.1.5.1.2 "><p id="p5318860247"><a name="p5318860247"></a><a name="p5318860247"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="26.69%" headers="mcps1.1.5.1.3 "><p id="p631856102414"><a name="p631856102414"></a><a name="p631856102414"></a>是否开启底库向量重排。</p>
</td>
<td class="cellrowborder" valign="top" width="37.51%" headers="mcps1.1.5.1.4 "><p id="p231813619242"><a name="p231813619242"></a><a name="p231813619242"></a>0或1。</p>
</td>
</tr>
<tr id="row523013315504"><td class="cellrowborder" valign="top" width="18.05%" headers="mcps1.1.5.1.1 "><p id="p10230123316509"><a name="p10230123316509"></a><a name="p10230123316509"></a>level</p>
</td>
<td class="cellrowborder" valign="top" width="17.75%" headers="mcps1.1.5.1.2 "><p id="p3793051201812"><a name="p3793051201812"></a><a name="p3793051201812"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="26.69%" headers="mcps1.1.5.1.3 "><p id="p102301133105015"><a name="p102301133105015"></a><a name="p102301133105015"></a>控制量化的等级。</p>
</td>
<td class="cellrowborder" valign="top" width="37.51%" headers="mcps1.1.5.1.4 "><p id="p1051225510340"><a name="p1051225510340"></a><a name="p1051225510340"></a>[0,3]</p>
<a name="ul1454195619238"></a><a name="ul1454195619238"></a><ul id="ul1454195619238"><li>0：表示FP32量化。</li><li>1：表示SQ8U量化。</li><li>2：表示SQ4U量化。</li><li>3：表示FP16量化。</li></ul>
</td>
</tr>
</tbody>
</table>

**返回值<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>
<table><thead align="left"><tr id="row1569152711463"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p146911527174618"><a name="p146911527174618"></a><a name="p146911527174618"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p136911627194618"><a name="p136911627194618"></a><a name="p136911627194618"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row769192744612"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p106910272463"><a name="p106910272463"></a><a name="p106910272463"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p2611111352313"><a name="p2611111352313"></a><a name="p2611111352313"></a>接口由底层C++接口封装而来。异常抛出由底层C++接口控制。</p>
</td>
</tr>
</tbody>
</table>

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
<table><thead align="left"><tr id="row1569152711463"><th class="cellrowborder" valign="top" width="34.599999999999994%" id="mcps1.1.3.1.1"><p id="p146911527174618"><a name="p146911527174618"></a><a name="p146911527174618"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="65.4%" id="mcps1.1.3.1.2"><p id="p136911627194618"><a name="p136911627194618"></a><a name="p136911627194618"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row769192744612"><td class="cellrowborder" valign="top" width="34.599999999999994%" headers="mcps1.1.3.1.1 "><p id="p106910272463"><a name="p106910272463"></a><a name="p106910272463"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="65.4%" headers="mcps1.1.3.1.2 "><p id="p17947191512276"><a name="p17947191512276"></a><a name="p17947191512276"></a>接口由底层C++接口封装而来，异常抛出由底层C++接口控制。</p>
</td>
</tr>
</tbody>
</table>

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
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="14.14%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="21.36%" id="mcps1.1.5.1.2"><p id="p1192894081911"><a name="p1192894081911"></a><a name="p1192894081911"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="28.65%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="35.85%" id="mcps1.1.5.1.4"><p id="p18686165314813"><a name="p18686165314813"></a><a name="p18686165314813"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>nq</p>
</td>
<td class="cellrowborder" valign="top" width="21.36%" headers="mcps1.1.5.1.2 "><p id="p179282406193"><a name="p179282406193"></a><a name="p179282406193"></a><span>int</span></p>
</td>
<td class="cellrowborder" valign="top" width="28.65%" headers="mcps1.1.5.1.3 "><p id="p182303331508"><a name="p182303331508"></a><a name="p182303331508"></a>查询向量集数据量。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85%" headers="mcps1.1.5.1.4 "><p id="p1446074319406"><a name="p1446074319406"></a><a name="p1446074319406"></a>大于等于1。建议小于10亿。</p>
</td>
</tr>
<tr id="row11230173385019"><td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.1.5.1.1 "><p id="p22301333165015"><a name="p22301333165015"></a><a name="p22301333165015"></a>xq</p>
</td>
<td class="cellrowborder" valign="top" width="21.36%" headers="mcps1.1.5.1.2 "><p id="p1792864071912"><a name="p1792864071912"></a><a name="p1792864071912"></a>numpy.ndarray</p>
</td>
<td class="cellrowborder" valign="top" width="28.65%" headers="mcps1.1.5.1.3 "><p id="p10230433115013"><a name="p10230433115013"></a><a name="p10230433115013"></a>查询向量集数据。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85%" headers="mcps1.1.5.1.4 "><p id="p19460943204013"><a name="p19460943204013"></a><a name="p19460943204013"></a>限制非空，<span>期待长度为nq * dim</span>（数据量 * 特征维度）。</p>
</td>
</tr>
<tr id="row92309336505"><td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.1.5.1.1 "><p id="p162309336505"><a name="p162309336505"></a><a name="p162309336505"></a>topk</p>
</td>
<td class="cellrowborder" valign="top" width="21.36%" headers="mcps1.1.5.1.2 "><p id="p692844014192"><a name="p692844014192"></a><a name="p692844014192"></a><span>int</span></p>
</td>
<td class="cellrowborder" valign="top" width="28.65%" headers="mcps1.1.5.1.3 "><p id="p92301933165017"><a name="p92301933165017"></a><a name="p92301933165017"></a>最近邻的数量。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85%" headers="mcps1.1.5.1.4 "><p id="p1178758184115"><a name="p1178758184115"></a><a name="p1178758184115"></a>[1,nb]，其中<span class="parmname" id="parmname201022052769"><a name="parmname201022052769"></a><a name="parmname201022052769"></a>“nb”</span>为向量底库数据量大小。</p>
</td>
</tr>
<tr id="row33251301573"><td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.1.5.1.1 "><p id="p83251102715"><a name="p83251102715"></a><a name="p83251102715"></a><span>distances</span></p>
</td>
<td class="cellrowborder" valign="top" width="21.36%" headers="mcps1.1.5.1.2 "><p id="p9928140121918"><a name="p9928140121918"></a><a name="p9928140121918"></a>numpy.ndarray</p>
</td>
<td class="cellrowborder" valign="top" width="28.65%" headers="mcps1.1.5.1.3 "><p id="p8325130776"><a name="p8325130776"></a><a name="p8325130776"></a>距离数组。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85%" headers="mcps1.1.5.1.4 "><p id="p1218364610343"><a name="p1218364610343"></a><a name="p1218364610343"></a>限制非空，<span>期待长度为nq * topk</span>。</p>
</td>
</tr>
<tr id="row17889102871"><td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.1.5.1.1 "><p id="p1188922077"><a name="p1188922077"></a><a name="p1188922077"></a>labels</p>
</td>
<td class="cellrowborder" valign="top" width="21.36%" headers="mcps1.1.5.1.2 "><p id="p14928164014191"><a name="p14928164014191"></a><a name="p14928164014191"></a>numpy.ndarray</p>
</td>
<td class="cellrowborder" valign="top" width="28.65%" headers="mcps1.1.5.1.3 "><p id="p1889122372"><a name="p1889122372"></a><a name="p1889122372"></a>检索结果的ID数组。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85%" headers="mcps1.1.5.1.4 "><p id="p13889132574"><a name="p13889132574"></a><a name="p13889132574"></a>限制非空，<span>期待长度为nq * topk</span>。</p>
</td>
</tr>
<tr id="row177151948121320"><td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.1.5.1.1 "><p id="p3715448191319"><a name="p3715448191319"></a><a name="p3715448191319"></a>num_threads</p>
</td>
<td class="cellrowborder" valign="top" width="21.36%" headers="mcps1.1.5.1.2 "><p id="p5928440101919"><a name="p5928440101919"></a><a name="p5928440101919"></a><span>int</span></p>
</td>
<td class="cellrowborder" valign="top" width="28.65%" headers="mcps1.1.5.1.3 "><p id="p137151148161319"><a name="p137151148161319"></a><a name="p137151148161319"></a>检索时使用的线程数。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85%" headers="mcps1.1.5.1.4 "><p id="p95801533174311"><a name="p95801533174311"></a><a name="p95801533174311"></a>[1,std::thread::hardware_concurrency()]，其中std::thread::hardware_concurrency()为<span>当前系统支持的并发线程数</span>。</p>
</td>
</tr>
</tbody>
</table>

**返回值<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>
<table><thead align="left"><tr id="row1569152711463"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p146911527174618"><a name="p146911527174618"></a><a name="p146911527174618"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p136911627194618"><a name="p136911627194618"></a><a name="p136911627194618"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row769192744612"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p106910272463"><a name="p106910272463"></a><a name="p106910272463"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p2611111352313"><a name="p2611111352313"></a><a name="p2611111352313"></a>接口由底层C++接口封装而来，异常抛出由底层C++接口控制。</p>
</td>
</tr>
</tbody>
</table>

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
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="14.08%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="22.64%" id="mcps1.1.5.1.2"><p id="p854220356207"><a name="p854220356207"></a><a name="p854220356207"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="26.810000000000002%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="36.47%" id="mcps1.1.5.1.4"><p id="p1440932116441"><a name="p1440932116441"></a><a name="p1440932116441"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="14.08%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>ef</p>
</td>
<td class="cellrowborder" valign="top" width="22.64%" headers="mcps1.1.5.1.2 "><p id="p1754243572014"><a name="p1754243572014"></a><a name="p1754243572014"></a><span>int</span></p>
</td>
<td class="cellrowborder" valign="top" width="26.810000000000002%" headers="mcps1.1.5.1.3 "><p id="p39711451181514"><a name="p39711451181514"></a><a name="p39711451181514"></a>检索时的候选节点列表大小。</p>
</td>
<td class="cellrowborder" valign="top" width="36.47%" headers="mcps1.1.5.1.4 "><p id="p1667165924518"><a name="p1667165924518"></a><a name="p1667165924518"></a>[1,nb]，其中<span class="parmname" id="parmname336535516614"><a name="parmname336535516614"></a><a name="parmname336535516614"></a>“nb”</span>为向量底库数据量大小。</p>
</td>
</tr>
</tbody>
</table>

**返回值<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>
<table><thead align="left"><tr id="row1569152711463"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p146911527174618"><a name="p146911527174618"></a><a name="p146911527174618"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p136911627194618"><a name="p136911627194618"></a><a name="p136911627194618"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row769192744612"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p106910272463"><a name="p106910272463"></a><a name="p106910272463"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p2611111352313"><a name="p2611111352313"></a><a name="p2611111352313"></a>接口由底层C++接口封装而来，异常抛出由底层C++接口控制。</p>
</td>
</tr>
</tbody>
</table>

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
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="16.009999999999998%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="19.49%" id="mcps1.1.5.1.2"><p id="p8128856112017"><a name="p8128856112017"></a><a name="p8128856112017"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="30.12%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="34.38%" id="mcps1.1.5.1.4"><p id="p1440932116441"><a name="p1440932116441"></a><a name="p1440932116441"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="16.009999999999998%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>path</p>
</td>
<td class="cellrowborder" valign="top" width="19.49%" headers="mcps1.1.5.1.2 "><p id="p1112855612010"><a name="p1112855612010"></a><a name="p1112855612010"></a>字符串</p>
</td>
<td class="cellrowborder" valign="top" width="30.12%" headers="mcps1.1.5.1.3 "><p id="p39711451181514"><a name="p39711451181514"></a><a name="p39711451181514"></a>检索器的保存路径。</p>
</td>
<td class="cellrowborder" valign="top" width="34.38%" headers="mcps1.1.5.1.4 "><p id="p20167131514510"><a name="p20167131514510"></a><a name="p20167131514510"></a>取值长度小于199字符。</p>
</td>
</tr>
</tbody>
</table>

**返回值<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>
<table><thead align="left"><tr id="row1569152711463"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p146911527174618"><a name="p146911527174618"></a><a name="p146911527174618"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p136911627194618"><a name="p136911627194618"></a><a name="p136911627194618"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row769192744612"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p106910272463"><a name="p106910272463"></a><a name="p106910272463"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p2611111352313"><a name="p2611111352313"></a><a name="p2611111352313"></a>接口由底层C++接口封装而来，异常抛出由底层C++接口控制。</p>
</td>
</tr>
</tbody>
</table>

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
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="17.21%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="18.82%" id="mcps1.1.5.1.2"><p id="p8128856112017"><a name="p8128856112017"></a><a name="p8128856112017"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="29.74%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="34.23%" id="mcps1.1.5.1.4"><p id="p1440932116441"><a name="p1440932116441"></a><a name="p1440932116441"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="17.21%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>path</p>
</td>
<td class="cellrowborder" valign="top" width="18.82%" headers="mcps1.1.5.1.2 "><p id="p1112855612010"><a name="p1112855612010"></a><a name="p1112855612010"></a>字符串</p>
</td>
<td class="cellrowborder" valign="top" width="29.74%" headers="mcps1.1.5.1.3 "><p id="p39711451181514"><a name="p39711451181514"></a><a name="p39711451181514"></a>检索器的加载路径。</p>
</td>
<td class="cellrowborder" valign="top" width="34.23%" headers="mcps1.1.5.1.4 "><p id="p20167131514510"><a name="p20167131514510"></a><a name="p20167131514510"></a>取值长度小于199字符。</p>
</td>
</tr>
</tbody>
</table>

**返回值<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p19997736105"><a name="p19997736105"></a><a name="p19997736105"></a>接口由底层C++接口封装而来，异常抛出由底层C++接口控制。</p>
</td>
</tr>
</tbody>
</table>

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
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="16.20837916208379%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="20.3979602039796%" id="mcps1.1.5.1.2"><p id="p8128856112017"><a name="p8128856112017"></a><a name="p8128856112017"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="27.947205279472055%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="35.446455354464554%" id="mcps1.1.5.1.4"><p id="p1440932116441"><a name="p1440932116441"></a><a name="p1440932116441"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="16.20837916208379%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>path</p>
</td>
<td class="cellrowborder" valign="top" width="20.3979602039796%" headers="mcps1.1.5.1.2 "><p id="p1112855612010"><a name="p1112855612010"></a><a name="p1112855612010"></a>字符串</p>
</td>
<td class="cellrowborder" valign="top" width="27.947205279472055%" headers="mcps1.1.5.1.3 "><p id="p39711451181514"><a name="p39711451181514"></a><a name="p39711451181514"></a>图索引的保存路径。</p>
</td>
<td class="cellrowborder" valign="top" width="35.446455354464554%" headers="mcps1.1.5.1.4 "><p id="p20167131514510"><a name="p20167131514510"></a><a name="p20167131514510"></a>取值长度小于199字符。</p>
</td>
</tr>
</tbody>
</table>

**返回值<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>
<table><thead align="left"><tr id="row1569152711463"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p146911527174618"><a name="p146911527174618"></a><a name="p146911527174618"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p136911627194618"><a name="p136911627194618"></a><a name="p136911627194618"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row769192744612"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p106910272463"><a name="p106910272463"></a><a name="p106910272463"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p2611111352313"><a name="p2611111352313"></a><a name="p2611111352313"></a>接口由底层C++接口封装而来，异常抛出由底层C++接口控制。</p>
</td>
</tr>
</tbody>
</table>

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
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.14%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.91%" id="mcps1.1.5.1.2"><p id="p8128856112017"><a name="p8128856112017"></a><a name="p8128856112017"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="21.78%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="45.17%" id="mcps1.1.5.1.4"><p id="p1440932116441"><a name="p1440932116441"></a><a name="p1440932116441"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.14%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>path</p>
</td>
<td class="cellrowborder" valign="top" width="17.91%" headers="mcps1.1.5.1.2 "><p id="p1112855612010"><a name="p1112855612010"></a><a name="p1112855612010"></a>字符串</p>
</td>
<td class="cellrowborder" valign="top" width="21.78%" headers="mcps1.1.5.1.3 "><p id="p39711451181514"><a name="p39711451181514"></a><a name="p39711451181514"></a>检索器的加载路径。</p>
</td>
<td class="cellrowborder" valign="top" width="45.17%" headers="mcps1.1.5.1.4 "><p id="p20167131514510"><a name="p20167131514510"></a><a name="p20167131514510"></a>取值长度小于199字符。</p>
</td>
</tr>
<tr id="row412192193411"><td class="cellrowborder" valign="top" width="15.14%" headers="mcps1.1.5.1.1 "><p id="p19414810153017"><a name="p19414810153017"></a><a name="p19414810153017"></a>level</p>
</td>
<td class="cellrowborder" valign="top" width="17.91%" headers="mcps1.1.5.1.2 "><p id="p17614134914213"><a name="p17614134914213"></a><a name="p17614134914213"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="21.78%" headers="mcps1.1.5.1.3 "><p id="p5414151014309"><a name="p5414151014309"></a><a name="p5414151014309"></a>控制量化的等级。</p>
</td>
<td class="cellrowborder" valign="top" width="45.17%" headers="mcps1.1.5.1.4 "><p id="p14665102215"><a name="p14665102215"></a><a name="p14665102215"></a>[-1,3]</p>
<a name="ul1454195619238"></a><a name="ul1454195619238"></a><ul id="ul1454195619238"><li>-1：默认值，表示saveGraph时保存的量化等级。</li><li>0：表示FP32量化。</li><li>1：表示SQ8U量化。</li><li>2：表示SQ4U量化。</li><li>3：表示FP16量化。</li></ul>
</td>
</tr>
</tbody>
</table>

**返回值<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p19997736105"><a name="p19997736105"></a><a name="p19997736105"></a>接口由底层C++接口封装而来，异常抛出由底层C++接口控制。</p>
</td>
</tr>
</tbody>
</table>

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
<table><thead align="left"><tr id="row1569152711463"><th class="cellrowborder" valign="top" width="36.96%" id="mcps1.1.3.1.1"><p id="p146911527174618"><a name="p146911527174618"></a><a name="p146911527174618"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="63.04%" id="mcps1.1.3.1.2"><p id="p136911627194618"><a name="p136911627194618"></a><a name="p136911627194618"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row769192744612"><td class="cellrowborder" valign="top" width="36.96%" headers="mcps1.1.3.1.1 "><p id="p106910272463"><a name="p106910272463"></a><a name="p106910272463"></a>numpy.ndarray</p>
</td>
<td class="cellrowborder" valign="top" width="63.04%" headers="mcps1.1.3.1.2 "><p id="p14753115604612"><a name="p14753115604612"></a><a name="p14753115604612"></a>存储检索器内容的数组。</p>
</td>
</tr>
</tbody>
</table>

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
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.09%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="16.71%" id="mcps1.1.5.1.2"><p id="p654931862217"><a name="p654931862217"></a><a name="p654931862217"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="21.64%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="46.56%" id="mcps1.1.5.1.4"><p id="p1440932116441"><a name="p1440932116441"></a><a name="p1440932116441"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.09%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>data_arr</p>
</td>
<td class="cellrowborder" valign="top" width="16.71%" headers="mcps1.1.5.1.2 "><p id="p2054931812228"><a name="p2054931812228"></a><a name="p2054931812228"></a>numpy.ndarray</p>
</td>
<td class="cellrowborder" valign="top" width="21.64%" headers="mcps1.1.5.1.3 "><p id="p39711451181514"><a name="p39711451181514"></a><a name="p39711451181514"></a>存储检索器内容的数组。</p>
</td>
<td class="cellrowborder" valign="top" width="46.56%" headers="mcps1.1.5.1.4 "><p id="p20167131514510"><a name="p20167131514510"></a><a name="p20167131514510"></a>存储检索器内容的数组的起始地址限制非空，存储检索器内容的数组的长度限制为serialize接口时保存的数组长度。</p>
</td>
</tr>
</tbody>
</table>

**返回值<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>
<table><thead align="left"><tr id="row1569152711463"><th class="cellrowborder" valign="top" width="36.96%" id="mcps1.1.3.1.1"><p id="p146911527174618"><a name="p146911527174618"></a><a name="p146911527174618"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="63.04%" id="mcps1.1.3.1.2"><p id="p136911627194618"><a name="p136911627194618"></a><a name="p136911627194618"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row769192744612"><td class="cellrowborder" valign="top" width="36.96%" headers="mcps1.1.3.1.1 "><p id="p106910272463"><a name="p106910272463"></a><a name="p106910272463"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="63.04%" headers="mcps1.1.3.1.2 "><p id="p19997736105"><a name="p19997736105"></a><a name="p19997736105"></a>接口由底层C++接口封装而来，异常抛出由底层C++接口控制。</p>
</td>
</tr>
</tbody>
</table>

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
<table><thead align="left"><tr id="row1569152711463"><th class="cellrowborder" valign="top" width="36.96%" id="mcps1.1.3.1.1"><p id="p146911527174618"><a name="p146911527174618"></a><a name="p146911527174618"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="63.04%" id="mcps1.1.3.1.2"><p id="p136911627194618"><a name="p136911627194618"></a><a name="p136911627194618"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row769192744612"><td class="cellrowborder" valign="top" width="36.96%" headers="mcps1.1.3.1.1 "><p id="p106910272463"><a name="p106910272463"></a><a name="p106910272463"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="63.04%" headers="mcps1.1.3.1.2 "><p id="p19997736105"><a name="p19997736105"></a><a name="p19997736105"></a>不添加底库的场景下，默认返回值为0。</p>
</td>
</tr>
</tbody>
</table>

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
<table><thead align="left"><tr id="row1569152711463"><th class="cellrowborder" valign="top" width="36.96%" id="mcps1.1.3.1.1"><p id="p146911527174618"><a name="p146911527174618"></a><a name="p146911527174618"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="63.04%" id="mcps1.1.3.1.2"><p id="p136911627194618"><a name="p136911627194618"></a><a name="p136911627194618"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row769192744612"><td class="cellrowborder" valign="top" width="36.96%" headers="mcps1.1.3.1.1 "><p id="p106910272463"><a name="p106910272463"></a><a name="p106910272463"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="63.04%" headers="mcps1.1.3.1.2 "><p id="p19997736105"><a name="p19997736105"></a><a name="p19997736105"></a>有参构建的场景下等于<span class="parmname" id="parmname8531896718"><a name="parmname8531896718"></a><a name="parmname8531896718"></a>“dim”</span>参数，无参构建的场景或有参构建后调用load/deserialize/loadGraph接口后，返回值为读取的检索器/图索引中的数据的维度。</p>
</td>
</tr>
</tbody>
</table>

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
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="13.44%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="18.360000000000003%" id="mcps1.1.5.1.2"><p id="p654931862217"><a name="p654931862217"></a><a name="p654931862217"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="21.64%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="46.56%" id="mcps1.1.5.1.4"><p id="p1440932116441"><a name="p1440932116441"></a><a name="p1440932116441"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="13.44%" headers="mcps1.1.5.1.1 "><p id="p184071120102610"><a name="p184071120102610"></a><a name="p184071120102610"></a>adding_pref</p>
</td>
<td class="cellrowborder" valign="top" width="18.360000000000003%" headers="mcps1.1.5.1.2 "><p id="p2054931812228"><a name="p2054931812228"></a><a name="p2054931812228"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="21.64%" headers="mcps1.1.5.1.3 "><p id="p0407020102611"><a name="p0407020102611"></a><a name="p0407020102611"></a>超参候选集插入阈值。</p>
</td>
<td class="cellrowborder" valign="top" width="46.56%" headers="mcps1.1.5.1.4 "><p id="p20167131514510"><a name="p20167131514510"></a><a name="p20167131514510"></a>大于等于1。</p>
</td>
</tr>
<tr id="row188955417267"><td class="cellrowborder" valign="top" width="13.44%" headers="mcps1.1.5.1.1 "><p id="p37102045152610"><a name="p37102045152610"></a><a name="p37102045152610"></a>patience</p>
</td>
<td class="cellrowborder" valign="top" width="18.360000000000003%" headers="mcps1.1.5.1.2 "><p id="p1089574110268"><a name="p1089574110268"></a><a name="p1089574110268"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="21.64%" headers="mcps1.1.5.1.3 "><p id="p117109457269"><a name="p117109457269"></a><a name="p117109457269"></a>检索耐心值。</p>
</td>
<td class="cellrowborder" valign="top" width="46.56%" headers="mcps1.1.5.1.4 "><p id="p789514142616"><a name="p789514142616"></a><a name="p789514142616"></a>大于等于1。</p>
</td>
</tr>
</tbody>
</table>

**返回值<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>
<table><thead align="left"><tr id="row1569152711463"><th class="cellrowborder" valign="top" width="36.96%" id="mcps1.1.3.1.1"><p id="p146911527174618"><a name="p146911527174618"></a><a name="p146911527174618"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="63.04%" id="mcps1.1.3.1.2"><p id="p136911627194618"><a name="p136911627194618"></a><a name="p136911627194618"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row769192744612"><td class="cellrowborder" valign="top" width="36.96%" headers="mcps1.1.3.1.1 "><p id="p106910272463"><a name="p106910272463"></a><a name="p106910272463"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="63.04%" headers="mcps1.1.3.1.2 "><p id="p19997736105"><a name="p19997736105"></a><a name="p19997736105"></a>接口由底层C++接口封装而来，异常抛出由底层C++接口控制。</p>
</td>
</tr>
</tbody>
</table>

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
