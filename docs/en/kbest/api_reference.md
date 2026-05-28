# API Reference

## C++

### API Description

[**Table 1**](#c++-apis-provided-by-KBest) describes the C++ APIs provided by KBest.

**Table 1** C++ APIs provided by KBest<a id="c++-apis-provided-by-KBest"></a>

<a name="table1194910128449"></a>
<table><thead align="left"><tr id="row99491812134412"><th class="cellrowborder" valign="top" width="34.38%" id="mcps1.2.3.1.1"><p id="p1794951224415"><a name="p1794951224415"></a><a name="p1794951224415"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="65.62%" id="mcps1.2.3.1.2"><p id="p6949612124415"><a name="p6949612124415"></a><a name="p6949612124415"></a>Function</p>
</th>
</tr>
</thead>
<tbody><tr id="row119491112174414"><td class="cellrowborder" valign="top" width="34.38%" headers="mcps1.2.3.1.1 "><p id="p1494931224410"><a name="p1494931224410"></a><a name="p1494931224410"></a>KBest</p>
</td>
<td class="cellrowborder" valign="top" width="65.62%" headers="mcps1.2.3.1.2 "><p id="p3949012174411"><a name="p3949012174411"></a><a name="p3949012174411"></a>Initializes the build of graph search (via default or parameterized constructor).</p>
</td>
</tr>
<tr id="row9949131219443"><td class="cellrowborder" valign="top" width="34.38%" headers="mcps1.2.3.1.1 "><p id="p1094921294415"><a name="p1094921294415"></a><a name="p1094921294415"></a>Add</p>
</td>
<td class="cellrowborder" valign="top" width="65.62%" headers="mcps1.2.3.1.2 "><p id="p1794941284418"><a name="p1794941284418"></a><a name="p1794941284418"></a>Builds a graph index.</p>
</td>
</tr>
<tr id="row379293619370"><td class="cellrowborder" valign="top" width="34.38%" headers="mcps1.2.3.1.1 "><p id="p10792123618373"><a name="p10792123618373"></a><a name="p10792123618373"></a>BuildSearcher</p>
</td>
<td class="cellrowborder" valign="top" width="65.62%" headers="mcps1.2.3.1.2 "><p id="p379243633713"><a name="p379243633713"></a><a name="p379243633713"></a>Builds a searcher.</p>
</td>
</tr>
<tr id="row1594913120443"><td class="cellrowborder" valign="top" width="34.38%" headers="mcps1.2.3.1.1 "><p id="p4949012144417"><a name="p4949012144417"></a><a name="p4949012144417"></a>Search</p>
</td>
<td class="cellrowborder" valign="top" width="65.62%" headers="mcps1.2.3.1.2 "><p id="p594911128445"><a name="p594911128445"></a><a name="p594911128445"></a>Searches for a graph.</p>
</td>
</tr>
<tr id="row6949131274416"><td class="cellrowborder" valign="top" width="34.38%" headers="mcps1.2.3.1.1 "><p id="p594971224411"><a name="p594971224411"></a><a name="p594971224411"></a>SetEf</p>
</td>
<td class="cellrowborder" valign="top" width="65.62%" headers="mcps1.2.3.1.2 "><p id="p794971214414"><a name="p794971214414"></a><a name="p794971214414"></a>Sets the size of a candidate node list during search.</p>
</td>
</tr>
<tr id="row694916124445"><td class="cellrowborder" valign="top" width="34.38%" headers="mcps1.2.3.1.1 "><p id="p8949131214448"><a name="p8949131214448"></a><a name="p8949131214448"></a>Save</p>
</td>
<td class="cellrowborder" valign="top" width="65.62%" headers="mcps1.2.3.1.2 "><p id="p894941210443"><a name="p894941210443"></a><a name="p894941210443"></a>Saves the searcher to a specified path.</p>
</td>
</tr>
<tr id="row159491712174414"><td class="cellrowborder" valign="top" width="34.38%" headers="mcps1.2.3.1.1 "><p id="p894991214449"><a name="p894991214449"></a><a name="p894991214449"></a>Load</p>
</td>
<td class="cellrowborder" valign="top" width="65.62%" headers="mcps1.2.3.1.2 "><p id="p2094917128448"><a name="p2094917128448"></a><a name="p2094917128448"></a>Loads the searcher from the specified path.</p>
</td>
</tr>
<tr id="row184131856399"><td class="cellrowborder" valign="top" width="34.38%" headers="mcps1.2.3.1.1 "><p id="p935410178398"><a name="p935410178398"></a><a name="p935410178398"></a>SaveGraph</p>
</td>
<td class="cellrowborder" valign="top" width="65.62%" headers="mcps1.2.3.1.2 "><p id="p113548174390"><a name="p113548174390"></a><a name="p113548174390"></a>Saves the graph index to a specified path.</p>
</td>
</tr>
<tr id="row1587810973913"><td class="cellrowborder" valign="top" width="34.38%" headers="mcps1.2.3.1.1 "><p id="p0355121763910"><a name="p0355121763910"></a><a name="p0355121763910"></a>LoadGraph</p>
</td>
<td class="cellrowborder" valign="top" width="65.62%" headers="mcps1.2.3.1.2 "><p id="p12355117103918"><a name="p12355117103918"></a><a name="p12355117103918"></a>Loads the graph index from the specified path.</p>
</td>
</tr>
<tr id="row78159104213"><td class="cellrowborder" valign="top" width="34.38%" headers="mcps1.2.3.1.1 "><p id="p108461119154212"><a name="p108461119154212"></a><a name="p108461119154212"></a>Serialize</p>
</td>
<td class="cellrowborder" valign="top" width="65.62%" headers="mcps1.2.3.1.2 "><p id="p1584621994217"><a name="p1584621994217"></a><a name="p1584621994217"></a>Serializes the searcher content into an array.</p>
</td>
</tr>
<tr id="row123946122423"><td class="cellrowborder" valign="top" width="34.38%" headers="mcps1.2.3.1.1 "><p id="p2846119204220"><a name="p2846119204220"></a><a name="p2846119204220"></a>Deserialize</p>
</td>
<td class="cellrowborder" valign="top" width="65.62%" headers="mcps1.2.3.1.2 "><p id="p3403194411458"><a name="p3403194411458"></a><a name="p3403194411458"></a>Deserializes and restores the searcher content from the array.</p>
</td>
</tr>
<tr id="row968819494476"><td class="cellrowborder" valign="top" width="34.38%" headers="mcps1.2.3.1.1 "><p id="p7688749124717"><a name="p7688749124717"></a><a name="p7688749124717"></a>GetNTotal</p>
</td>
<td class="cellrowborder" valign="top" width="65.62%" headers="mcps1.2.3.1.2 "><p id="p668874918478"><a name="p668874918478"></a><a name="p668874918478"></a>Returns the total number of data entries in the database within the graph index.</p>
</td>
</tr>
<tr id="row89311814810"><td class="cellrowborder" valign="top" width="34.38%" headers="mcps1.2.3.1.1 "><p id="p09312186486"><a name="p09312186486"></a><a name="p09312186486"></a>GetDim</p>
</td>
<td class="cellrowborder" valign="top" width="65.62%" headers="mcps1.2.3.1.2 "><p id="p39310182489"><a name="p39310182489"></a><a name="p39310182489"></a>Returns the dimensionality of the data in the graph index.</p>
</td>
</tr>
<tr id="row170810446223"><td class="cellrowborder" valign="top" width="34.38%" headers="mcps1.2.3.1.1 "><p id="p227124617229"><a name="p227124617229"></a><a name="p227124617229"></a>SetEarlyStoppingParams</p>
</td>
<td class="cellrowborder" valign="top" width="65.62%" headers="mcps1.2.3.1.2 "><p id="p87099445228"><a name="p87099445228"></a><a name="p87099445228"></a>Sets the parameters for early stopping optimization.</p>
</td>
</tr>
</tbody>
</table>

### Parameterized Constructor

**API Definition <a name="section172317194488"></a>**

KBest\(int dim, int R, int L, int A, const char \*metric, const std::string &init\_builder\_type\);

KBest\(int dim, int R, int L, float A, int graph\_opt\_iter, const std::string &metric, const std::string &init\_builder\_type, const std::string &index\_type\);

**API Function<a name="section1153124784912"></a>**

Initializes the build of graph search.

**Parameter Description <a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.56155615561556%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="13.06130613061306%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="35.52355235523553%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>dim</p>
</td>
<td class="cellrowborder" valign="top" width="13.06130613061306%" headers="mcps1.1.5.1.2 "><p id="p98931015893"><a name="p98931015893"></a><a name="p98931015893"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="35.52355235523553%" headers="mcps1.1.5.1.3 "><p id="p182303331508"><a name="p182303331508"></a><a name="p182303331508"></a>Feature dimension</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>[1, 2999]</p>
</td>
</tr>
<tr id="row11230173385019"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p22301333165015"><a name="p22301333165015"></a><a name="p22301333165015"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="13.06130613061306%" headers="mcps1.1.5.1.2 "><p id="p5893141517919"><a name="p5893141517919"></a><a name="p5893141517919"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="35.52355235523553%" headers="mcps1.1.5.1.3 "><p id="p10230433115013"><a name="p10230433115013"></a><a name="p10230433115013"></a>Number of neighboring nodes</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p129897813251"><a name="p129897813251"></a><a name="p129897813251"></a>[11, 499]</p>
</td>
</tr>
<tr id="row1368063274610"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p116802032174613"><a name="p116802032174613"></a><a name="p116802032174613"></a>L</p>
</td>
<td class="cellrowborder" valign="top" width="13.06130613061306%" headers="mcps1.1.5.1.2 "><p id="p489312151893"><a name="p489312151893"></a><a name="p489312151893"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="35.52355235523553%" headers="mcps1.1.5.1.3 "><p id="p268013224617"><a name="p268013224617"></a><a name="p268013224617"></a>Size of the candidate node list during graph construction</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p6989158192510"><a name="p6989158192510"></a><a name="p6989158192510"></a>[11, 1999]</p>
</td>
</tr>
<tr id="row8597534164617"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p4597734184616"><a name="p4597734184616"></a><a name="p4597734184616"></a>A</p>
</td>
<td class="cellrowborder" valign="top" width="13.06130613061306%" headers="mcps1.1.5.1.2 "><p id="p178931015394"><a name="p178931015394"></a><a name="p178931015394"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="35.52355235523553%" headers="mcps1.1.5.1.3 "><p id="p65975343465"><a name="p65975343465"></a><a name="p65975343465"></a>Angle threshold for pruning during graph construction</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p16989883251"><a name="p16989883251"></a><a name="p16989883251"></a>[11, 360]</p>
</td>
</tr>
<tr id="row523013315504"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p10230123316509"><a name="p10230123316509"></a><a name="p10230123316509"></a>metric</p>
</td>
<td class="cellrowborder" valign="top" width="13.06130613061306%" headers="mcps1.1.5.1.2 "><p id="p2894215596"><a name="p2894215596"></a><a name="p2894215596"></a>const char *</p>
</td>
<td class="cellrowborder" valign="top" width="35.52355235523553%" headers="mcps1.1.5.1.3 "><p id="p102301133105015"><a name="p102301133105015"></a><a name="p102301133105015"></a>Distance metric</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p16989188132515"><a name="p16989188132515"></a><a name="p16989188132515"></a><span class="parmvalue" id="parmvalue12115517324"><a name="parmvalue12115517324"></a><a name="parmvalue12115517324"></a> <code>L2</code></span> or <span class="parmvalue" id="parmvalue18251015195114"><a name="parmvalue18251015195114"></a><a name="parmvalue18251015195114"></a> <code>IP</code></span>.</p>
<a name="ul396901541013"></a><a name="ul396901541013"></a><ul id="ul396901541013"><li><span class="parmvalue" id="parmvalue28857185517"><a name="parmvalue28857185517"></a><a name="parmvalue28857185517"></a> <code>L2</code></span>: Euclidean distance </li><li><span class="parmvalue" id="parmvalue1928610244515"><a name="parmvalue1928610244515"></a><a name="parmvalue1928610244515"></a> <code>IP</code></span>: inner product distance</li></ul>
</td>
</tr>
<tr id="row1523083315012"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p10230433105020"><a name="p10230433105020"></a><a name="p10230433105020"></a>init_builder_type</p>
</td>
<td class="cellrowborder" valign="top" width="13.06130613061306%" headers="mcps1.1.5.1.2 "><p id="p15894141519917"><a name="p15894141519917"></a><a name="p15894141519917"></a>const std::string &amp;</p>
</td>
<td class="cellrowborder" valign="top" width="35.52355235523553%" headers="mcps1.1.5.1.3 "><p id="p623053365015"><a name="p623053365015"></a><a name="p623053365015"></a>Algorithm for constructing the k-nearest neighbor graph</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1946832961016"><a name="p1946832961016"></a><a name="p1946832961016"></a><span class="parmvalue" id="parmvalue176672813511"><a name="parmvalue176672813511"></a><a name="parmvalue176672813511"></a> <code>RNNDescent</code></span> or <span class="parmvalue" id="parmvalue4621549165112"><a name="parmvalue4621549165112"></a><a name="parmvalue4621549165112"></a> <code>NNDescent</code></span>: Each represents an algorithm for constructing the k-nearest neighbor graph. <span class="parmvalue" id="parmvalue534725412518"><a name="parmvalue534725412518"></a><a name="parmvalue534725412518"></a> <code>RNNDescent</code></span> is recommended.</p>
</td>
</tr>
<tr id="row387211011106"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p2023791201011"><a name="p2023791201011"></a><a name="p2023791201011"></a>graph_opt_iter</p>
</td>
<td class="cellrowborder" valign="top" width="13.06130613061306%" headers="mcps1.1.5.1.2 "><p id="p198722006101"><a name="p198722006101"></a><a name="p198722006101"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="35.52355235523553%" headers="mcps1.1.5.1.3 "><p id="p10237212111013"><a name="p10237212111013"></a><a name="p10237212111013"></a>Number of self-iterations for the graph index</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p8872207100"><a name="p8872207100"></a><a name="p8872207100"></a>[0, 30]</p>
</td>
</tr>
<tr id="row7131153011107"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p1546185591017"><a name="p1546185591017"></a><a name="p1546185591017"></a>index_type</p>
</td>
<td class="cellrowborder" valign="top" width="13.06130613061306%" headers="mcps1.1.5.1.2 "><p id="p19131103031011"><a name="p19131103031011"></a><a name="p19131103031011"></a><span>const std::string </span><span>&amp;</span></p>
</td>
<td class="cellrowborder" valign="top" width="35.52355235523553%" headers="mcps1.1.5.1.3 "><p id="p55461255161011"><a name="p55461255161011"></a><a name="p55461255161011"></a>Neighbor selection strategy</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p213293001016"><a name="p213293001016"></a><a name="p213293001016"></a><span class="parmvalue" id="parmvalue3260403116"><a name="parmvalue3260403116"></a><a name="parmvalue3260403116"></a> <code>HNSW</code></span><span>, </span><span class="parmvalue" id="parmvalue41171544161114"><a name="parmvalue41171544161114"></a><a name="parmvalue41171544161114"></a> <code>NSG</code></span><span>, </span><span class="parmvalue" id="parmvalue1739675061118"><a name="parmvalue1739675061118"></a><a name="parmvalue1739675061118"></a> <code>TSDG</code></span><span>, or </span><span class="parmvalue" id="parmvalue5852453141117"><a name="parmvalue5852453141117"></a><a name="parmvalue5852453141117"></a> <code>SSG</code></span>: Each represents a neighbor selection strategy.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c++
#include <iostream>
#include "kbest.h"

int main() {
    // Parameter configuration
    int dim = 128;              // Feature dimension
    int R = 32;                 // Number of neighboring nodes
    int L = 200;                 // Size of the candidate node list during graph construction
    int A = 60;                 // Angle threshold for pruning during graph construction
    int graph_opt_iter = 2;     // Number of self-iterations for the graph index
    
    // Method 1: simple construction
    KBest index1(dim, R, L, A, "L2", "RNNDescent");
    std::cout << "Method 1: KBest index created successfully, dimension: " << index1.GetDim() << std::endl;
    
    // Method 2: full construction (recommended)
    KBest index2(dim, R, L, A, graph_opt_iter, "L2", "RNNDescent", "HNSW");
    std::cout << "Method 2: KBest index created successfully, dimension: " << index2.GetDim() << std::endl;
    
    return 0;
}
```

### Default Constructor

**API Definition <a name="section172317194488"></a>**

KBest\(\);

**API Function<a name="section1153124784912"></a>**

Initialize the build of graph search without arguments.

Instances created using this API support only the Load, Deserialize, and LoadGraph operations. When an API other than the preceding API is invoked, the value <code>-1</code> is returned.

**Parameter Description <a name="section157501312135019"></a>**

None

**Example**

```c++
#include <iostream>
#include "kbest.h"

int main() {
    // Default constructor, used for loading a previously saved index.
    KBest index;
    
    // Load a searcher from a file.
    int ret = index.Load("./saved_index.bin");
    if (ret == 0) {
        std::cout << "Index loaded successfully" << std::endl;
        std::cout << "Data dimension: " << index.GetDim() << std::endl;
        std::cout << "Number of data entries in the database: " << index.GetNTotal() << std::endl;
    }
    
    return 0;
}
```

### Add

**API Definition <a name="section172317194488"></a>**

int Add\(int nb, const float \*xb, int consecutive, int level\);

int Add\(int nb, const float \*xb, int consecutive, int reorder, int level\);

**API Function<a name="section1153124784912"></a>**

Builds a graph index.

**Parameter Description <a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="14.528547145285472%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="18.488151184881513%" id="mcps1.1.5.1.2"><p id="p18620101081116"><a name="p18620101081116"></a><a name="p18620101081116"></a> Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="21.14788521147885%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="45.83541645835416%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="14.528547145285472%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>nb</p>
</td>
<td class="cellrowborder" valign="top" width="18.488151184881513%" headers="mcps1.1.5.1.2 "><p id="p15620161014116"><a name="p15620161014116"></a><a name="p15620161014116"></a><span>int</span></p>
</td>
<td class="cellrowborder" valign="top" width="21.14788521147885%" headers="mcps1.1.5.1.3 "><p id="p182303331508"><a name="p182303331508"></a><a name="p182303331508"></a>Number of data entries in the vector database</p>
</td>
<td class="cellrowborder" valign="top" width="45.83541645835416%" headers="mcps1.1.5.1.4 "><p id="p1151275553412"><a name="p1151275553412"></a><a name="p1151275553412"></a>The value must be greater than or equal to 1. It is recommended that the value be less than 1 billion.</p>
</td>
</tr>
<tr id="row11230173385019"><td class="cellrowborder" valign="top" width="14.528547145285472%" headers="mcps1.1.5.1.1 "><p id="p22301333165015"><a name="p22301333165015"></a><a name="p22301333165015"></a>xb</p>
</td>
<td class="cellrowborder" valign="top" width="18.488151184881513%" headers="mcps1.1.5.1.2 "><p id="p362011011112"><a name="p362011011112"></a><a name="p362011011112"></a>const float *</p>
</td>
<td class="cellrowborder" valign="top" width="21.14788521147885%" headers="mcps1.1.5.1.3 "><p id="p10230433115013"><a name="p10230433115013"></a><a name="p10230433115013"></a>Vector database data</p>
</td>
<td class="cellrowborder" valign="top" width="45.83541645835416%" headers="mcps1.1.5.1.4 "><p id="p15512135514343"><a name="p15512135514343"></a><a name="p15512135514343"></a>It cannot be null. The length must be <code>nb</code> × <code>dim</code> (number of vectors × feature dimension).</p>
</td>
</tr>
<tr id="row92309336505"><td class="cellrowborder" valign="top" width="14.528547145285472%" headers="mcps1.1.5.1.1 "><p id="p162309336505"><a name="p162309336505"></a><a name="p162309336505"></a>consecutive</p>
</td>
<td class="cellrowborder" valign="top" width="18.488151184881513%" headers="mcps1.1.5.1.2 "><p id="p0620310181118"><a name="p0620310181118"></a><a name="p0620310181118"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="21.14788521147885%" headers="mcps1.1.5.1.3 "><p id="p92301933165017"><a name="p92301933165017"></a><a name="p92301933165017"></a>Block size</p>
</td>
<td class="cellrowborder" valign="top" width="45.83541645835416%" headers="mcps1.1.5.1.4 "><p id="p1151265503419"><a name="p1151265503419"></a><a name="p1151265503419"></a>[1, 31]</p>
</td>
</tr>
<tr id="row523013315504"><td class="cellrowborder" valign="top" width="14.528547145285472%" headers="mcps1.1.5.1.1 "><p id="p10230123316509"><a name="p10230123316509"></a><a name="p10230123316509"></a>level</p>
</td>
<td class="cellrowborder" valign="top" width="18.488151184881513%" headers="mcps1.1.5.1.2 "><p id="p126201910161110"><a name="p126201910161110"></a><a name="p126201910161110"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="21.14788521147885%" headers="mcps1.1.5.1.3 "><p id="p102301133105015"><a name="p102301133105015"></a><a name="p102301133105015"></a>Quantization level</p>
</td>
<td class="cellrowborder" valign="top" width="45.83541645835416%" headers="mcps1.1.5.1.4 "><p id="p19544111913232"><a name="p19544111913232"></a><a name="p19544111913232"></a>[0, 3]</p>
<a name="ul1454195619238"></a><a name="ul1454195619238"></a><ul id="ul1454195619238"><li><code>0</code>: FP32 quantization </li><li><code>1</code>: SQ8U quantization </li><li><code>2</code>: SQ4U quantization </li><li><code>3</code>: FP16 quantization</li></ul>
</td>
</tr>
<tr id="row1836863331311"><td class="cellrowborder" valign="top" width="14.528547145285472%" headers="mcps1.1.5.1.1 "><p id="p1830838111320"><a name="p1830838111320"></a><a name="p1830838111320"></a>reorder</p>
</td>
<td class="cellrowborder" valign="top" width="18.488151184881513%" headers="mcps1.1.5.1.2 "><p id="p73681333191314"><a name="p73681333191314"></a><a name="p73681333191314"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="21.14788521147885%" headers="mcps1.1.5.1.3 "><p id="p1083016385138"><a name="p1083016385138"></a><a name="p1083016385138"></a>Indicates whether to enable reordering of database vectors.</p>
</td>
<td class="cellrowborder" valign="top" width="45.83541645835416%" headers="mcps1.1.5.1.4 "><p id="p53681533101319"><a name="p53681533101319"></a><a name="p53681533101319"></a><code>0</code> or <code>1</code>.</p>
</td>
</tr>
</tbody>
</table>

**Return Value<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>
<table><thead align="left"><tr id="row1569152711463"><th class="cellrowborder" valign="top" width="34.599999999999994%" id="mcps1.1.3.1.1"><p id="p146911527174618"><a name="p146911527174618"></a><a name="p146911527174618"></a>Data Type </p>
</th>
<th class="cellrowborder" valign="top" width="65.4%" id="mcps1.1.3.1.2"><p id="p136911627194618"><a name="p136911627194618"></a><a name="p136911627194618"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row769192744612"><td class="cellrowborder" valign="top" width="34.599999999999994%" headers="mcps1.1.3.1.1 "><p id="p106910272463"><a name="p106910272463"></a><a name="p106910272463"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="65.4%" headers="mcps1.1.3.1.2 "><p id="p2611111352313"><a name="p2611111352313"></a><a name="p2611111352313"></a>If the parameter value is not within the value range, <code>-1</code> is returned. If this API is called after Load/Deserialize/LoadGraph, <code>-1</code> is returned. In other cases, <code>0</code> is returned.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c++
#include <iostream>
#include <vector>
#include <cstdlib>
#include "kbest.h"

int main() {
    int dim = 128;
    int nb = 10000; // Number of database vectors
    
    // Create an index.
    KBest index(dim, 32, 200, 60, 2, "L2", "RNNDescent", "HNSW");
    
    // Prepare database data.
    std::vector<float> xb(nb * dim);
    for (int i = 0; i < nb * dim; i++) {
        xb[i] = static_cast<float>(rand()) / RAND_MAX;
    }
    
    // Builds a graph index.
    int consecutive = 16; // Block size
    int reorder = 1; // Enable reordering of database vectors.
    int level = 0; // No quantization (FP32)
    
    int ret = index.Add(nb, xb.data(), consecutive, reorder, level);
    
    if (ret == 0) {
        std::cout << "Graph index created successfully" << std::endl;
        std::cout << "Number of data entries in the database: " << index.GetNTotal() << std::endl;
    } else {
        std::cout << "Failed to create the graph index. Error code: " << ret << std::endl;
    }
    
    return 0;
}
```

### BuildSearcher

**API Definition <a name="section172317194488"></a>**

int BuildSearcher\(\);

**API Function<a name="section1153124784912"></a>**

Builds a searcher using the <code>level</code> parameter from the Add API as the quantization parameter.

**Parameter Description <a name="section157501312135019"></a>**

None

**Return Value<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>
<table><thead align="left"><tr id="row1569152711463"><th class="cellrowborder" valign="top" width="34.599999999999994%" id="mcps1.1.3.1.1"><p id="p146911527174618"><a name="p146911527174618"></a><a name="p146911527174618"></a>Data Type </p>
</th>
<th class="cellrowborder" valign="top" width="65.4%" id="mcps1.1.3.1.2"><p id="p136911627194618"><a name="p136911627194618"></a><a name="p136911627194618"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row769192744612"><td class="cellrowborder" valign="top" width="34.599999999999994%" headers="mcps1.1.3.1.1 "><p id="p106910272463"><a name="p106910272463"></a><a name="p106910272463"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="65.4%" headers="mcps1.1.3.1.2 "><p id="p2611111352313"><a name="p2611111352313"></a><a name="p2611111352313"></a>If this API is called after Load/Deserialize/LoadGraph, <code>-1</code> is returned and the searcher remains unchanged.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c++
#include <iostream>
#include <vector>
#include "kbest.h"

int main() {
    int dim = 128;
    int nb = 10000;
    
    // Create an index.
    KBest index(dim, 32, 200, 60, 2, "L2", "RNNDescent", "HNSW");
    
    // Prepare and add database data.
    std::vector<float> xb(nb * dim);
    for (int i = 0; i < nb * dim; i++) {
        xb[i] = static_cast<float>(rand()) / RAND_MAX;
    }
    index.Add(nb, xb.data(), 16, 1, 0);
    
    // Build a searcher.
    int ret = index.BuildSearcher();
    
    if (ret == 0) {
        std::cout << "Searcher created successfully, ready for search" << std::endl;
    } else {
        std::cout << "Failed to build the searcher." << std::endl;
    }
    
    return 0;
}
```

### Search

**API Definition <a name="section172317194488"></a>**

int Search\(int nq, const float \*xq, int topk, float \*distances, int64\_t \*labels, int num\_thread\);

**API Function<a name="section1153124784912"></a>**

Searches for a graph.

**Parameter Description <a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="12.73%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="18.2%" id="mcps1.1.5.1.2"><p id="p1521112495121"><a name="p1521112495121"></a><a name="p1521112495121"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="29.79%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="39.28%" id="mcps1.1.5.1.4"><p id="p84604435401"><a name="p84604435401"></a><a name="p84604435401"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="12.73%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>nq</p>
</td>
<td class="cellrowborder" valign="top" width="18.2%" headers="mcps1.1.5.1.2 "><p id="p1521194918129"><a name="p1521194918129"></a><a name="p1521194918129"></a><span>int</span></p>
</td>
<td class="cellrowborder" valign="top" width="29.79%" headers="mcps1.1.5.1.3 "><p id="p182303331508"><a name="p182303331508"></a><a name="p182303331508"></a>Number of query vectors</p>
</td>
<td class="cellrowborder" valign="top" width="39.28%" headers="mcps1.1.5.1.4 "><p id="p1446074319406"><a name="p1446074319406"></a><a name="p1446074319406"></a>The value must be greater than or equal to 1. It is recommended that the value be less than 1 billion.</p>
</td>
</tr>
<tr id="row11230173385019"><td class="cellrowborder" valign="top" width="12.73%" headers="mcps1.1.5.1.1 "><p id="p22301333165015"><a name="p22301333165015"></a><a name="p22301333165015"></a>xq</p>
</td>
<td class="cellrowborder" valign="top" width="18.2%" headers="mcps1.1.5.1.2 "><p id="p321144921213"><a name="p321144921213"></a><a name="p321144921213"></a>const float *</p>
</td>
<td class="cellrowborder" valign="top" width="29.79%" headers="mcps1.1.5.1.3 "><p id="p10230433115013"><a name="p10230433115013"></a><a name="p10230433115013"></a>Query vector data</p>
</td>
<td class="cellrowborder" valign="top" width="39.28%" headers="mcps1.1.5.1.4 "><p id="p19460943204013"><a name="p19460943204013"></a><a name="p19460943204013"></a>It cannot be null, and the expected length is <code>nq</code> × <code>dim</code> (number of vectors × feature dimension).</p>
</td>
</tr>
<tr id="row92309336505"><td class="cellrowborder" valign="top" width="12.73%" headers="mcps1.1.5.1.1 "><p id="p162309336505"><a name="p162309336505"></a><a name="p162309336505"></a>topk</p>
</td>
<td class="cellrowborder" valign="top" width="18.2%" headers="mcps1.1.5.1.2 "><p id="p122111249101212"><a name="p122111249101212"></a><a name="p122111249101212"></a><span>int</span></p>
</td>
<td class="cellrowborder" valign="top" width="29.79%" headers="mcps1.1.5.1.3 "><p id="p92301933165017"><a name="p92301933165017"></a><a name="p92301933165017"></a>Number of nearest neighbors</p>
</td>
<td class="cellrowborder" valign="top" width="39.28%" headers="mcps1.1.5.1.4 "><p id="p1178758184115"><a name="p1178758184115"></a><a name="p1178758184115"></a>[1, nb], where <span class="parmname" id="parmname15768691767"><a name="parmname15768691767"></a><a name="parmname15768691767"></a><code>nb</code></span> indicates the number of data entries in the vector database.</p>
</td>
</tr>
<tr id="row523013315504"><td class="cellrowborder" valign="top" width="12.73%" headers="mcps1.1.5.1.1 "><p id="p10230123316509"><a name="p10230123316509"></a><a name="p10230123316509"></a>distances</p>
</td>
<td class="cellrowborder" valign="top" width="18.2%" headers="mcps1.1.5.1.2 "><p id="p5211114910120"><a name="p5211114910120"></a><a name="p5211114910120"></a>float *</p>
</td>
<td class="cellrowborder" valign="top" width="29.79%" headers="mcps1.1.5.1.3 "><p id="p102301133105015"><a name="p102301133105015"></a><a name="p102301133105015"></a>Distance array</p>
</td>
<td class="cellrowborder" valign="top" width="39.28%" headers="mcps1.1.5.1.4 "><p id="p124318194133"><a name="p124318194133"></a><a name="p124318194133"></a>It cannot be null, and <span>the expected length is <code>nq</code> × <code>topk</code></span>.</p>
</td>
</tr>
<tr id="row1523083315012"><td class="cellrowborder" valign="top" width="12.73%" headers="mcps1.1.5.1.1 "><p id="p10230433105020"><a name="p10230433105020"></a><a name="p10230433105020"></a>labels</p>
</td>
<td class="cellrowborder" valign="top" width="18.2%" headers="mcps1.1.5.1.2 "><p id="p1921118495123"><a name="p1921118495123"></a><a name="p1921118495123"></a>int64_t *</p>
</td>
<td class="cellrowborder" valign="top" width="29.79%" headers="mcps1.1.5.1.3 "><p id="p33565281418"><a name="p33565281418"></a><a name="p33565281418"></a>ID array of search results</p>
</td>
<td class="cellrowborder" valign="top" width="39.28%" headers="mcps1.1.5.1.4 "><p id="p124602043204018"><a name="p124602043204018"></a><a name="p124602043204018"></a>It cannot be null, and <span>the expected length is <code>nq</code> × <code>topk</code></span>.</p>
</td>
</tr>
<tr id="row177151948121320"><td class="cellrowborder" valign="top" width="12.73%" headers="mcps1.1.5.1.1 "><p id="p3715448191319"><a name="p3715448191319"></a><a name="p3715448191319"></a>num_thread</p>
</td>
<td class="cellrowborder" valign="top" width="18.2%" headers="mcps1.1.5.1.2 "><p id="p4211249101218"><a name="p4211249101218"></a><a name="p4211249101218"></a><span>int</span></p>
</td>
<td class="cellrowborder" valign="top" width="29.79%" headers="mcps1.1.5.1.3 "><p id="p137151148161319"><a name="p137151148161319"></a><a name="p137151148161319"></a>Number of threads used for search</p>
</td>
<td class="cellrowborder" valign="top" width="39.28%" headers="mcps1.1.5.1.4 "><p id="p95801533174311"><a name="p95801533174311"></a><a name="p95801533174311"></a>[1, std::thread::hardware_concurrency()], where <code>std::thread::hardware_concurrency()</code> indicates <span>the number of concurrent threads supported by the current system</span>.</p>
</td>
</tr>
</tbody>
</table>

**Return Value<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>
<table><thead align="left"><tr id="row1569152711463"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p146911527174618"><a name="p146911527174618"></a><a name="p146911527174618"></a>Data Type </p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p136911627194618"><a name="p136911627194618"></a><a name="p136911627194618"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row769192744612"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p106910272463"><a name="p106910272463"></a><a name="p106910272463"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p2611111352313"><a name="p2611111352313"></a><a name="p2611111352313"></a>If the parameter value is not within the value range, <code>-1</code> is returned. If this API is called before BuildSearcher or Load/Deserialize/LoadGraph, <code>-1</code> is returned. In other cases, <code>0</code> is returned.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c++
#include <iostream>
#include <vector>
#include "kbest.h"

int main() {
    int dim = 128;
    int nb = 10000;
    int nq = 10;     // Number of query vectors
    int topk = 5;     // Return top five nearest neighbors.
    
    // Create and build an index.
    KBest index(dim, 32, 200, 60, 2, "L2", "RNNDescent", "HNSW");
    
    std::vector<float> xb(nb * dim);
    for (int i = 0; i < nb * dim; i++) {
        xb[i] = static_cast<float>(rand()) / RAND_MAX;
    }
    index.Add(nb, xb.data(), 16, 1, 0);
    index.BuildSearcher();
    
    // Prepare the query vectors.
    std::vector<float> xq(nq * dim);
    for (int i = 0; i < nq * dim; i++) {
        xq[i] = static_cast<float>(rand()) / RAND_MAX;
    }
    
    // Prepare the result array.
    std::vector<float> distances(nq * topk);
    std::vector<int64_t> labels(nq * topk);
    
    // Perform search.
    int num_thread = 4;
    int ret = index.Search(nq, xq.data(), topk, distances.data(), labels.data(), num_thread);
    
    if (ret == 0) {
        std::cout << "Search succeeded: " << std::endl;
        // Output the result of the first query vector.
        std::cout << "Nearest neighbor of query vector 0: " << std::endl;
        for (int i = 0; i < topk; i++) {
            std::cout << " ID: " << labels[i] << ", Distance: " << distances[i] << std::endl;
        }
    }
    
    return 0;
}
```

### SetEf

**API Definition <a name="section172317194488"></a>**

int SetEf\(int ef\);

**API Function<a name="section1153124784912"></a>**

Sets the size of the candidate node list during search.

**Parameter Description <a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="14.280000000000001%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="15.64%" id="mcps1.1.5.1.2"><p id="p82341657161314"><a name="p82341657161314"></a><a name="p82341657161314"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="34.54%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="35.54%" id="mcps1.1.5.1.4"><p id="p1440932116441"><a name="p1440932116441"></a><a name="p1440932116441"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="14.280000000000001%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>ef</p>
</td>
<td class="cellrowborder" valign="top" width="15.64%" headers="mcps1.1.5.1.2 "><p id="p9234135711132"><a name="p9234135711132"></a><a name="p9234135711132"></a><span>int</span></p>
</td>
<td class="cellrowborder" valign="top" width="34.54%" headers="mcps1.1.5.1.3 "><p id="p39711451181514"><a name="p39711451181514"></a><a name="p39711451181514"></a>Size of the candidate node list during search</p>
</td>
<td class="cellrowborder" valign="top" width="35.54%" headers="mcps1.1.5.1.4 "><p id="p1178758184115"><a name="p1178758184115"></a><a name="p1178758184115"></a>[1, nb], where <span class="parmname" id="parmname15768691767"><a name="parmname15768691767"></a><a name="parmname15768691767"></a><code>nb</code></span> indicates the number of data entries in the vector database.</p>
</td>
</tr>
</tbody>
</table>

**Return Value<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>
<table><thead align="left"><tr id="row1569152711463"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p146911527174618"><a name="p146911527174618"></a><a name="p146911527174618"></a>Data Type </p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p136911627194618"><a name="p136911627194618"></a><a name="p136911627194618"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row769192744612"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p106910272463"><a name="p106910272463"></a><a name="p106910272463"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p2611111352313"><a name="p2611111352313"></a><a name="p2611111352313"></a>If the parameter value is not within the value range, <code>-1</code> is returned. If this API is called before BuildSearcher or Load/Deserialize/LoadGraph, <code>-1</code> is returned. In other cases, <code>0</code> is returned.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c++
#include <iostream>
#include <vector>
#include "kbest.h"

int main() {
    int dim = 128;
    int nb = 10000;
    
    // Create and build an index.
    KBest index(dim, 32, 200, 60, 2, "L2", "RNNDescent", "HNSW");
    
    std::vector<float> xb(nb * dim);
    for (int i = 0; i < nb * dim; i++) {
        xb[i] = static_cast<float>(rand()) / RAND_MAX;
    }
    index.Add(nb, xb.data(), 16, 1, 0);
    index.BuildSearcher();
    
    // Set a small ef value (faster search, but lower accuracy).
    index.SetEf(50);
    std::cout << "Searching with ef=50..." << std::endl;
    
    // Set a large ef value (slower search, but higher accuracy).
    int ret = index.SetEf(200);
    if (ret == 0) {
        std::cout << "Successfully set ef=200" << std::endl;
    }
    
    return 0;
}
```

### Save

**API Definition <a name="section172317194488"></a>**

int Save\(const char \*path\) const;

**API Function<a name="section1153124784912"></a>**

Saves a searcher to a specified path in a single process.

**Parameter Description <a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="16.06%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="15.18%" id="mcps1.1.5.1.2"><p id="p17714142111149"><a name="p17714142111149"></a><a name="p17714142111149"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="34.239999999999995%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="34.52%" id="mcps1.1.5.1.4"><p id="p1440932116441"><a name="p1440932116441"></a><a name="p1440932116441"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="16.06%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>path</p>
</td>
<td class="cellrowborder" valign="top" width="15.18%" headers="mcps1.1.5.1.2 "><p id="p171412119148"><a name="p171412119148"></a><a name="p171412119148"></a>const char *</p>
</td>
<td class="cellrowborder" valign="top" width="34.239999999999995%" headers="mcps1.1.5.1.3 "><p id="p39711451181514"><a name="p39711451181514"></a><a name="p39711451181514"></a>Path for storing the searcher</p>
</td>
<td class="cellrowborder" valign="top" width="34.52%" headers="mcps1.1.5.1.4 "><p id="p20167131514510"><a name="p20167131514510"></a><a name="p20167131514510"></a>The value contains less than 199 characters.</p>
</td>
</tr>
</tbody>
</table>

**Return Value<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>
<table><thead align="left"><tr id="row1569152711463"><th class="cellrowborder" valign="top" width="38.95%" id="mcps1.1.3.1.1"><p id="p146911527174618"><a name="p146911527174618"></a><a name="p146911527174618"></a>Data Type </p>
</th>
<th class="cellrowborder" valign="top" width="61.050000000000004%" id="mcps1.1.3.1.2"><p id="p136911627194618"><a name="p136911627194618"></a><a name="p136911627194618"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row769192744612"><td class="cellrowborder" valign="top" width="38.95%" headers="mcps1.1.3.1.1 "><p id="p106910272463"><a name="p106910272463"></a><a name="p106910272463"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="61.050000000000004%" headers="mcps1.1.3.1.2 "><p id="p2611111352313"><a name="p2611111352313"></a><a name="p2611111352313"></a>If the parameter value is not within the value range or an I/O problem such as incorrect save path occurs, <code>-1</code> is returned. <span>If this API is called before BuildSearcher</span>, <code>-1</code> is returned. In other cases, <code>0</code> is returned.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c++
#include <iostream>
#include <vector>
#include "kbest.h"

int main() {
    int dim = 128;
    int nb = 10000;
    
    // Create and build an index.
    KBest index(dim, 32, 200, 60, 2, "L2", "RNNDescent", "HNSW");
    
    std::vector<float> xb(nb * dim);
    for (int i = 0; i < nb * dim; i++) {
        xb[i] = static_cast<float>(rand()) / RAND_MAX;
    }
    index.Add(nb, xb.data(), 16, 1, 0);
    index.BuildSearcher();
    
    // Save the searcher.
    int ret = index.Save("./kbest_index.bin");
    
    if (ret == 0) {
        std::cout << "Searcher successfully saved to ./kbest_index.bin" << std::endl;
    } else {
        std::cout << " Failed to save the searcher" << std::endl;
    }
    
    return 0;
}
```

### Load

**API Definition <a name="section172317194488"></a>**

int Load\(const char \*path\);

**API Function<a name="section1153124784912"></a>**

Loads a searcher from a specified path.

**Parameter Description <a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="16.13161316131613%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="15.441544154415443%" id="mcps1.1.5.1.2"><p id="p2138751201416"><a name="p2138751201416"></a><a name="p2138751201416"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="35.34353435343534%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="33.083308330833084%" id="mcps1.1.5.1.4"><p id="p1440932116441"><a name="p1440932116441"></a><a name="p1440932116441"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="16.13161316131613%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>path</p>
</td>
<td class="cellrowborder" valign="top" width="15.441544154415443%" headers="mcps1.1.5.1.2 "><p id="p11381051141410"><a name="p11381051141410"></a><a name="p11381051141410"></a>const char *</p>
</td>
<td class="cellrowborder" valign="top" width="35.34353435343534%" headers="mcps1.1.5.1.3 "><p id="p39711451181514"><a name="p39711451181514"></a><a name="p39711451181514"></a>Path from which the searcher is loaded</p>
</td>
<td class="cellrowborder" valign="top" width="33.083308330833084%" headers="mcps1.1.5.1.4 "><p id="p20167131514510"><a name="p20167131514510"></a><a name="p20167131514510"></a>The value contains less than 199 characters.</p>
</td>
</tr>
</tbody>
</table>

**Return Value<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>
<table><thead align="left"><tr id="row1569152711463"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p146911527174618"><a name="p146911527174618"></a><a name="p146911527174618"></a>Data Type </p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p136911627194618"><a name="p136911627194618"></a><a name="p136911627194618"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row769192744612"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p106910272463"><a name="p106910272463"></a><a name="p106910272463"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p2611111352313"><a name="p2611111352313"></a><a name="p2611111352313"></a>If the parameter value is not within the value range or an I/O problem such as incorrect read path occurs, <code>-1</code> is returned. In other cases, <code>0</code> is returned.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c++
#include <iostream>
#include <vector>
#include "kbest.h"

int main() {
    // Create an index instance using the default constructor.
    KBest index;
    
    // Load a searcher from a file.
    int ret = index.Load("./kbest_index.bin");
    
    if (ret == 0) {
        std::cout << "Searcher loaded successfully" << std::endl;
        std::cout << "Data dimension: " << index.GetDim() << std::endl;
        std::cout << "Number of data entries in the database: " << index.GetNTotal() << std::endl;
        
        // Once loaded, the searcher is ready for search.
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
        std::cout << "Failed to load the searcher: " << std::endl;
    }
    
    return 0;
}
```

### SaveGraph

**API Definition <a name="section172317194488"></a>**

int SaveGraph\(const char \*path\) const;

**API Function<a name="section1153124784912"></a>**

Saves a graph index to a specified path in a single process.

**Parameter Description <a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="13.63%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="17.48%" id="mcps1.1.5.1.2"><p id="p13945191217156"><a name="p13945191217156"></a><a name="p13945191217156"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="34.510000000000005%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="34.38%" id="mcps1.1.5.1.4"><p id="p1440932116441"><a name="p1440932116441"></a><a name="p1440932116441"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="13.63%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>path</p>
</td>
<td class="cellrowborder" valign="top" width="17.48%" headers="mcps1.1.5.1.2 "><p id="p8945111231510"><a name="p8945111231510"></a><a name="p8945111231510"></a>const char *</p>
</td>
<td class="cellrowborder" valign="top" width="34.510000000000005%" headers="mcps1.1.5.1.3 "><p id="p39711451181514"><a name="p39711451181514"></a><a name="p39711451181514"></a>Path for storing the graph index</p>
</td>
<td class="cellrowborder" valign="top" width="34.38%" headers="mcps1.1.5.1.4 "><p id="p20167131514510"><a name="p20167131514510"></a><a name="p20167131514510"></a>The value contains less than 199 characters.</p>
</td>
</tr>
</tbody>
</table>

**Return Value<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>
<table><thead align="left"><tr id="row1569152711463"><th class="cellrowborder" valign="top" width="38.9%" id="mcps1.1.3.1.1"><p id="p146911527174618"><a name="p146911527174618"></a><a name="p146911527174618"></a>Data Type </p>
</th>
<th class="cellrowborder" valign="top" width="61.1%" id="mcps1.1.3.1.2"><p id="p136911627194618"><a name="p136911627194618"></a><a name="p136911627194618"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row769192744612"><td class="cellrowborder" valign="top" width="38.9%" headers="mcps1.1.3.1.1 "><p id="p106910272463"><a name="p106910272463"></a><a name="p106910272463"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="61.1%" headers="mcps1.1.3.1.2 "><p id="p2611111352313"><a name="p2611111352313"></a><a name="p2611111352313"></a>If the parameter value is not within the value range or an I/O problem such as incorrect save path occurs, <code>-1</code> is returned. If this API is called before the Add API, <code>-1</code> is returned. If this API is called after BuildSearcher or Load/Deserialize/LoadGraph, <code>-1</code> is returned. In other cases, <code>0</code> is returned.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c++
#include <iostream>
#include <vector>
#include "kbest.h"

int main() {
    int dim = 128;
    int nb = 10000;
    
    // Create an index and add data.
    KBest index(dim, 32, 200, 60, 2, "L2", "RNNDescent", "HNSW");
    
    std::vector<float> xb(nb * dim);
    for (int i = 0; i < nb * dim; i++) {
        xb[i] = static_cast<float>(rand()) / RAND_MAX;
    }
    index.Add(nb, xb.data(), 16, 1, 0);
    
    // Save the graph index before calling BuildSearcher.
    int ret = index.SaveGraph("./kbest_graph.bin");
    
    if (ret == 0) {
        std::cout << " Graph index successfully saved to ./kbest_graph.bin" << std::endl;
    } else {
        std::cout << "Failed to save the graph index." << std::endl;
    }
    
    return 0;
}
```

### LoadGraph

**API Definition <a name="section172317194488"></a>**

int LoadGraph\(const char \*path, int level\);

**API Function<a name="section1153124784912"></a>**

Loads a searcher from a specified path.

**Parameter Description <a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="10.73%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="20.990000000000002%" id="mcps1.1.5.1.2"><p id="p16585143220155"><a name="p16585143220155"></a><a name="p16585143220155"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="25.66%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="42.620000000000005%" id="mcps1.1.5.1.4"><p id="p1440932116441"><a name="p1440932116441"></a><a name="p1440932116441"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="10.73%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>path</p>
</td>
<td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.1.5.1.2 "><p id="p17585193281515"><a name="p17585193281515"></a><a name="p17585193281515"></a>const char *</p>
</td>
<td class="cellrowborder" valign="top" width="25.66%" headers="mcps1.1.5.1.3 "><p id="p39711451181514"><a name="p39711451181514"></a><a name="p39711451181514"></a>Path from which the searcher is loaded</p>
</td>
<td class="cellrowborder" valign="top" width="42.620000000000005%" headers="mcps1.1.5.1.4 "><p id="p20167131514510"><a name="p20167131514510"></a><a name="p20167131514510"></a>The value contains less than 199 characters.</p>
</td>
</tr>
<tr id="row641410102301"><td class="cellrowborder" valign="top" width="10.73%" headers="mcps1.1.5.1.1 "><p id="p19414810153017"><a name="p19414810153017"></a><a name="p19414810153017"></a>level</p>
</td>
<td class="cellrowborder" valign="top" width="20.990000000000002%" headers="mcps1.1.5.1.2 "><p id="p195851932131517"><a name="p195851932131517"></a><a name="p195851932131517"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="25.66%" headers="mcps1.1.5.1.3 "><p id="p5414151014309"><a name="p5414151014309"></a><a name="p5414151014309"></a>Quantization level</p>
</td>
<td class="cellrowborder" valign="top" width="42.620000000000005%" headers="mcps1.1.5.1.4 "><p id="p14665102215"><a name="p14665102215"></a><a name="p14665102215"></a>[-1,3]</p>
<a name="ul1454195619238"></a><a name="ul1454195619238"></a><ul id="ul1454195619238"><li><code>-1</code>: default value, indicating the quantization level saved during the SaveGraph operation. </li><li><code>0</code>: FP32 quantization </li><li><code>1</code>: SQ8U quantization </li><li><code>2</code>: SQ4U quantization </li><li><code>3</code>: FP16 quantization</li></ul>
</td>
</tr>
</tbody>
</table>

**Return Value<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>
<table><thead align="left"><tr id="row1569152711463"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p146911527174618"><a name="p146911527174618"></a><a name="p146911527174618"></a>Data Type </p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p136911627194618"><a name="p136911627194618"></a><a name="p136911627194618"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row769192744612"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p106910272463"><a name="p106910272463"></a><a name="p106910272463"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p2611111352313"><a name="p2611111352313"></a><a name="p2611111352313"></a>If the parameter value is not within the value range or an I/O problem such as incorrect read path occurs, <code>-1</code> is returned. In other cases, <code>0</code> is returned.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c++
#include <iostream>
#include <vector>
#include "kbest.h"

int main() {
    // Create an index instance using the default constructor.
    KBest index;
    
    // Load the graph index from a file and use the quantization level saved with it.
    int ret = index.LoadGraph("./kbest_graph.bin", -1);
    
    if (ret == 0) {
        std::cout << "Graph index loaded successfully" << std::endl;
        std::cout << "Data dimension: " << index.GetDim() << std::endl;
        std::cout << "Number of data entries in the database: " << index.GetNTotal() << std::endl;
        
        // Once loaded, the searcher is ready for search.
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

**API Definition <a name="section172317194488"></a>**

int Serialize\(uint8\_t \*&dataPtr, size\_t &dataLength\) const;

**API Function<a name="section1153124784912"></a>**

Stores the searcher content into the uint8 array with a length of <code>dataLength</code> bytes and a start address of <code>dataPtr</code>.

**Parameter Description <a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="14.23%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="16.619999999999997%" id="mcps1.1.5.1.2"><p id="p1475418561158"><a name="p1475418561158"></a><a name="p1475418561158"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="36.84%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="32.31%" id="mcps1.1.5.1.4"><p id="p1440932116441"><a name="p1440932116441"></a><a name="p1440932116441"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="14.23%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>dataPtr</p>
</td>
<td class="cellrowborder" valign="top" width="16.619999999999997%" headers="mcps1.1.5.1.2 "><p id="p57541756181511"><a name="p57541756181511"></a><a name="p57541756181511"></a>uint8_t *&amp;</p>
</td>
<td class="cellrowborder" valign="top" width="36.84%" headers="mcps1.1.5.1.3 "><p id="p39711451181514"><a name="p39711451181514"></a><a name="p39711451181514"></a>Start address of the array that stores the searcher content</p>
</td>
<td class="cellrowborder" valign="top" width="32.31%" headers="mcps1.1.5.1.4 "><p id="p20167131514510"><a name="p20167131514510"></a><a name="p20167131514510"></a>The value can only be a null pointer.</p>
</td>
</tr>
<tr id="row641410102301"><td class="cellrowborder" valign="top" width="14.23%" headers="mcps1.1.5.1.1 "><p id="p19414810153017"><a name="p19414810153017"></a><a name="p19414810153017"></a>dataLength</p>
</td>
<td class="cellrowborder" valign="top" width="16.619999999999997%" headers="mcps1.1.5.1.2 "><p id="p57541256161516"><a name="p57541256161516"></a><a name="p57541256161516"></a>size_t &amp;</p>
</td>
<td class="cellrowborder" valign="top" width="36.84%" headers="mcps1.1.5.1.3 "><p id="p5414151014309"><a name="p5414151014309"></a><a name="p5414151014309"></a>Length of the array that stores the searcher content</p>
</td>
<td class="cellrowborder" valign="top" width="32.31%" headers="mcps1.1.5.1.4 "><p id="p44144105305"><a name="p44144105305"></a><a name="p44144105305"></a>The value must be <code>0</code>.</p>
</td>
</tr>
</tbody>
</table>

**Return Value<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>
<table><thead align="left"><tr id="row1569152711463"><th class="cellrowborder" valign="top" width="36.96%" id="mcps1.1.3.1.1"><p id="p146911527174618"><a name="p146911527174618"></a><a name="p146911527174618"></a>Data Type </p>
</th>
<th class="cellrowborder" valign="top" width="63.04%" id="mcps1.1.3.1.2"><p id="p136911627194618"><a name="p136911627194618"></a><a name="p136911627194618"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row769192744612"><td class="cellrowborder" valign="top" width="36.96%" headers="mcps1.1.3.1.1 "><p id="p106910272463"><a name="p106910272463"></a><a name="p106910272463"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="63.04%" headers="mcps1.1.3.1.2 "><p id="p2611111352313"><a name="p2611111352313"></a><a name="p2611111352313"></a>If the parameter value is not within the value range, <code>-1</code> is returned. If this API is called after BuildSearcher or Load/Deserialize/LoadGraph, <code>-1</code> is returned. In other cases, <code>0</code> is returned.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c++
#include <iostream>
#include <vector>
#include "kbest.h"

int main() {
    int dim = 128;
    int nb = 10000;
    
    // Create an index and add data.
    KBest index(dim, 32, 200, 60, 2, "L2", "RNNDescent", "HNSW");
    
    std::vector<float> xb(nb * dim);
    for (int i = 0; i < nb * dim; i++) {
        xb[i] = static_cast<float>(rand()) / RAND_MAX;
    }
    index.Add(nb, xb.data(), 16, 1, 0);
    
    // Serialize the searcher content into an array.
    uint8_t* dataPtr = nullptr;
    size_t dataLength = 0;
    
    int ret = index.Serialize(dataPtr, dataLength);
    
    if (ret == 0) {
        std::cout << "Serialization succeeded. Data length: " << dataLength << " bytes" << std::endl;
        
        //... You can store the serialized data (pointed to by dataPtr) in the database...
        
        // Release the memory after use.
        delete[] dataPtr;
    }
    
    return 0;
}
```

### Deserialize

**API Definition <a name="section172317194488"></a>**

int Deserialize\(const uint8\_t \*dataPtr, const size\_t &dataLength\);

**API Function<a name="section1153124784912"></a>**

Restores a search index instance from a serialized data array pointed to by <code>dataPtr</code>, with length <code>dataLength</code>.

**Parameter Description <a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="14.54854514548545%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="18.44815518448155%" id="mcps1.1.5.1.2"><p id="p8993101991611"><a name="p8993101991611"></a><a name="p8993101991611"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="32.436756324367565%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="34.56654334566544%" id="mcps1.1.5.1.4"><p id="p1440932116441"><a name="p1440932116441"></a><a name="p1440932116441"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="14.54854514548545%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>dataPtr</p>
</td>
<td class="cellrowborder" valign="top" width="18.44815518448155%" headers="mcps1.1.5.1.2 "><p id="p199331913161"><a name="p199331913161"></a><a name="p199331913161"></a>const uint8_t *</p>
</td>
<td class="cellrowborder" valign="top" width="32.436756324367565%" headers="mcps1.1.5.1.3 "><p id="p39711451181514"><a name="p39711451181514"></a><a name="p39711451181514"></a>Start address of the array that stores the searcher content</p>
</td>
<td class="cellrowborder" valign="top" width="34.56654334566544%" headers="mcps1.1.5.1.4 "><p id="p20167131514510"><a name="p20167131514510"></a><a name="p20167131514510"></a>It cannot be null.</p>
</td>
</tr>
<tr id="row641410102301"><td class="cellrowborder" valign="top" width="14.54854514548545%" headers="mcps1.1.5.1.1 "><p id="p19414810153017"><a name="p19414810153017"></a><a name="p19414810153017"></a>dataLength</p>
</td>
<td class="cellrowborder" valign="top" width="18.44815518448155%" headers="mcps1.1.5.1.2 "><p id="p2993101915163"><a name="p2993101915163"></a><a name="p2993101915163"></a>const size_t &amp;</p>
</td>
<td class="cellrowborder" valign="top" width="32.436756324367565%" headers="mcps1.1.5.1.3 "><p id="p5414151014309"><a name="p5414151014309"></a><a name="p5414151014309"></a>Length of the array that stores the searcher content</p>
</td>
<td class="cellrowborder" valign="top" width="34.56654334566544%" headers="mcps1.1.5.1.4 "><p id="p44144105305"><a name="p44144105305"></a><a name="p44144105305"></a>Array length saved when the Serialize API is called.</p>
</td>
</tr>
</tbody>
</table>

**Return Value<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>
<table><thead align="left"><tr id="row1569152711463"><th class="cellrowborder" valign="top" width="36.96%" id="mcps1.1.3.1.1"><p id="p146911527174618"><a name="p146911527174618"></a><a name="p146911527174618"></a>Data Type </p>
</th>
<th class="cellrowborder" valign="top" width="63.04%" id="mcps1.1.3.1.2"><p id="p136911627194618"><a name="p136911627194618"></a><a name="p136911627194618"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row769192744612"><td class="cellrowborder" valign="top" width="36.96%" headers="mcps1.1.3.1.1 "><p id="p106910272463"><a name="p106910272463"></a><a name="p106910272463"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="63.04%" headers="mcps1.1.3.1.2 "><p id="p249262275018"><a name="p249262275018"></a><a name="p249262275018"></a>If the parameter value is not within the range, <code>-1</code> is returned. Otherwise, <code>0</code> is returned.</p>
<p id="p2611111352313"><a name="p2611111352313"></a><a name="p2611111352313"></a>The Serialize API applies for array memory internally. After calling this API, use <code>delete []</code> to release the resources.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c++
#include <iostream>
#include <vector>
#include "kbest.h"

int main() {
    int dim = 128;
    int nb = 10000;
    
    // Create an index and serialize it.
    KBest index1(dim, 32, 200, 60, 2, "L2", "RNNDescent", "HNSW");
    
    std::vector<float> xb(nb * dim);
    for (int i = 0; i < nb * dim; i++) {
        xb[i] = static_cast<float>(rand()) / RAND_MAX;
    }
    index1.Add(nb, xb.data(), 16, 1, 0);
    
    uint8_t* dataPtr = nullptr;
    size_t dataLength = 0;
    index1.Serialize(dataPtr, dataLength);
    
    // Restore the index from the serialized data.
    KBest index2;
    int ret = index2.Deserialize(dataPtr, dataLength);
    
    if (ret == 0) {
        std::cout << "Deserialization succeeded: " << std::endl;
        std::cout << "Dimension of the index after deserialization: " << index2.GetDim() << std::endl;
        std::cout << "Number of database entries after deserialization: " << index2.GetNTotal() << std::endl;
        
        // Once deserialized, the index is ready for search.
    }
    
    // Release the memory allocated during serialization.
    delete[] dataPtr;
    
    return 0;
}
```

### GetNTotal

**API Definition <a name="section172317194488"></a>**

int GetNTotal\(\) const;

**API Function<a name="section1153124784912"></a>**

Returns the total number of data entries in the database within the graph index.

**Parameter Description <a name="section1521117111210"></a>**

None

**Return Value<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>
<table><thead align="left"><tr id="row1569152711463"><th class="cellrowborder" valign="top" width="36.96%" id="mcps1.1.3.1.1"><p id="p146911527174618"><a name="p146911527174618"></a><a name="p146911527174618"></a>Data Type </p>
</th>
<th class="cellrowborder" valign="top" width="63.04%" id="mcps1.1.3.1.2"><p id="p136911627194618"><a name="p136911627194618"></a><a name="p136911627194618"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row769192744612"><td class="cellrowborder" valign="top" width="36.96%" headers="mcps1.1.3.1.1 "><p id="p106910272463"><a name="p106910272463"></a><a name="p106910272463"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="63.04%" headers="mcps1.1.3.1.2 "><p id="p2611111352313"><a name="p2611111352313"></a><a name="p2611111352313"></a>If no database is added,<code>0</code> is returned by default.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c++
#include <iostream>
#include <vector>
#include "kbest.h"

int main() {
    int dim = 128;
    int nb = 10000;
    
    KBest index(dim, 32, 200, 60, 2, "L2", "RNNDescent", "HNSW");
    
    // Before adding data
    std::cout << "Number of data entries in the database before adding data: " << index.GetNTotal() << std::endl;
    
    // Add data.
    std::vector<float> xb(nb * dim);
    for (int i = 0; i < nb * dim; i++) {
        xb[i] = static_cast<float>(rand()) / RAND_MAX;
    }
    index.Add(nb, xb.data(), 16, 1, 0);
    
    // After adding data
    std::cout << "Number of data entries in the database after adding data: " << index.GetNTotal() << std::endl;
    
    return 0;
}
```

### GetDim

**API Definition <a name="section172317194488"></a>**

int GetDim\(\) const;

**API Function<a name="section1153124784912"></a>**

Returns the data dimension in the current graph index.

**Parameter Description <a name="section1521117111210"></a>**

None

**Return Value<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>
<table><thead align="left"><tr id="row1569152711463"><th class="cellrowborder" valign="top" width="36.96%" id="mcps1.1.3.1.1"><p id="p146911527174618"><a name="p146911527174618"></a><a name="p146911527174618"></a>Data Type </p>
</th>
<th class="cellrowborder" valign="top" width="63.04%" id="mcps1.1.3.1.2"><p id="p136911627194618"><a name="p136911627194618"></a><a name="p136911627194618"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row769192744612"><td class="cellrowborder" valign="top" width="36.96%" headers="mcps1.1.3.1.1 "><p id="p106910272463"><a name="p106910272463"></a><a name="p106910272463"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="63.04%" headers="mcps1.1.3.1.2 "><p id="p2611111352313"><a name="p2611111352313"></a><a name="p2611111352313"></a>If an index is created using a parameterized constructor, the value is the same as that of <span class="parmname" id="parmname8379143211611"><a name="parmname8379143211611"></a><a name="parmname8379143211611"></a><code>dim</code></span>. If an index is created using a default constructor or if an index created with a parameterized constructor is later re-initialized by calling Load/Deserialize/LoadGraph, the return value is the dimension of data read from the searcher or the graph index.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c++
#include <iostream>
#include "kbest.h"

int main() {
    int dim = 128;
    
    // Create with parameterized constructor
    KBest index1(dim, 32, 200, 60, 2, "L2", "RNNDescent", "HNSW");
    std::cout << "Dimension after parameterized construction: " << index1.GetDim() << std::endl;
    
    // Create with default constructor, then load from file
    KBest index2;
    index2.Load("./kbest_index.bin");
    std::cout << "Dimension after loading from file: " << index2.GetDim() << std::endl;
    
    return 0;
}
```

### SetEarlyStoppingParams

**API Definition <a name="section172317194488"></a>**

int SetEarlyStoppingParams\(int32\_t adding\_pref, int32\_t patience\)

**API Function<a name="section1153124784912"></a>**

Sets the parameters for early stopping optimization.

**Parameter Description <a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.2984701529847%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="17.698230176982303%" id="mcps1.1.5.1.2"><p id="p8993101991611"><a name="p8993101991611"></a><a name="p8993101991611"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="32.436756324367565%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="34.56654334566544%" id="mcps1.1.5.1.4"><p id="p1440932116441"><a name="p1440932116441"></a><a name="p1440932116441"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.2984701529847%" headers="mcps1.1.5.1.1 "><p id="p6904143931516"><a name="p6904143931516"></a><a name="p6904143931516"></a>adding_pref</p>
</td>
<td class="cellrowborder" valign="top" width="17.698230176982303%" headers="mcps1.1.5.1.2 "><p id="p199331913161"><a name="p199331913161"></a><a name="p199331913161"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="32.436756324367565%" headers="mcps1.1.5.1.3 "><p id="p29041739131510"><a name="p29041739131510"></a><a name="p29041739131510"></a>Threshold for inserting the hyperparameter candidate set</p>
</td>
<td class="cellrowborder" valign="top" width="34.56654334566544%" headers="mcps1.1.5.1.4 "><p id="p20167131514510"><a name="p20167131514510"></a><a name="p20167131514510"></a>The value must be greater than or equal to 1.</p>
</td>
</tr>
<tr id="row641410102301"><td class="cellrowborder" valign="top" width="15.2984701529847%" headers="mcps1.1.5.1.1 "><p id="p11712134791515"><a name="p11712134791515"></a><a name="p11712134791515"></a>patience</p>
</td>
<td class="cellrowborder" valign="top" width="17.698230176982303%" headers="mcps1.1.5.1.2 "><p id="p2993101915163"><a name="p2993101915163"></a><a name="p2993101915163"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="32.436756324367565%" headers="mcps1.1.5.1.3 "><p id="p8712247141513"><a name="p8712247141513"></a><a name="p8712247141513"></a>Search patience value</p>
</td>
<td class="cellrowborder" valign="top" width="34.56654334566544%" headers="mcps1.1.5.1.4 "><p id="p57702186162"><a name="p57702186162"></a><a name="p57702186162"></a>The value must be greater than or equal to 1.</p>
</td>
</tr>
</tbody>
</table>

**Return Value<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>
<table><thead align="left"><tr id="row1569152711463"><th class="cellrowborder" valign="top" width="36.09%" id="mcps1.1.3.1.1"><p id="p146911527174618"><a name="p146911527174618"></a><a name="p146911527174618"></a>Data Type </p>
</th>
<th class="cellrowborder" valign="top" width="63.91%" id="mcps1.1.3.1.2"><p id="p136911627194618"><a name="p136911627194618"></a><a name="p136911627194618"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row769192744612"><td class="cellrowborder" valign="top" width="36.09%" headers="mcps1.1.3.1.1 "><p id="p106910272463"><a name="p106910272463"></a><a name="p106910272463"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="63.91%" headers="mcps1.1.3.1.2 "><p id="p2611111352313"><a name="p2611111352313"></a><a name="p2611111352313"></a>If the parameter value is not within the value range, <code>-1</code> is returned. If this API is called after BuildSearcher or Load/Deserialize/LoadGraph, <code>-1</code> is returned. In other cases, <code>0</code> is returned.</p>
</td>
</tr>
</tbody>
</table>

**Example**

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
    
    // Set the parameters for early stopping (call API before BuildSearcher).
    int adding_pref = 5;   // Threshold for inserting a hyperparameter candidate set.
    int patience = 10;     // Search patience value.
    
    int ret = index.SetEarlyStoppingParams(adding_pref, patience);
    
    if (ret == 0) {
        std::cout << "Parameters for early stopping successfully set" << std::endl;
    }
    
    // Then, build a searcher.
    index.BuildSearcher();
    
    return 0;
}
```

## Python

### API Description

[**Table 1**](#python-apis-provided-by-kbest) describes the Python APIs provided by KBest.

**Table 1** Python APIs provided by KBest <a id="python-apis-provided-by-kbest"></a>

<a name="table1194910128449"></a>
<table><thead align="left"><tr id="row99491812134412"><th class="cellrowborder" valign="top" width="31.269999999999996%" id="mcps1.2.3.1.1"><p id="p1794951224415"><a name="p1794951224415"></a><a name="p1794951224415"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="68.73%" id="mcps1.2.3.1.2"><p id="p6949612124415"><a name="p6949612124415"></a><a name="p6949612124415"></a>Function</p>
</th>
</tr>
</thead>
<tbody><tr id="row119491112174414"><td class="cellrowborder" valign="top" width="31.269999999999996%" headers="mcps1.2.3.1.1 "><p id="p1494931224410"><a name="p1494931224410"></a><a name="p1494931224410"></a>KBest</p>
</td>
<td class="cellrowborder" valign="top" width="68.73%" headers="mcps1.2.3.1.2 "><p id="p3949012174411"><a name="p3949012174411"></a><a name="p3949012174411"></a>Initializes the build of graph search (via default or parameterized constructor).</p>
</td>
</tr>
<tr id="row9949131219443"><td class="cellrowborder" valign="top" width="31.269999999999996%" headers="mcps1.2.3.1.1 "><p id="p1094921294415"><a name="p1094921294415"></a><a name="p1094921294415"></a>add</p>
</td>
<td class="cellrowborder" valign="top" width="68.73%" headers="mcps1.2.3.1.2 "><p id="p1794941284418"><a name="p1794941284418"></a><a name="p1794941284418"></a>Builds a graph index.</p>
</td>
</tr>
<tr id="row1511111561717"><td class="cellrowborder" valign="top" width="31.269999999999996%" headers="mcps1.2.3.1.1 "><p id="p10792123618373"><a name="p10792123618373"></a><a name="p10792123618373"></a>buildSearcher</p>
</td>
<td class="cellrowborder" valign="top" width="68.73%" headers="mcps1.2.3.1.2 "><p id="p379243633713"><a name="p379243633713"></a><a name="p379243633713"></a>Builds a searcher.</p>
</td>
</tr>
<tr id="row1594913120443"><td class="cellrowborder" valign="top" width="31.269999999999996%" headers="mcps1.2.3.1.1 "><p id="p4949012144417"><a name="p4949012144417"></a><a name="p4949012144417"></a>search</p>
</td>
<td class="cellrowborder" valign="top" width="68.73%" headers="mcps1.2.3.1.2 "><p id="p594911128445"><a name="p594911128445"></a><a name="p594911128445"></a>Searches for a graph.</p>
</td>
</tr>
<tr id="row6949131274416"><td class="cellrowborder" valign="top" width="31.269999999999996%" headers="mcps1.2.3.1.1 "><p id="p594971224411"><a name="p594971224411"></a><a name="p594971224411"></a>setEf</p>
</td>
<td class="cellrowborder" valign="top" width="68.73%" headers="mcps1.2.3.1.2 "><p id="p794971214414"><a name="p794971214414"></a><a name="p794971214414"></a>Sets the size of a candidate node list during search.</p>
</td>
</tr>
<tr id="row694916124445"><td class="cellrowborder" valign="top" width="31.269999999999996%" headers="mcps1.2.3.1.1 "><p id="p8949131214448"><a name="p8949131214448"></a><a name="p8949131214448"></a>save</p>
</td>
<td class="cellrowborder" valign="top" width="68.73%" headers="mcps1.2.3.1.2 "><p id="p894941210443"><a name="p894941210443"></a><a name="p894941210443"></a>Saves the searcher to a specified path.</p>
</td>
</tr>
<tr id="row159491712174414"><td class="cellrowborder" valign="top" width="31.269999999999996%" headers="mcps1.2.3.1.1 "><p id="p894991214449"><a name="p894991214449"></a><a name="p894991214449"></a>load</p>
</td>
<td class="cellrowborder" valign="top" width="68.73%" headers="mcps1.2.3.1.2 "><p id="p2094917128448"><a name="p2094917128448"></a><a name="p2094917128448"></a>Loads the searcher from the specified path.</p>
</td>
</tr>
<tr id="row1673619410185"><td class="cellrowborder" valign="top" width="31.269999999999996%" headers="mcps1.2.3.1.1 "><p id="p935410178398"><a name="p935410178398"></a><a name="p935410178398"></a>saveGraph</p>
</td>
<td class="cellrowborder" valign="top" width="68.73%" headers="mcps1.2.3.1.2 "><p id="p113548174390"><a name="p113548174390"></a><a name="p113548174390"></a>Saves the graph index to a specified path.</p>
</td>
</tr>
<tr id="row12461646151811"><td class="cellrowborder" valign="top" width="31.269999999999996%" headers="mcps1.2.3.1.1 "><p id="p0355121763910"><a name="p0355121763910"></a><a name="p0355121763910"></a>loadGraph</p>
</td>
<td class="cellrowborder" valign="top" width="68.73%" headers="mcps1.2.3.1.2 "><p id="p12355117103918"><a name="p12355117103918"></a><a name="p12355117103918"></a>Loads the graph index from the specified path.</p>
</td>
</tr>
<tr id="row55914831817"><td class="cellrowborder" valign="top" width="31.269999999999996%" headers="mcps1.2.3.1.1 "><p id="p108461119154212"><a name="p108461119154212"></a><a name="p108461119154212"></a>serialize</p>
</td>
<td class="cellrowborder" valign="top" width="68.73%" headers="mcps1.2.3.1.2 "><p id="p1584621994217"><a name="p1584621994217"></a><a name="p1584621994217"></a>Serializes the searcher content into an array.</p>
</td>
</tr>
<tr id="row169601149121817"><td class="cellrowborder" valign="top" width="31.269999999999996%" headers="mcps1.2.3.1.1 "><p id="p2846119204220"><a name="p2846119204220"></a><a name="p2846119204220"></a>deserialize</p>
</td>
<td class="cellrowborder" valign="top" width="68.73%" headers="mcps1.2.3.1.2 "><p id="p3403194411458"><a name="p3403194411458"></a><a name="p3403194411458"></a>Deserializes and restores the searcher content from the array.</p>
</td>
</tr>
<tr id="row26944513185"><td class="cellrowborder" valign="top" width="31.269999999999996%" headers="mcps1.2.3.1.1 "><p id="p7688749124717"><a name="p7688749124717"></a><a name="p7688749124717"></a>getNTotal</p>
</td>
<td class="cellrowborder" valign="top" width="68.73%" headers="mcps1.2.3.1.2 "><p id="p668874918478"><a name="p668874918478"></a><a name="p668874918478"></a>Returns the total number of data entries in the database within the graph index.</p>
</td>
</tr>
<tr id="row13483105413186"><td class="cellrowborder" valign="top" width="31.269999999999996%" headers="mcps1.2.3.1.1 "><p id="p09312186486"><a name="p09312186486"></a><a name="p09312186486"></a>getDim</p>
</td>
<td class="cellrowborder" valign="top" width="68.73%" headers="mcps1.2.3.1.2 "><p id="p39310182489"><a name="p39310182489"></a><a name="p39310182489"></a>Returns the dimensionality of the data in the graph index.</p>
</td>
</tr>
<tr id="row53311836151712"><td class="cellrowborder" valign="top" width="31.269999999999996%" headers="mcps1.2.3.1.1 "><p id="p227124617229"><a name="p227124617229"></a><a name="p227124617229"></a>setEarlyStoppingParams</p>
</td>
<td class="cellrowborder" valign="top" width="68.73%" headers="mcps1.2.3.1.2 "><p id="p87099445228"><a name="p87099445228"></a><a name="p87099445228"></a>Sets the parameters for early stopping optimization.</p>
</td>
</tr>
</tbody>
</table>

### Parameterized Constructor

**API Definition <a name="section172317194488"></a>**

class KBest\(dim: int, R: int, L: int, A: int, graph\_opt\_iter:int, metric: string, init\_builder\_type: string, index\_type: string, numa\_enabled: bool, numa\_nodes\_number: int\)

**API Function<a name="section1153124784912"></a>**

Initializes the build of graph search.

**Parameter Description <a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="18.099999999999998%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="15.36%" id="mcps1.1.5.1.2"><p id="p124241910191712"><a name="p124241910191712"></a><a name="p124241910191712"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="28.470000000000002%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="38.07%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="18.099999999999998%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>dim</p>
</td>
<td class="cellrowborder" valign="top" width="15.36%" headers="mcps1.1.5.1.2 "><p id="p164249104172"><a name="p164249104172"></a><a name="p164249104172"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="28.470000000000002%" headers="mcps1.1.5.1.3 "><p id="p182303331508"><a name="p182303331508"></a><a name="p182303331508"></a>Feature dimension</p>
</td>
<td class="cellrowborder" valign="top" width="38.07%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>[1,2999]</p>
</td>
</tr>
<tr id="row11230173385019"><td class="cellrowborder" valign="top" width="18.099999999999998%" headers="mcps1.1.5.1.1 "><p id="p22301333165015"><a name="p22301333165015"></a><a name="p22301333165015"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="15.36%" headers="mcps1.1.5.1.2 "><p id="p942481041718"><a name="p942481041718"></a><a name="p942481041718"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="28.470000000000002%" headers="mcps1.1.5.1.3 "><p id="p10230433115013"><a name="p10230433115013"></a><a name="p10230433115013"></a>Number of neighboring nodes</p>
</td>
<td class="cellrowborder" valign="top" width="38.07%" headers="mcps1.1.5.1.4 "><p id="p129897813251"><a name="p129897813251"></a><a name="p129897813251"></a>[11, 499]</p>
</td>
</tr>
<tr id="row14667192918485"><td class="cellrowborder" valign="top" width="18.099999999999998%" headers="mcps1.1.5.1.1 "><p id="p116802032174613"><a name="p116802032174613"></a><a name="p116802032174613"></a>L</p>
</td>
<td class="cellrowborder" valign="top" width="15.36%" headers="mcps1.1.5.1.2 "><p id="p1242415108176"><a name="p1242415108176"></a><a name="p1242415108176"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="28.470000000000002%" headers="mcps1.1.5.1.3 "><p id="p268013224617"><a name="p268013224617"></a><a name="p268013224617"></a>Size of the candidate node list during graph construction</p>
</td>
<td class="cellrowborder" valign="top" width="38.07%" headers="mcps1.1.5.1.4 "><p id="p6989158192510"><a name="p6989158192510"></a><a name="p6989158192510"></a>[11,1999]</p>
</td>
</tr>
<tr id="row17551732134814"><td class="cellrowborder" valign="top" width="18.099999999999998%" headers="mcps1.1.5.1.1 "><p id="p4597734184616"><a name="p4597734184616"></a><a name="p4597734184616"></a>A</p>
</td>
<td class="cellrowborder" valign="top" width="15.36%" headers="mcps1.1.5.1.2 "><p id="p2424101041714"><a name="p2424101041714"></a><a name="p2424101041714"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="28.470000000000002%" headers="mcps1.1.5.1.3 "><p id="p65975343465"><a name="p65975343465"></a><a name="p65975343465"></a>Angle threshold for pruning during graph construction</p>
</td>
<td class="cellrowborder" valign="top" width="38.07%" headers="mcps1.1.5.1.4 "><p id="p16989883251"><a name="p16989883251"></a><a name="p16989883251"></a>[11, 360]</p>
</td>
</tr>
<tr id="row188092073209"><td class="cellrowborder" valign="top" width="18.099999999999998%" headers="mcps1.1.5.1.1 "><p id="p9161114132017"><a name="p9161114132017"></a><a name="p9161114132017"></a>graph_opt_iter</p>
</td>
<td class="cellrowborder" valign="top" width="15.36%" headers="mcps1.1.5.1.2 "><p id="p18809137102014"><a name="p18809137102014"></a><a name="p18809137102014"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="28.470000000000002%" headers="mcps1.1.5.1.3 "><p id="p51611714162017"><a name="p51611714162017"></a><a name="p51611714162017"></a>Number of self-iterations for the graph index</p>
</td>
<td class="cellrowborder" valign="top" width="38.07%" headers="mcps1.1.5.1.4 "><p id="p180911714202"><a name="p180911714202"></a><a name="p180911714202"></a>[0,30]</p>
</td>
</tr>
<tr id="row523013315504"><td class="cellrowborder" valign="top" width="18.099999999999998%" headers="mcps1.1.5.1.1 "><p id="p10230123316509"><a name="p10230123316509"></a><a name="p10230123316509"></a>metric</p>
</td>
<td class="cellrowborder" valign="top" width="15.36%" headers="mcps1.1.5.1.2 "><p id="p19424710151712"><a name="p19424710151712"></a><a name="p19424710151712"></a> string.</p>
</td>
<td class="cellrowborder" valign="top" width="28.470000000000002%" headers="mcps1.1.5.1.3 "><p id="p102301133105015"><a name="p102301133105015"></a><a name="p102301133105015"></a>Distance metric </p>
</td>
<td class="cellrowborder" valign="top" width="38.07%" headers="mcps1.1.5.1.4 "><p id="p16989188132515"><a name="p16989188132515"></a><a name="p16989188132515"></a><span class="parmvalue" id="parmvalue07091746125712"><a name="parmvalue07091746125712"></a><a name="parmvalue07091746125712"></a><code>L2</code></span> or <span class="parmvalue" id="parmvalue112105525575"><a name="parmvalue112105525575"></a><a name="parmvalue112105525575"></a><code>IP</code></span>.</p>
<a name="ul194922278186"></a><a name="ul194922278186"></a><ul id="ul194922278186"><li><span class="parmvalue" id="parmvalue14698175535715"><a name="parmvalue14698175535715"></a><a name="parmvalue14698175535715"></a><code>L2</code></span>: Euclidean distance. </li><li><span class="parmvalue" id="parmvalue20513559115717"><a name="parmvalue20513559115717"></a><a name="parmvalue20513559115717"></a><code>IP</code></span>: inner product distance</li></ul>
</td>
</tr>
<tr id="row1523083315012"><td class="cellrowborder" valign="top" width="18.099999999999998%" headers="mcps1.1.5.1.1 "><p id="p10230433105020"><a name="p10230433105020"></a><a name="p10230433105020"></a>init_builder_type</p>
</td>
<td class="cellrowborder" valign="top" width="15.36%" headers="mcps1.1.5.1.2 "><p id="p34241210171720"><a name="p34241210171720"></a><a name="p34241210171720"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="28.470000000000002%" headers="mcps1.1.5.1.3 "><p id="p623053365015"><a name="p623053365015"></a><a name="p623053365015"></a>Algorithm for constructing the k-nearest neighbor graph.</p>
</td>
<td class="cellrowborder" valign="top" width="38.07%" headers="mcps1.1.5.1.4 "><p id="p9989158112520"><a name="p9989158112520"></a><a name="p9989158112520"></a><span class="parmvalue" id="parmvalue122210335814"><a name="parmvalue122210335814"></a><a name="parmvalue122210335814"></a><code>RNNDescent</code></span> and <span class="parmvalue" id="parmvalue1521813710584"><a name="parmvalue1521813710584"></a><a name="parmvalue1521813710584"></a><code>NNDescent</code></span>. Each represents an algorithm for constructing the k-nearest neighbor graph. <span class="parmvalue" id="parmvalue47521111175812"><a name="parmvalue47521111175812"></a><a name="parmvalue47521111175812"></a><code>RNNDescent</code></span> is recommended.</p>
</td>
</tr>
<tr id="row19521191612225"><td class="cellrowborder" valign="top" width="18.099999999999998%" headers="mcps1.1.5.1.1 "><p id="p1546185591017"><a name="p1546185591017"></a><a name="p1546185591017"></a>index_type</p>
</td>
<td class="cellrowborder" valign="top" width="15.36%" headers="mcps1.1.5.1.2 "><p id="p19131103031011"><a name="p19131103031011"></a><a name="p19131103031011"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="28.470000000000002%" headers="mcps1.1.5.1.3 "><p id="p55461255161011"><a name="p55461255161011"></a><a name="p55461255161011"></a>Neighbor selection strategy</p>
</td>
<td class="cellrowborder" valign="top" width="38.07%" headers="mcps1.1.5.1.4 "><p id="p213293001016"><a name="p213293001016"></a><a name="p213293001016"></a><span class="parmvalue" id="parmvalue3260403116"><a name="parmvalue3260403116"></a><a name="parmvalue3260403116"></a> <code>HNSW</code></span><span>, </span><span class="parmvalue" id="parmvalue41171544161114"><a name="parmvalue41171544161114"></a><a name="parmvalue41171544161114"></a> <code>NSG</code></span><span>, </span><span class="parmvalue" id="parmvalue1739675061118"><a name="parmvalue1739675061118"></a><a name="parmvalue1739675061118"></a> <code>TSDG</code></span><span>, or </span><span class="parmvalue" id="parmvalue5852453141117"><a name="parmvalue5852453141117"></a><a name="parmvalue5852453141117"></a> <code>SSG</code></span>: Each represents a neighbor selection strategy.</p>
</td>
</tr>
<tr id="row167566217421"><td class="cellrowborder" valign="top" width="18.099999999999998%" headers="mcps1.1.5.1.1 "><p id="p1575610224213"><a name="p1575610224213"></a><a name="p1575610224213"></a>numa_enabled</p>
</td>
<td class="cellrowborder" valign="top" width="15.36%" headers="mcps1.1.5.1.2 "><p id="p16424121021718"><a name="p16424121021718"></a><a name="p16424121021718"></a> Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="28.470000000000002%" headers="mcps1.1.5.1.3 "><p id="p87563211420"><a name="p87563211420"></a><a name="p87563211420"></a> Indicates whether to enable NUMA optimization.</p>
</td>
<td class="cellrowborder" valign="top" width="38.07%" headers="mcps1.1.5.1.4 "><p id="p1262653354620"><a name="p1262653354620"></a><a name="p1262653354620"></a>-</p>
</td>
</tr>
<tr id="row1020145194211"><td class="cellrowborder" valign="top" width="18.099999999999998%" headers="mcps1.1.5.1.1 "><p id="p1620145194210"><a name="p1620145194210"></a><a name="p1620145194210"></a>numa_nodes_number</p>
</td>
<td class="cellrowborder" valign="top" width="15.36%" headers="mcps1.1.5.1.2 "><p id="p4424410171711"><a name="p4424410171711"></a><a name="p4424410171711"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="28.470000000000002%" headers="mcps1.1.5.1.3 "><p id="p13201125144212"><a name="p13201125144212"></a><a name="p13201125144212"></a>Number of NUMA nodes.</p>
</td>
<td class="cellrowborder" valign="top" width="38.07%" headers="mcps1.1.5.1.4 "><p id="p13626333134613"><a name="p13626333134613"></a><a name="p13626333134613"></a>The value must be greater than or equal to 1.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```python
import numpy as np
import kbest

# Parameter configuration
dim = 128              # Feature dimension
R = 32                 # Number of neighboring nodes
L = 200                # Size of the candidate node list during graph construction
A = 60                # Angle threshold for pruning during graph construction
graph_opt_iter = 2     # Number of self-iterations for the graph index

# Create an index (without NUMA optimization).
index = kbest.KBest(dim, R, L, A, graph_opt_iter, "L2", "RNNDescent", "HNSW", False, 1)

print(f"KBest index successfully created. Dimension: {index.getDim()}")
```

### Default Constructor

**API Definition <a name="section172317194488"></a>**

class KBest\(\)

**API Function<a name="section1153124784912"></a>**

Initializes the build of graph search without arguments.

**Parameter Description <a name="section157501312135019"></a>**

None

**Example**

```python
import kbest

# Default constructor, used for loading a previously saved index.
index = kbest.KBest()

# Load a searcher from a file.
ret = index.load("./saved_index.bin")
if ret == 0:
    print("Index successfully loaded")
    print(f"Data dimension: {index.getDim()}")
    print(f"Number of data entries in the database: {index.getNTotal()}")
```

### add

**API Definition <a name="section172317194488"></a>**

def add\(nb:int, xb: numpy.ndarray, consecutive: int, reorder: int, level: int\) -\> int

**API Function<a name="section1153124784912"></a>**

Builds a graph index.

**Parameter Description <a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="18.05%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="17.75%" id="mcps1.1.5.1.2"><p id="p117938514184"><a name="p117938514184"></a><a name="p117938514184"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="26.69%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="37.51%" id="mcps1.1.5.1.4"><p id="p18686165314813"><a name="p18686165314813"></a><a name="p18686165314813"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="18.05%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>nb</p>
</td>
<td class="cellrowborder" valign="top" width="17.75%" headers="mcps1.1.5.1.2 "><p id="p679315141818"><a name="p679315141818"></a><a name="p679315141818"></a><span>int</span></p>
</td>
<td class="cellrowborder" valign="top" width="26.69%" headers="mcps1.1.5.1.3 "><p id="p182303331508"><a name="p182303331508"></a><a name="p182303331508"></a>Number of data entries in the vector database</p>
</td>
<td class="cellrowborder" valign="top" width="37.51%" headers="mcps1.1.5.1.4 "><p id="p1151275553412"><a name="p1151275553412"></a><a name="p1151275553412"></a>The value must be greater than or equal to 1. It is recommended that the value be less than 1 billion.</p>
</td>
</tr>
<tr id="row11230173385019"><td class="cellrowborder" valign="top" width="18.05%" headers="mcps1.1.5.1.1 "><p id="p22301333165015"><a name="p22301333165015"></a><a name="p22301333165015"></a>xb</p>
</td>
<td class="cellrowborder" valign="top" width="17.75%" headers="mcps1.1.5.1.2 "><p id="p4793135121812"><a name="p4793135121812"></a><a name="p4793135121812"></a>numpy.ndarray</p>
</td>
<td class="cellrowborder" valign="top" width="26.69%" headers="mcps1.1.5.1.3 "><p id="p10230433115013"><a name="p10230433115013"></a><a name="p10230433115013"></a>Vector database data</p>
</td>
<td class="cellrowborder" valign="top" width="37.51%" headers="mcps1.1.5.1.4 "><p id="p1218364610343"><a name="p1218364610343"></a><a name="p1218364610343"></a>It cannot be null. The length must be <code>nb</code> × <code>dim</code> (number of vectors × feature dimension).</p>
</td>
</tr>
<tr id="row92309336505"><td class="cellrowborder" valign="top" width="18.05%" headers="mcps1.1.5.1.1 "><p id="p162309336505"><a name="p162309336505"></a><a name="p162309336505"></a>consecutive</p>
</td>
<td class="cellrowborder" valign="top" width="17.75%" headers="mcps1.1.5.1.2 "><p id="p3793145191818"><a name="p3793145191818"></a><a name="p3793145191818"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="26.69%" headers="mcps1.1.5.1.3 "><p id="p92301933165017"><a name="p92301933165017"></a><a name="p92301933165017"></a>Block size</p>
</td>
<td class="cellrowborder" valign="top" width="37.51%" headers="mcps1.1.5.1.4 "><p id="p1151265503419"><a name="p1151265503419"></a><a name="p1151265503419"></a>[1,31]</p>
</td>
</tr>
<tr id="row11317866249"><td class="cellrowborder" valign="top" width="18.05%" headers="mcps1.1.5.1.1 "><p id="p1231811620244"><a name="p1231811620244"></a><a name="p1231811620244"></a><span>reorder</span></p>
</td>
<td class="cellrowborder" valign="top" width="17.75%" headers="mcps1.1.5.1.2 "><p id="p5318860247"><a name="p5318860247"></a><a name="p5318860247"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="26.69%" headers="mcps1.1.5.1.3 "><p id="p631856102414"><a name="p631856102414"></a><a name="p631856102414"></a>Indicates whether to enable reordering of database vectors.</p>
</td>
<td class="cellrowborder" valign="top" width="37.51%" headers="mcps1.1.5.1.4 "><p id="p231813619242"><a name="p231813619242"></a><a name="p231813619242"></a><code>0</code> or <code>1</code>.</p>
</td>
</tr>
<tr id="row523013315504"><td class="cellrowborder" valign="top" width="18.05%" headers="mcps1.1.5.1.1 "><p id="p10230123316509"><a name="p10230123316509"></a><a name="p10230123316509"></a>level</p>
</td>
<td class="cellrowborder" valign="top" width="17.75%" headers="mcps1.1.5.1.2 "><p id="p3793051201812"><a name="p3793051201812"></a><a name="p3793051201812"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="26.69%" headers="mcps1.1.5.1.3 "><p id="p102301133105015"><a name="p102301133105015"></a><a name="p102301133105015"></a>Quantization level</p>
</td>
<td class="cellrowborder" valign="top" width="37.51%" headers="mcps1.1.5.1.4 "><p id="p1051225510340"><a name="p1051225510340"></a><a name="p1051225510340"></a>[0, 3]</p>
<a name="ul1454195619238"></a><a name="ul1454195619238"></a><ul id="ul1454195619238"><li><code>0</code>: FP32 quantization </li><li><code>1</code>: SQ8U quantization </li><li><code>2</code>: SQ4U quantization </li><li><code>3</code>: FP16 quantization</li></ul>
</td>
</tr>
</tbody>
</table>

**Return Value<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>
<table><thead align="left"><tr id="row1569152711463"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p146911527174618"><a name="p146911527174618"></a><a name="p146911527174618"></a>Data Type </p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p136911627194618"><a name="p136911627194618"></a><a name="p136911627194618"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row769192744612"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p106910272463"><a name="p106910272463"></a><a name="p106910272463"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p2611111352313"><a name="p2611111352313"></a><a name="p2611111352313"></a>This API is a wrapper for an underlying C++ API, which controls exception handling.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```python
import numpy as np
import kbest

dim = 128
nb = 10000  # Number of database vectors

# Create an index.
index = kbest.KBest(dim, 32, 200, 60, 2, "L2", "RNNDescent", "HNSW", False, 1)

# Prepare database data.
xb = np.random.random((nb, dim)).astype(np.float32)

# Build a graph index.
consecutive = 16  # Block size
reorder = 1 # Enable reordering of database vectors.
level = 0         # FP32 quantization

ret = index.add(nb, xb, consecutive, reorder, level)

if ret == 0:
    print("Graph index created successfully.")
    print(f"Data entries in the database: {index.getNTotal()}")
else:
    print(f"Failed to create the graph index. Error code: {ret}")
```

### buildSearcher

**API Definition <a name="section172317194488"></a>**

def buildSearcher\(\) -\> int

**API Function<a name="section1153124784912"></a>**

Builds a searcher using the <code>level</code> parameter from the Add API as the quantization parameter.

**Parameter Description <a name="section157501312135019"></a>**

None

**Return Value<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>
<table><thead align="left"><tr id="row1569152711463"><th class="cellrowborder" valign="top" width="34.599999999999994%" id="mcps1.1.3.1.1"><p id="p146911527174618"><a name="p146911527174618"></a><a name="p146911527174618"></a>Data Type </p>
</th>
<th class="cellrowborder" valign="top" width="65.4%" id="mcps1.1.3.1.2"><p id="p136911627194618"><a name="p136911627194618"></a><a name="p136911627194618"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row769192744612"><td class="cellrowborder" valign="top" width="34.599999999999994%" headers="mcps1.1.3.1.1 "><p id="p106910272463"><a name="p106910272463"></a><a name="p106910272463"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="65.4%" headers="mcps1.1.3.1.2 "><p id="p17947191512276"><a name="p17947191512276"></a><a name="p17947191512276"></a>This API is a wrapper for an underlying C++ API, which controls exception handling.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```python
import numpy as np
import kbest

dim = 128
nb = 10000

# Create an index.
index = kbest.KBest(dim, 32, 200, 60, 2, "L2", "RNNDescent", "HNSW", False, 1)

# Add database data.
xb = np.random.random((nb, dim)).astype(np.float32)
index.add(nb, xb, 16, 1, 0)

# Build a searcher.
ret = index.buildSearcher()

if ret == 0:
    print ("Searcher created successfully, ready for search")
else:
    print ("Failed to build the searcher")
```

### search<a name="ZH-CN_TOPIC_0000002549873553"></a>

**API Definition <a name="section172317194488"></a>**

def search\(nq: int, xq: numpy.ndarray, topk: int, distances: numpy.ndarray, labels: numpy.ndarray, num\_threads: int\) -\> int

**API Function<a name="section1153124784912"></a>**

Searches for a graph.

**Parameter Description <a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="14.14%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="21.36%" id="mcps1.1.5.1.2"><p id="p1192894081911"><a name="p1192894081911"></a><a name="p1192894081911"></a> Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="28.65%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="35.85%" id="mcps1.1.5.1.4"><p id="p18686165314813"><a name="p18686165314813"></a><a name="p18686165314813"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>nq</p>
</td>
<td class="cellrowborder" valign="top" width="21.36%" headers="mcps1.1.5.1.2 "><p id="p179282406193"><a name="p179282406193"></a><a name="p179282406193"></a><span>int</span></p>
</td>
<td class="cellrowborder" valign="top" width="28.65%" headers="mcps1.1.5.1.3 "><p id="p182303331508"><a name="p182303331508"></a><a name="p182303331508"></a>Number of query vectors</p>
</td>
<td class="cellrowborder" valign="top" width="35.85%" headers="mcps1.1.5.1.4 "><p id="p1446074319406"><a name="p1446074319406"></a><a name="p1446074319406"></a>The value must be greater than or equal to 1. It is recommended that the value be less than 1 billion.</p>
</td>
</tr>
<tr id="row11230173385019"><td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.1.5.1.1 "><p id="p22301333165015"><a name="p22301333165015"></a><a name="p22301333165015"></a>xq</p>
</td>
<td class="cellrowborder" valign="top" width="21.36%" headers="mcps1.1.5.1.2 "><p id="p1792864071912"><a name="p1792864071912"></a><a name="p1792864071912"></a>numpy.ndarray</p>
</td>
<td class="cellrowborder" valign="top" width="28.65%" headers="mcps1.1.5.1.3 "><p id="p10230433115013"><a name="p10230433115013"></a><a name="p10230433115013"></a>Query vector data</p>
</td>
<td class="cellrowborder" valign="top" width="35.85%" headers="mcps1.1.5.1.4 "><p id="p19460943204013"><a name="p19460943204013"></a><a name="p19460943204013"></a>It cannot be null, <span>and the expected length is <code>nq</code> × <code>dim</code></span> (number of vectors × feature dimension).</p>
</td>
</tr>
<tr id="row92309336505"><td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.1.5.1.1 "><p id="p162309336505"><a name="p162309336505"></a><a name="p162309336505"></a>topk</p>
</td>
<td class="cellrowborder" valign="top" width="21.36%" headers="mcps1.1.5.1.2 "><p id="p692844014192"><a name="p692844014192"></a><a name="p692844014192"></a><span>int</span></p>
</td>
<td class="cellrowborder" valign="top" width="28.65%" headers="mcps1.1.5.1.3 "><p id="p92301933165017"><a name="p92301933165017"></a><a name="p92301933165017"></a>Number of nearest neighbors</p>
</td>
<td class="cellrowborder" valign="top" width="35.85%" headers="mcps1.1.5.1.4 "><p id="p1178758184115"><a name="p1178758184115"></a><a name="p1178758184115"></a>[1, nb], where <span class="parmname" id="parmname201022052769"><a name="parmname201022052769"></a><a name="parmname201022052769"></a><code>nb</code></span> indicates the number of data entries in the vector database.</p>
</td>
</tr>
<tr id="row33251301573"><td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.1.5.1.1 "><p id="p83251102715"><a name="p83251102715"></a><a name="p83251102715"></a><span>distances</span></p>
</td>
<td class="cellrowborder" valign="top" width="21.36%" headers="mcps1.1.5.1.2 "><p id="p9928140121918"><a name="p9928140121918"></a><a name="p9928140121918"></a>numpy.ndarray</p>
</td>
<td class="cellrowborder" valign="top" width="28.65%" headers="mcps1.1.5.1.3 "><p id="p8325130776"><a name="p8325130776"></a><a name="p8325130776"></a>Distance array</p>
</td>
<td class="cellrowborder" valign="top" width="35.85%" headers="mcps1.1.5.1.4 "><p id="p1218364610343"><a name="p1218364610343"></a><a name="p1218364610343"></a>It cannot be null, and <span>the expected length is <code>nq</code> × <code>topk</code></span>.</p>
</td>
</tr>
<tr id="row17889102871"><td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.1.5.1.1 "><p id="p1188922077"><a name="p1188922077"></a><a name="p1188922077"></a>labels</p>
</td>
<td class="cellrowborder" valign="top" width="21.36%" headers="mcps1.1.5.1.2 "><p id="p14928164014191"><a name="p14928164014191"></a><a name="p14928164014191"></a>numpy.ndarray</p>
</td>
<td class="cellrowborder" valign="top" width="28.65%" headers="mcps1.1.5.1.3 "><p id="p1889122372"><a name="p1889122372"></a><a name="p1889122372"></a>ID array of search results</p>
</td>
<td class="cellrowborder" valign="top" width="35.85%" headers="mcps1.1.5.1.4 "><p id="p13889132574"><a name="p13889132574"></a><a name="p13889132574"></a>It cannot be null, and <span>the expected length is <code>nq</code> × <code>topk</code></span>.</p>
</td>
</tr>
<tr id="row177151948121320"><td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.1.5.1.1 "><p id="p3715448191319"><a name="p3715448191319"></a><a name="p3715448191319"></a>num_threads</p>
</td>
<td class="cellrowborder" valign="top" width="21.36%" headers="mcps1.1.5.1.2 "><p id="p5928440101919"><a name="p5928440101919"></a><a name="p5928440101919"></a><span>int</span></p>
</td>
<td class="cellrowborder" valign="top" width="28.65%" headers="mcps1.1.5.1.3 "><p id="p137151148161319"><a name="p137151148161319"></a><a name="p137151148161319"></a>Number of threads used for search</p>
</td>
<td class="cellrowborder" valign="top" width="35.85%" headers="mcps1.1.5.1.4 "><p id="p95801533174311"><a name="p95801533174311"></a><a name="p95801533174311"></a>[1, std::thread::hardware_concurrency()], where <code>std::thread::hardware_concurrency()</code> indicates <span>the number of concurrent threads supported by the current system</span>.</p>
</td>
</tr>
</tbody>
</table>

**Return Value<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>
<table><thead align="left"><tr id="row1569152711463"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p146911527174618"><a name="p146911527174618"></a><a name="p146911527174618"></a>Data Type </p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p136911627194618"><a name="p136911627194618"></a><a name="p136911627194618"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row769192744612"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p106910272463"><a name="p106910272463"></a><a name="p106910272463"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p2611111352313"><a name="p2611111352313"></a><a name="p2611111352313"></a>This API is a wrapper for an underlying C++ API, which controls exception handling.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```python
import numpy as np
import kbest

dim = 128
nb = 10000
nq = 10      # Number of query vectors
topk = 5      # Return top five nearest neighbors.

# Create and build an index.
index = kbest.KBest(dim, 32, 200, 60, 2, "L2", "RNNDescent", "HNSW", False, 1)

xb = np.random.random((nb, dim)).astype(np.float32)
index.add(nb, xb, 16, 1, 0)
index.buildSearcher()

# Prepare the query vectors.
xq = np.random.random((nq, dim)).astype(np.float32)

# Prepare the result array.
distances = np.zeros((nq, topk), dtype=np.float32)
labels = np.zeros((nq, topk), dtype=np.int64)

# Perform search.
num_threads = 4
ret = index.search(nq, xq, topk, distances, labels, num_threads)

if ret == 0:
    print("Search succeeded")
    print(f"Nearest neighbor of query vector 0: ")
    for i in range(topk):
        print(f"  ID: {labels[0, i]}, distance: {distances[0, i]}")
```

### setEf

**API Definition <a name="section172317194488"></a>**

def setEf\(ef: int\) -\> int

**API Function<a name="section1153124784912"></a>**

Sets the size of the candidate node list during search.

**Parameter Description <a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="14.08%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="22.64%" id="mcps1.1.5.1.2"><p id="p854220356207"><a name="p854220356207"></a><a name="p854220356207"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="26.810000000000002%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="36.47%" id="mcps1.1.5.1.4"><p id="p1440932116441"><a name="p1440932116441"></a><a name="p1440932116441"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="14.08%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>ef</p>
</td>
<td class="cellrowborder" valign="top" width="22.64%" headers="mcps1.1.5.1.2 "><p id="p1754243572014"><a name="p1754243572014"></a><a name="p1754243572014"></a><span>int</span></p>
</td>
<td class="cellrowborder" valign="top" width="26.810000000000002%" headers="mcps1.1.5.1.3 "><p id="p39711451181514"><a name="p39711451181514"></a><a name="p39711451181514"></a>Size of the candidate node list during search</p>
</td>
<td class="cellrowborder" valign="top" width="36.47%" headers="mcps1.1.5.1.4 "><p id="p1667165924518"><a name="p1667165924518"></a><a name="p1667165924518"></a>[1, nb], where <span class="parmname" id="parmname336535516614"><a name="parmname336535516614"></a><a name="parmname336535516614"></a><code>nb</code></span> indicates the number of data entries in the vector database.</p>
</td>
</tr>
</tbody>
</table>

**Return Value<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>
<table><thead align="left"><tr id="row1569152711463"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p146911527174618"><a name="p146911527174618"></a><a name="p146911527174618"></a>Data Type </p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p136911627194618"><a name="p136911627194618"></a><a name="p136911627194618"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row769192744612"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p106910272463"><a name="p106910272463"></a><a name="p106910272463"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p2611111352313"><a name="p2611111352313"></a><a name="p2611111352313"></a>This API is a wrapper for an underlying C++ API, which controls exception handling.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```python
import numpy as np
import kbest

dim = 128
nb = 10000

# Create and build an index.
index = kbest.KBest(dim, 32, 200, 60, 2, "L2", "RNNDescent", "HNSW", False, 1)

xb = np.random.random((nb, dim)).astype(np.float32)
index.add(nb, xb, 16, 1, 0)
index.buildSearcher()

# Set a small ef value (faster search, but lower accuracy).
index.setEf(50)
print ("Searching with ef=50...")

# Set a large ef value (slower search, but higher accuracy).
ret = index.setEf(200)
if ret == 0:
    print ("Successfully set ef=200")
```

### save

**API Definition <a name="section172317194488"></a>**

def save\(path: string\) -\> int

**API Function<a name="section1153124784912"></a>**

Saves a searcher to a specified path in a single process.

**Parameter Description <a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="16.009999999999998%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="19.49%" id="mcps1.1.5.1.2"><p id="p8128856112017"><a name="p8128856112017"></a><a name="p8128856112017"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="30.12%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="33.083308330833084%" id="mcps1.1.5.1.4"><p id="p1440932116441"><a name="p1440932116441"></a><a name="p1440932116441"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="16.009999999999998%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>path</p>
</td>
<td class="cellrowborder" valign="top" width="19.49%" headers="mcps1.1.5.1.2 "><p id="p1112855612010"><a name="p1112855612010"></a><a name="p1112855612010"></a> String</p>
</td>
<td class="cellrowborder" valign="top" width="30.12%" headers="mcps1.1.5.1.3 "><p id="p39711451181514"><a name="p39711451181514"></a><a name="p39711451181514"></a>Path for storing the searcher</p>
</td>
<td class="cellrowborder" valign="top" width="34.38%" headers="mcps1.1.5.1.4 "><p id="p20167131514510"><a name="p20167131514510"></a><a name="p20167131514510"></a>The value contains less than 199 characters.</p>
</td>
</tr>
</tbody>
</table>

**Return Value<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>
<table><thead align="left"><tr id="row1569152711463"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p146911527174618"><a name="p146911527174618"></a><a name="p146911527174618"></a>Data Type </p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p136911627194618"><a name="p136911627194618"></a><a name="p136911627194618"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row769192744612"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p106910272463"><a name="p106910272463"></a><a name="p106910272463"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p2611111352313"><a name="p2611111352313"></a><a name="p2611111352313"></a>This API is a wrapper for an underlying C++ API, which controls exception handling.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```python
import numpy as np
import kbest

dim = 128
nb = 10000

# Create and build an index.
index = kbest.KBest(dim, 32, 200, 60, 2, "L2", "RNNDescent", "HNSW", False, 1)

xb = np.random.random((nb, dim)).astype(np.float32)
index.add(nb, xb, 16, 1, 0)
index.buildSearcher()

# Save the searcher.
ret = index.save("./kbest_index.bin")

if ret == 0:
    print("Searcher successfully saved to ./kbest_index.bin successfully.")
else:
    print ("Failed to save the searcher")
```

### load

**API Definition <a name="section172317194488"></a>**

def load\(path: string\) -\> int

**API Function<a name="section1153124784912"></a>**

Loads a searcher from a specified path.

**Parameter Description <a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="17.21%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="18.82%" id="mcps1.1.5.1.2"><p id="p8128856112017"><a name="p8128856112017"></a><a name="p8128856112017"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="29.74%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="34.23%" id="mcps1.1.5.1.4"><p id="p1440932116441"><a name="p1440932116441"></a><a name="p1440932116441"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="17.21%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>path</p>
</td>
<td class="cellrowborder" valign="top" width="18.82%" headers="mcps1.1.5.1.2 "><p id="p1112855612010"><a name="p1112855612010"></a><a name="p1112855612010"></a> String</p>
</td>
<td class="cellrowborder" valign="top" width="29.74%" headers="mcps1.1.5.1.3 "><p id="p39711451181514"><a name="p39711451181514"></a><a name="p39711451181514"></a>Path from which the searcher is loaded</p>
</td>
<td class="cellrowborder" valign="top" width="34.23%" headers="mcps1.1.5.1.4 "><p id="p20167131514510"><a name="p20167131514510"></a><a name="p20167131514510"></a>The value contains less than 199 characters.</p>
</td>
</tr>
</tbody>
</table>

**Return Value<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p19997736105"><a name="p19997736105"></a><a name="p19997736105"></a>This API is a wrapper for an underlying C++ API, which controls exception handling.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```python
import numpy as np
import kbest

# Create an index instance using the default constructor.
index = kbest.KBest()

# Load a searcher from a file.
ret = index.load("./kbest_index.bin")

if ret == 0:
    print("Searcher successfully loaded")
    print(f"Data dimension: {index.getDim()}")
    print(f"Data entries in the database: {index.getNTotal()}")
    
    # Once loaded, the searcher is ready for search.
    nq = 1
    topk = 5
    dim = index.getDim()
    
    xq = np.random.random((nq, dim)).astype(np.float32)
    distances = np.zeros((nq, topk), dtype=np.float32)
    labels = np.zeros((nq, topk), dtype=np.int64)
    
    index.search(nq, xq, topk, distances, labels, 4)
else:
    print("Failed to load the searcher")
```

### saveGraph

**API Definition <a name="section172317194488"></a>**

def saveGraph\(path: string\) -\> int

**API Function<a name="section1153124784912"></a>**

Saves a graph index to a specified path in a single process.

**Parameter Description <a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="16.20837916208379%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="20.3979602039796%" id="mcps1.1.5.1.2"><p id="p8128856112017"><a name="p8128856112017"></a><a name="p8128856112017"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="27.947205279472055%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="35.446455354464554%" id="mcps1.1.5.1.4"><p id="p1440932116441"><a name="p1440932116441"></a><a name="p1440932116441"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="16.20837916208379%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>path</p>
</td>
<td class="cellrowborder" valign="top" width="20.3979602039796%" headers="mcps1.1.5.1.2 "><p id="p1112855612010"><a name="p1112855612010"></a><a name="p1112855612010"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="27.947205279472055%" headers="mcps1.1.5.1.3 "><p id="p39711451181514"><a name="p39711451181514"></a><a name="p39711451181514"></a>Path for storing the graph index</p>
</td>
<td class="cellrowborder" valign="top" width="35.446455354464554%" headers="mcps1.1.5.1.4 "><p id="p20167131514510"><a name="p20167131514510"></a><a name="p20167131514510"></a>The value contains less than 199 characters.</p>
</td>
</tr>
</tbody>
</table>

**Return Value<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>
<table><thead align="left"><tr id="row1569152711463"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p146911527174618"><a name="p146911527174618"></a><a name="p146911527174618"></a>Data Type </p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p136911627194618"><a name="p136911627194618"></a><a name="p136911627194618"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row769192744612"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p106910272463"><a name="p106910272463"></a><a name="p106910272463"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p2611111352313"><a name="p2611111352313"></a><a name="p2611111352313"></a>This API is a wrapper for an underlying C++ API, which controls exception handling.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```python
import numpy as np
import kbest

dim = 128
nb = 10000

# Create an index and add data.
index = kbest.KBest(dim, 32, 200, 60, 2, "L2", "RNNDescent", "HNSW", False, 1)

xb = np.random.random((nb, dim)).astype(np.float32)
index.add(nb, xb, 16, 1, 0)

# Save the graph index before calling buildSearcher.
ret = index.saveGraph("./kbest_graph.bin")

if ret == 0:
    print("Graph index successfully saved to ./kbest_graph.bin successfully.")
else:
    print ("Failed to save the graph index")
```

### loadGraph

**API Definition <a name="section172317194488"></a>**

def load\(path: string, level: int\) -\> int

**API Function<a name="section1153124784912"></a>**

Loads a searcher from a specified path.

**Parameter Description <a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.14%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="17.91%" id="mcps1.1.5.1.2"><p id="p8128856112017"><a name="p8128856112017"></a><a name="p8128856112017"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="21.78%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="45.17%" id="mcps1.1.5.1.4"><p id="p1440932116441"><a name="p1440932116441"></a><a name="p1440932116441"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.14%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>path</p>
</td>
<td class="cellrowborder" valign="top" width="17.91%" headers="mcps1.1.5.1.2 "><p id="p1112855612010"><a name="p1112855612010"></a><a name="p1112855612010"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="21.78%" headers="mcps1.1.5.1.3 "><p id="p39711451181514"><a name="p39711451181514"></a><a name="p39711451181514"></a>Path from which the searcher is loaded</p>
</td>
<td class="cellrowborder" valign="top" width="45.17%" headers="mcps1.1.5.1.4 "><p id="p20167131514510"><a name="p20167131514510"></a><a name="p20167131514510"></a>The value contains less than 199 characters.</p>
</td>
</tr>
<tr id="row412192193411"><td class="cellrowborder" valign="top" width="15.14%" headers="mcps1.1.5.1.1 "><p id="p19414810153017"><a name="p19414810153017"></a><a name="p19414810153017"></a>level</p>
</td>
<td class="cellrowborder" valign="top" width="17.91%" headers="mcps1.1.5.1.2 "><p id="p17614134914213"><a name="p17614134914213"></a><a name="p17614134914213"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="21.78%" headers="mcps1.1.5.1.3 "><p id="p5414151014309"><a name="p5414151014309"></a><a name="p5414151014309"></a>Quantization level</p>
</td>
<td class="cellrowborder" valign="top" width="45.17%" headers="mcps1.1.5.1.4 "><p id="p14665102215"><a name="p14665102215"></a><a name="p14665102215"></a>[-1,3]</p>
<a name="ul1454195619238"></a><a name="ul1454195619238"></a><ul id="ul1454195619238"><li><code>-1</code>: default value, indicating the quantization level saved during the saveGraph operation. </li><li><code>0</code>: FP32 quantization </li><li><code>1</code>: SQ8U quantization </li><li><code>2</code>: SQ4U quantization </li><li><code>3</code>: FP16 quantization</li></ul>
</td>
</tr>
</tbody>
</table>

**Return Value<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p19997736105"><a name="p19997736105"></a><a name="p19997736105"></a>This API is a wrapper for an underlying C++ API, which controls exception handling.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```python
import numpy as np
import kbest

# Create an index instance using the default constructor.
index = kbest.KBest()

# Load the graph index from a file and use the quantization level saved with it.
ret = index.loadGraph("./kbest_graph.bin", -1)

if ret == 0:
    print("Graph index loaded successfully.")
    print(f"Data dimension: {index.getDim()}")
    print(f"Data entries in the database: {index.getNTotal()}")
    
    # Once loaded, the searcher is ready for search.
    nq = 1
    topk = 5
    dim = index.getDim()
    
    xq = np.random.random((nq, dim)).astype(np.float32)
    distances = np.zeros((nq, topk), dtype=np.float32)
    labels = np.zeros((nq, topk), dtype=np.int64)
    
    index.search(nq, xq, topk, distances, labels, 4)
```

### serialize

**API Definition <a name="section172317194488"></a>**

def serialize\(\) -\> numpy.ndarray

**API Function<a name="section1153124784912"></a>**

Serialize the searcher content into an array.

**Parameter Description <a name="section157501312135019"></a>**

None

**Return Value<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>
<table><thead align="left"><tr id="row1569152711463"><th class="cellrowborder" valign="top" width="36.96%" id="mcps1.1.3.1.1"><p id="p146911527174618"><a name="p146911527174618"></a><a name="p146911527174618"></a>Data Type </p>
</th>
<th class="cellrowborder" valign="top" width="63.04%" id="mcps1.1.3.1.2"><p id="p136911627194618"><a name="p136911627194618"></a><a name="p136911627194618"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row769192744612"><td class="cellrowborder" valign="top" width="36.96%" headers="mcps1.1.3.1.1 "><p id="p106910272463"><a name="p106910272463"></a><a name="p106910272463"></a>numpy.ndarray</p>
</td>
<td class="cellrowborder" valign="top" width="63.04%" headers="mcps1.1.3.1.2 "><p id="p14753115604612"><a name="p14753115604612"></a><a name="p14753115604612"></a>Array that stores the searcher content</p>
</td>
</tr>
</tbody>
</table>

**Example**

```python
import numpy as np
import kbest

dim = 128
nb = 10000

# Create an index and add data.
index = kbest.KBest(dim, 32, 200, 60, 2, "L2", "RNNDescent", "HNSW", False, 1)

xb = np.random.random((nb, dim)).astype(np.float32)
index.add(nb, xb, 16, 1, 0)

# Serialize the searcher content into an array.
data_arr = index.serialize()

print(f"Serialization succeeded. Data length: {len(data_arr)} bytes")

# You can store data_arr in the database.
```

### deserialize

**API Definition <a name="section172317194488"></a>**

def deserialize\(data\_arr: numpy.ndarray\) -\> int

**API Function<a name="section1153124784912"></a>**

Restores a search index instance from a serialized data array.

**Parameter Description <a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.09%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="16.71%" id="mcps1.1.5.1.2"><p id="p654931862217"><a name="p654931862217"></a><a name="p654931862217"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="21.64%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="46.56%" id="mcps1.1.5.1.4"><p id="p1440932116441"><a name="p1440932116441"></a><a name="p1440932116441"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.09%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>data_arr</p>
</td>
<td class="cellrowborder" valign="top" width="16.71%" headers="mcps1.1.5.1.2 "><p id="p2054931812228"><a name="p2054931812228"></a><a name="p2054931812228"></a>numpy.ndarray</p>
</td>
<td class="cellrowborder" valign="top" width="21.64%" headers="mcps1.1.5.1.3 "><p id="p39711451181514"><a name="p39711451181514"></a><a name="p39711451181514"></a>Array for storing the searcher content.</p>
</td>
<td class="cellrowborder" valign="top" width="46.56%" headers="mcps1.1.5.1.4 "><p id="p20167131514510"><a name="p20167131514510"></a><a name="p20167131514510"></a>The start address of the array for storing the searcher content cannot be null. The length of this array is the array length saved when the serialize API is called.</p>
</td>
</tr>
</tbody>
</table>

**Return Value<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>
<table><thead align="left"><tr id="row1569152711463"><th class="cellrowborder" valign="top" width="36.96%" id="mcps1.1.3.1.1"><p id="p146911527174618"><a name="p146911527174618"></a><a name="p146911527174618"></a>Data Type </p>
</th>
<th class="cellrowborder" valign="top" width="63.04%" id="mcps1.1.3.1.2"><p id="p136911627194618"><a name="p136911627194618"></a><a name="p136911627194618"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row769192744612"><td class="cellrowborder" valign="top" width="36.96%" headers="mcps1.1.3.1.1 "><p id="p106910272463"><a name="p106910272463"></a><a name="p106910272463"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="63.04%" headers="mcps1.1.3.1.2 "><p id="p19997736105"><a name="p19997736105"></a><a name="p19997736105"></a>This API is a wrapper for an underlying C++ API, which controls exception handling.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```python
import numpy as np
import kbest

dim = 128
nb = 10000

# Create an index and serialize it.
index1 = kbest.KBest(dim, 32, 200, 60, 2, "L2", "RNNDescent", "HNSW", False, 1)

xb = np.random.random((nb, dim)).astype(np.float32)
index1.add(nb, xb, 16, 1, 0)

data_arr = index1.serialize()

# Restore the index from the serialized data.
index2 = kbest.KBest()
ret = index2.deserialize(data_arr)

if ret == 0:
    print("Deserialization succeeded")
    print(f"Dimension of the index after deserialization: {index2.getDim()}")
    print(f"Number of database entries after deserialization: {index2.getNTotal()}")
```

### getNTotal

**API Definition <a name="section172317194488"></a>**

def getNTotal\(\) -\> int

**API Function<a name="section1153124784912"></a>**

Returns the total number of data entries in the database within the graph index.

**Parameter Description <a name="section1521117111210"></a>**

None

**Return Value<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>
<table><thead align="left"><tr id="row1569152711463"><th class="cellrowborder" valign="top" width="36.96%" id="mcps1.1.3.1.1"><p id="p146911527174618"><a name="p146911527174618"></a><a name="p146911527174618"></a>Data Type </p>
</th>
<th class="cellrowborder" valign="top" width="63.04%" id="mcps1.1.3.1.2"><p id="p136911627194618"><a name="p136911627194618"></a><a name="p136911627194618"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row769192744612"><td class="cellrowborder" valign="top" width="36.96%" headers="mcps1.1.3.1.1 "><p id="p106910272463"><a name="p106910272463"></a><a name="p106910272463"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="63.04%" headers="mcps1.1.3.1.2 "><p id="p19997736105"><a name="p19997736105"></a><a name="p19997736105"></a>If no database is added,<code>0</code> is returned by default.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```python
import numpy as np
import kbest

dim = 128
nb = 10000

index = kbest.KBest(dim, 32, 200, 60, 2, "L2", "RNNDescent", "HNSW", False, 1)

# Before adding data
print(f"Number of data entries in the database before adding data: {index.getNTotal()}")

# Add data
xb = np.random.random((nb, dim)).astype(np.float32)
index.add(nb, xb, 16, 1, 0)

# // After adding data
print(f"Number of data entries in the database after adding data: {index.getNTotal()}")
```

### getDim

**API Definition <a name="section172317194488"></a>**

def getDim\(\) -\> int

**API Function<a name="section1153124784912"></a>**

Returns the data dimension in the current graph index.

**Parameter Description <a name="section1521117111210"></a>**

None

**Return Value<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>
<table><thead align="left"><tr id="row1569152711463"><th class="cellrowborder" valign="top" width="36.96%" id="mcps1.1.3.1.1"><p id="p146911527174618"><a name="p146911527174618"></a><a name="p146911527174618"></a>Data Type </p>
</th>
<th class="cellrowborder" valign="top" width="63.04%" id="mcps1.1.3.1.2"><p id="p136911627194618"><a name="p136911627194618"></a><a name="p136911627194618"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row769192744612"><td class="cellrowborder" valign="top" width="36.96%" headers="mcps1.1.3.1.1 "><p id="p106910272463"><a name="p106910272463"></a><a name="p106910272463"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="63.04%" headers="mcps1.1.3.1.2 "><p id="p19997736105"><a name="p19997736105"></a><a name="p19997736105"></a>If an index is created using a parameterized constructor, the value is the same as that of <span class="parmname" id="parmname8531896718"><a name="parmname8531896718"></a><a name="parmname8531896718"></a><code>dim</code></span>. If an index is created using a default constructor or if an index created with a parameterized constructor is later re-initialized by calling load/deserialize/loadGraph, the return value is the dimension of data read from the searcher or the graph index.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```python
import kbest

dim = 128

# Create with parameterized constructor
index1 = kbest.KBest(dim, 32, 200, 60, 2, "L2", "RNNDescent", "HNSW", False, 1)
print(f"Dimension after parameterized construction: {index1.getDim()}")

# Create with default constructor, then load from file
index2 = kbest.KBest()
index2.load("./kbest_index.bin")
print(f"Dimension after loading from file: {index2.getDim()}")
```

### setEarlyStoppingParams

**API Definition <a name="section172317194488"></a>**

def setEarlyStoppingParams\(adding\_pref: int, patience: int\) -\> int

**API Function<a name="section1153124784912"></a>**

Sets the parameters for early stopping optimization.

**Parameter Description <a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="13.44%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="18.360000000000003%" id="mcps1.1.5.1.2"><p id="p654931862217"><a name="p654931862217"></a><a name="p654931862217"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="21.64%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="46.56%" id="mcps1.1.5.1.4"><p id="p1440932116441"><a name="p1440932116441"></a><a name="p1440932116441"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="13.44%" headers="mcps1.1.5.1.1 "><p id="p184071120102610"><a name="p184071120102610"></a><a name="p184071120102610"></a>adding_pref</p>
</td>
<td class="cellrowborder" valign="top" width="18.360000000000003%" headers="mcps1.1.5.1.2 "><p id="p2054931812228"><a name="p2054931812228"></a><a name="p2054931812228"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="21.64%" headers="mcps1.1.5.1.3 "><p id="p0407020102611"><a name="p0407020102611"></a><a name="p0407020102611"></a>Threshold for inserting the hyperparameter candidate set</p>
</td>
<td class="cellrowborder" valign="top" width="46.56%" headers="mcps1.1.5.1.4 "><p id="p20167131514510"><a name="p20167131514510"></a><a name="p20167131514510"></a>The value must be greater than or equal to 1.</p>
</td>
</tr>
<tr id="row188955417267"><td class="cellrowborder" valign="top" width="13.44%" headers="mcps1.1.5.1.1 "><p id="p37102045152610"><a name="p37102045152610"></a><a name="p37102045152610"></a>patience</p>
</td>
<td class="cellrowborder" valign="top" width="18.360000000000003%" headers="mcps1.1.5.1.2 "><p id="p1089574110268"><a name="p1089574110268"></a><a name="p1089574110268"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="21.64%" headers="mcps1.1.5.1.3 "><p id="p117109457269"><a name="p117109457269"></a><a name="p117109457269"></a>Search patience value</p>
</td>
<td class="cellrowborder" valign="top" width="46.56%" headers="mcps1.1.5.1.4 "><p id="p789514142616"><a name="p789514142616"></a><a name="p789514142616"></a>The value must be greater than or equal to 1.</p>
</td>
</tr>
</tbody>
</table>

**Return Value<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>
<table><thead align="left"><tr id="row1569152711463"><th class="cellrowborder" valign="top" width="36.96%" id="mcps1.1.3.1.1"><p id="p146911527174618"><a name="p146911527174618"></a><a name="p146911527174618"></a>Data Type </p>
</th>
<th class="cellrowborder" valign="top" width="63.04%" id="mcps1.1.3.1.2"><p id="p136911627194618"><a name="p136911627194618"></a><a name="p136911627194618"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row769192744612"><td class="cellrowborder" valign="top" width="36.96%" headers="mcps1.1.3.1.1 "><p id="p106910272463"><a name="p106910272463"></a><a name="p106910272463"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="63.04%" headers="mcps1.1.3.1.2 "><p id="p19997736105"><a name="p19997736105"></a><a name="p19997736105"></a>This API is a wrapper for an underlying C++ API, which controls exception handling.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```python
import numpy as np
import kbest

dim = 128
nb = 10000

index = kbest.KBest(dim, 32, 200, 60, 2, "L2", "RNNDescent", "HNSW", False, 1)

xb = np.random.random((nb, dim)).astype(np.float32)
index.add(nb, xb, 16, 1, 0)

# Set the parameters for early stopping (call this API before buildSearcher).
adding_pref = 5   # Threshold for inserting the hyperparameter candidate set
patience = 10     # Search patience value

ret = index.setEarlyStoppingParams(adding_pref, patience)

if ret == 0:
    print ("Parameters for early stopping successfully set")

# // Then, build a searcher.
index.buildSearcher()
```
