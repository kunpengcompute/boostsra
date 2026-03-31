# API参考

## Python接口

### 接口说明

KScaNN不提供对外接口，基于开源ScaNN算法做侵入式修改，对开源接口有新增。为获得最优性能，KScaNN接口内部不做完整入参校验，入参合法性由调用方业务来保证。KScaNN侵入式修改后的ScaNN所提供的Python接口如[**表 1** KScaNN修改后的Python接口](#KScaNN修改后的Python接口)所示。

**表 1** KScaNN修改后的Python接口<a id="KScaNN修改后的Python接口"></a>

<a name="table1194910128449"></a>
<table><thead align="left"><tr id="row99491812134412"><th class="cellrowborder" valign="top" width="31.269999999999996%" id="mcps1.2.3.1.1"><p id="p1794951224415"><a name="p1794951224415"></a><a name="p1794951224415"></a>接口名称</p>
</th>
<th class="cellrowborder" valign="top" width="68.73%" id="mcps1.2.3.1.2"><p id="p6949612124415"><a name="p6949612124415"></a><a name="p6949612124415"></a>接口作用</p>
</th>
</tr>
</thead>
<tbody><tr id="row712018285575"><td class="cellrowborder" valign="top" width="31.269999999999996%" headers="mcps1.2.3.1.1 "><p id="p12121102835714"><a name="p12121102835714"></a><a name="p12121102835714"></a>set_num_threads</p>
</td>
<td class="cellrowborder" valign="top" width="68.73%" headers="mcps1.2.3.1.2 "><p id="p111217289571"><a name="p111217289571"></a><a name="p111217289571"></a>配置搜索时启用线程数（相比开源算法新增的接口）。</p>
</td>
</tr>
<tr id="row119491112174414"><td class="cellrowborder" valign="top" width="31.269999999999996%" headers="mcps1.2.3.1.1 "><p id="p539219519167"><a name="p539219519167"></a><a name="p539219519167"></a>search_additional_params</p>
</td>
<td class="cellrowborder" valign="top" width="68.73%" headers="mcps1.2.3.1.2 "><p id="p3949012174411"><a name="p3949012174411"></a><a name="p3949012174411"></a>用于扩展ScaNN检索功能，提供额外的检索参数配置接口（相比开源算法新增的接口）。</p>
</td>
</tr>
<tr id="row9949131219443"><td class="cellrowborder" valign="top" width="31.269999999999996%" headers="mcps1.2.3.1.1 "><p id="p1094921294415"><a name="p1094921294415"></a><a name="p1094921294415"></a>search</p>
</td>
<td class="cellrowborder" valign="top" width="68.73%" headers="mcps1.2.3.1.2 "><p id="p1794941284418"><a name="p1794941284418"></a><a name="p1794941284418"></a>单query搜索接口，单线程执行（与开源算法保持一致）。</p>
</td>
</tr>
<tr id="row1594913120443"><td class="cellrowborder" valign="top" width="31.269999999999996%" headers="mcps1.2.3.1.1 "><p id="p4949012144417"><a name="p4949012144417"></a><a name="p4949012144417"></a>search_batched</p>
</td>
<td class="cellrowborder" valign="top" width="68.73%" headers="mcps1.2.3.1.2 "><p id="p1509193871710"><a name="p1509193871710"></a><a name="p1509193871710"></a>批量query搜索接口，单线程执行（与开源算法保持一致）。</p>
</td>
</tr>
<tr id="row6949131274416"><td class="cellrowborder" valign="top" width="31.269999999999996%" headers="mcps1.2.3.1.1 "><p id="p18867143114163"><a name="p18867143114163"></a><a name="p18867143114163"></a>search_batched_parallel</p>
</td>
<td class="cellrowborder" valign="top" width="68.73%" headers="mcps1.2.3.1.2 "><p id="p794971214414"><a name="p794971214414"></a><a name="p794971214414"></a>并行批量query搜索接口，多线程并发执行（与开源算法保持一致）。</p>
</td>
</tr>
<tr id="row694916124445"><td class="cellrowborder" valign="top" width="31.269999999999996%" headers="mcps1.2.3.1.1 "><p id="p136701839191615"><a name="p136701839191615"></a><a name="p136701839191615"></a>builder</p>
</td>
<td class="cellrowborder" valign="top" width="68.73%" headers="mcps1.2.3.1.2 "><p id="p894941210443"><a name="p894941210443"></a><a name="p894941210443"></a>用于开始构建（与开源算法保持一致）。</p>
</td>
</tr>
<tr id="row159491712174414"><td class="cellrowborder" valign="top" width="31.269999999999996%" headers="mcps1.2.3.1.1 "><p id="p10497124591619"><a name="p10497124591619"></a><a name="p10497124591619"></a>tree</p>
</td>
<td class="cellrowborder" valign="top" width="68.73%" headers="mcps1.2.3.1.2 "><p id="p2094917128448"><a name="p2094917128448"></a><a name="p2094917128448"></a>添加IVF分区的相关参数（与开源算法保持一致）。</p>
</td>
</tr>
<tr id="row198655487161"><td class="cellrowborder" valign="top" width="31.269999999999996%" headers="mcps1.2.3.1.1 "><p id="p11866448181619"><a name="p11866448181619"></a><a name="p11866448181619"></a>score_ah</p>
</td>
<td class="cellrowborder" valign="top" width="68.73%" headers="mcps1.2.3.1.2 "><p id="p786624801615"><a name="p786624801615"></a><a name="p786624801615"></a>添加PQ分区量化的相关参数（与开源算法保持一致）。</p>
</td>
</tr>
<tr id="row132215567163"><td class="cellrowborder" valign="top" width="31.269999999999996%" headers="mcps1.2.3.1.1 "><p id="p102211256151619"><a name="p102211256151619"></a><a name="p102211256151619"></a>reorder</p>
</td>
<td class="cellrowborder" valign="top" width="68.73%" headers="mcps1.2.3.1.2 "><p id="p18221256191618"><a name="p18221256191618"></a><a name="p18221256191618"></a>添加重排的相关参数（与开源算法保持一致）。</p>
</td>
</tr>
<tr id="row12818101418175"><td class="cellrowborder" valign="top" width="31.269999999999996%" headers="mcps1.2.3.1.1 "><p id="p9818141401711"><a name="p9818141401711"></a><a name="p9818141401711"></a>build</p>
</td>
<td class="cellrowborder" valign="top" width="68.73%" headers="mcps1.2.3.1.2 "><p id="p1818181431719"><a name="p1818181431719"></a><a name="p1818181431719"></a>用于构建索引（与开源算法保持一致）。</p>
</td>
</tr>
<tr id="row161581825204919"><td class="cellrowborder" valign="top" width="31.269999999999996%" headers="mcps1.2.3.1.1 "><p id="p11583253490"><a name="p11583253490"></a><a name="p11583253490"></a>serialize_to_mem</p>
</td>
<td class="cellrowborder" valign="top" width="68.73%" headers="mcps1.2.3.1.2 "><p id="p2158152518494"><a name="p2158152518494"></a><a name="p2158152518494"></a>将构建好的索引储存在数组中（相比开源算法新增的接口）。</p>
</td>
</tr>
<tr id="row87102818496"><td class="cellrowborder" valign="top" width="31.269999999999996%" headers="mcps1.2.3.1.1 "><p id="p5742804920"><a name="p5742804920"></a><a name="p5742804920"></a>deserialize_from_mem</p>
</td>
<td class="cellrowborder" valign="top" width="68.73%" headers="mcps1.2.3.1.2 "><p id="p17182874918"><a name="p17182874918"></a><a name="p17182874918"></a>给定存储序列化内容的数组，还原一个检索器的索引实例（相比开源算法新增的接口）。</p>
</td>
</tr>
<tr id="row161931542165614"><td class="cellrowborder" valign="top" width="31.269999999999996%" headers="mcps1.2.3.1.1 "><p id="p1193124211561"><a name="p1193124211561"></a><a name="p1193124211561"></a>get_num</p>
</td>
<td class="cellrowborder" valign="top" width="68.73%" headers="mcps1.2.3.1.2 "><p id="p61942042175616"><a name="p61942042175616"></a><a name="p61942042175616"></a>获取底库向量的数量（相比开源算法新增的接口）。</p>
</td>
</tr>
<tr id="row10100646175616"><td class="cellrowborder" valign="top" width="31.269999999999996%" headers="mcps1.2.3.1.1 "><p id="p2100154614561"><a name="p2100154614561"></a><a name="p2100154614561"></a>get_dim</p>
</td>
<td class="cellrowborder" valign="top" width="68.73%" headers="mcps1.2.3.1.2 "><p id="p15857202015577"><a name="p15857202015577"></a><a name="p15857202015577"></a>获取底库向量的维度（相比开源算法新增的接口）。</p>
</td>
</tr>
<tr id="row1925171313144"><td class="cellrowborder" valign="top" width="31.269999999999996%" headers="mcps1.2.3.1.1 "><p id="p7251113131417"><a name="p7251113131417"></a><a name="p7251113131417"></a>create_searcher</p>
</td>
<td class="cellrowborder" valign="top" width="68.73%" headers="mcps1.2.3.1.2 "><p id="p13431163771418"><a name="p13431163771418"></a><a name="p13431163771418"></a><span>基于入参构建索引并返回</span><span>ScannSearcher</span><span>（与开源算法相比增加</span>filter_thr和filter_type参数<span>）。</span></p>
</td>
</tr>
</tbody>
</table>

### set\_num\_threads

**接口定义<a name="section172317194488"></a>**

def set\_num\_threads\(num\_threads: int\) -\> None

**接口用途<a name="section1153124784912"></a>**

配置搜索时启用线程数（相比开源算法新增的接口）。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.4%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.26%" id="mcps1.1.5.1.2"><p id="p1844420713238"><a name="p1844420713238"></a><a name="p1844420713238"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="27.339999999999996%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="40%" id="mcps1.1.5.1.4"><p id="p232514861412"><a name="p232514861412"></a><a name="p232514861412"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.4%" headers="mcps1.1.5.1.1 "><p id="p455534613591"><a name="p455534613591"></a><a name="p455534613591"></a>num_threads</p>
</td>
<td class="cellrowborder" valign="top" width="17.26%" headers="mcps1.1.5.1.2 "><p id="p6444187172318"><a name="p6444187172318"></a><a name="p6444187172318"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="27.339999999999996%" headers="mcps1.1.5.1.3 "><p id="p16387135416598"><a name="p16387135416598"></a><a name="p16387135416598"></a>线程数量。</p>
</td>
<td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.5.1.4 "><p id="p1032519801411"><a name="p1032519801411"></a><a name="p1032519801411"></a>大于等于2，推荐配置为运行时CPU核数。</p>
</td>
</tr>
</tbody>
</table>

### search\_additional\_param

**接口定义<a name="section172317194488"></a>**

def search\_additional\_params \(adp\_threshold: float, refine\_prm: float, adp\_refined: int, leaves\_to\_search: int\) -\> bool

**接口用途<a name="section1153124784912"></a>**

用于扩展ScaNN检索功能，提供额外的检索参数配置接口（相比开源算法新增的接口）。应在索引构建后、检索前调用设置，接口参数具备缓存功能，一次设置，后续检索均生效。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="20.092009200920092%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.421442144214422%" id="mcps1.1.5.1.2"><p id="p73401941182314"><a name="p73401941182314"></a><a name="p73401941182314"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="34.98349834983499%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="30.503050305030506%" id="mcps1.1.5.1.4"><p id="p232514861412"><a name="p232514861412"></a><a name="p232514861412"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="20.092009200920092%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>adp_threshold</p>
</td>
<td class="cellrowborder" valign="top" width="14.421442144214422%" headers="mcps1.1.5.1.2 "><p id="p634084116239"><a name="p634084116239"></a><a name="p634084116239"></a>float</p>
</td>
<td class="cellrowborder" valign="top" width="34.98349834983499%" headers="mcps1.1.5.1.3 "><p id="p1551821410413"><a name="p1551821410413"></a><a name="p1551821410413"></a>决策阈值，典型值0.3。</p>
</td>
<td class="cellrowborder" valign="top" width="30.503050305030506%" headers="mcps1.1.5.1.4 "><p id="p2223102401510"><a name="p2223102401510"></a><a name="p2223102401510"></a>[0.1, 0.8]</p>
</td>
</tr>
<tr id="row52641156716"><td class="cellrowborder" valign="top" width="20.092009200920092%" headers="mcps1.1.5.1.1 "><p id="p1826581511711"><a name="p1826581511711"></a><a name="p1826581511711"></a>refine_prm</p>
</td>
<td class="cellrowborder" valign="top" width="14.421442144214422%" headers="mcps1.1.5.1.2 "><p id="p326515151774"><a name="p326515151774"></a><a name="p326515151774"></a>float</p>
</td>
<td class="cellrowborder" valign="top" width="34.98349834983499%" headers="mcps1.1.5.1.3 "><p id="p122656151672"><a name="p122656151672"></a><a name="p122656151672"></a>精细化控制过滤策略，典型值0.2，值越大则过滤的子空间个数越少，精度越高，但性能会下降。</p>
</td>
<td class="cellrowborder" valign="top" width="30.503050305030506%" headers="mcps1.1.5.1.4 "><p id="p32655151974"><a name="p32655151974"></a><a name="p32655151974"></a>[0.0, 1.0]，默认为0.0。</p>
</td>
</tr>
<tr id="row11230173385019"><td class="cellrowborder" valign="top" width="20.092009200920092%" headers="mcps1.1.5.1.1 "><p id="p6412202812239"><a name="p6412202812239"></a><a name="p6412202812239"></a>adp_refined</p>
</td>
<td class="cellrowborder" valign="top" width="14.421442144214422%" headers="mcps1.1.5.1.2 "><p id="p153407416237"><a name="p153407416237"></a><a name="p153407416237"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="34.98349834983499%" headers="mcps1.1.5.1.3 "><p id="p27308382419"><a name="p27308382419"></a><a name="p27308382419"></a>简单query所采用的子空间个数，典型值0，为训练自适应值（75分位点）。</p>
</td>
<td class="cellrowborder" valign="top" width="30.503050305030506%" headers="mcps1.1.5.1.4 "><p id="p9223152491519"><a name="p9223152491519"></a><a name="p9223152491519"></a>[0, leaves_to_search]，其中<span class="parmname" id="parmname2089000161016"><a name="parmname2089000161016"></a><a name="parmname2089000161016"></a>“leaves_to_search”</span>表示复杂query所采用的子空间个数。</p>
</td>
</tr>
<tr id="row92309336505"><td class="cellrowborder" valign="top" width="20.092009200920092%" headers="mcps1.1.5.1.1 "><p id="p162309336505"><a name="p162309336505"></a><a name="p162309336505"></a>leaves_to_search</p>
</td>
<td class="cellrowborder" valign="top" width="14.421442144214422%" headers="mcps1.1.5.1.2 "><p id="p14340141122314"><a name="p14340141122314"></a><a name="p14340141122314"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="34.98349834983499%" headers="mcps1.1.5.1.3 "><p id="p764411521247"><a name="p764411521247"></a><a name="p764411521247"></a>复杂query所采用的子空间个数，应与实际检索（search*）接口参数一致。</p>
</td>
<td class="cellrowborder" valign="top" width="30.503050305030506%" headers="mcps1.1.5.1.4 "><p id="p19223324111511"><a name="p19223324111511"></a><a name="p19223324111511"></a>[1, num_leaves]，其中<span class="parmname" id="parmname1935718105112"><a name="parmname1935718105112"></a><a name="parmname1935718105112"></a>“num_leaves”</span>表示IVF（Inverted File）倒排索引分区总子空间个数。</p>
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
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>bool</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p19997736105"><a name="p19997736105"></a><a name="p19997736105"></a>算法库加载成功，根据设置功能激活时返回True；否则返回False。</p>
</td>
</tr>
</tbody>
</table>

### search

**接口定义<a name="section172317194488"></a>**

def search\(q: numpy.ndarray, final\_num\_neighbors: int, pre\_reorder\_num\_neighbors: int, leaves\_to\_search: int\) -\> tuple\(idx, dist\)

**接口用途<a name="section1153124784912"></a>**

单query搜索接口，单线程执行（与开源算法保持一致）。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="17.68%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="15.709999999999999%" id="mcps1.1.5.1.2"><p id="p11820174522415"><a name="p11820174522415"></a><a name="p11820174522415"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="23.169999999999998%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="43.44%" id="mcps1.1.5.1.4"><p id="p9491844171618"><a name="p9491844171618"></a><a name="p9491844171618"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="17.68%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>q</p>
</td>
<td class="cellrowborder" valign="top" width="15.709999999999999%" headers="mcps1.1.5.1.2 "><p id="p4820154513242"><a name="p4820154513242"></a><a name="p4820154513242"></a>numpy.ndarray</p>
</td>
<td class="cellrowborder" valign="top" width="23.169999999999998%" headers="mcps1.1.5.1.3 "><p id="p182303331508"><a name="p182303331508"></a><a name="p182303331508"></a>Query。</p>
</td>
<td class="cellrowborder" valign="top" width="43.44%" headers="mcps1.1.5.1.4 "><p id="p949124418164"><a name="p949124418164"></a><a name="p949124418164"></a>限制非空。</p>
</td>
</tr>
<tr id="row11230173385019"><td class="cellrowborder" valign="top" width="17.68%" headers="mcps1.1.5.1.1 "><p id="p6412202812239"><a name="p6412202812239"></a><a name="p6412202812239"></a>final_num_neighbors</p>
</td>
<td class="cellrowborder" valign="top" width="15.709999999999999%" headers="mcps1.1.5.1.2 "><p id="p1682011454245"><a name="p1682011454245"></a><a name="p1682011454245"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="23.169999999999998%" headers="mcps1.1.5.1.3 "><p id="p10230433115013"><a name="p10230433115013"></a><a name="p10230433115013"></a>最终返回结果数量，TopK。</p>
</td>
<td class="cellrowborder" valign="top" width="43.44%" headers="mcps1.1.5.1.4 "><p id="p195481334151716"><a name="p195481334151716"></a><a name="p195481334151716"></a>大于等于1。</p>
</td>
</tr>
<tr id="row92309336505"><td class="cellrowborder" valign="top" width="17.68%" headers="mcps1.1.5.1.1 "><p id="p64119117270"><a name="p64119117270"></a><a name="p64119117270"></a>pre_reorder_num_neighbors</p>
</td>
<td class="cellrowborder" valign="top" width="15.709999999999999%" headers="mcps1.1.5.1.2 "><p id="p17820745122418"><a name="p17820745122418"></a><a name="p17820745122418"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="23.169999999999998%" headers="mcps1.1.5.1.3 "><p id="p92301933165017"><a name="p92301933165017"></a><a name="p92301933165017"></a>重排前保存结果数量。</p>
</td>
<td class="cellrowborder" valign="top" width="43.44%" headers="mcps1.1.5.1.4 "><p id="p849114441619"><a name="p849114441619"></a><a name="p849114441619"></a>大于等于final_num_neighbors，其中<span class="parmname" id="parmname16137152615912"><a name="parmname16137152615912"></a><a name="parmname16137152615912"></a>“final_num_neighbors”</span>为最终返回结果数量。</p>
</td>
</tr>
<tr id="row1678511193277"><td class="cellrowborder" valign="top" width="17.68%" headers="mcps1.1.5.1.1 "><p id="p778515193277"><a name="p778515193277"></a><a name="p778515193277"></a>leaves_to_search</p>
</td>
<td class="cellrowborder" valign="top" width="15.709999999999999%" headers="mcps1.1.5.1.2 "><p id="p782054510242"><a name="p782054510242"></a><a name="p782054510242"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="23.169999999999998%" headers="mcps1.1.5.1.3 "><p id="p1678617193274"><a name="p1678617193274"></a><a name="p1678617193274"></a>搜索子空间数量。</p>
</td>
<td class="cellrowborder" valign="top" width="43.44%" headers="mcps1.1.5.1.4 "><p id="p54914451617"><a name="p54914451617"></a><a name="p54914451617"></a>[1, num_leaves]，其中<span class="parmname" id="parmname13412142641214"><a name="parmname13412142641214"></a><a name="parmname13412142641214"></a>“num_leaves”</span>为IVF倒排索引分区总子空间个数。</p>
</td>
</tr>
</tbody>
</table>

**返回值<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="24.41%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="75.59%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="24.41%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>tuple(idx, dist)</p>
</td>
<td class="cellrowborder" valign="top" width="75.59%" headers="mcps1.1.3.1.2 "><p id="p16069535361"><a name="p16069535361"></a><a name="p16069535361"></a>idx为包含final_num_neighbors个底库ID的numpy.ndarray；dist为包含final_num_neighbors个距离的numpy.ndarray。</p>
</td>
</tr>
</tbody>
</table>

### search\_batched

**接口定义<a name="section172317194488"></a>**

def search\_batched\(queries: numpy.ndarray, final\_num\_neighbors: int, pre\_reorder\_num\_neighbors: int, leaves\_to\_search: int\) -\> tuple\(idx, dist\)

**接口用途<a name="section1153124784912"></a>**

批量query搜索接口，单线程执行（与开源算法保持一致）。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="19.78%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="15.15%" id="mcps1.1.5.1.2"><p id="p34582118269"><a name="p34582118269"></a><a name="p34582118269"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="29.189999999999998%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="35.88%" id="mcps1.1.5.1.4"><p id="p0143133471810"><a name="p0143133471810"></a><a name="p0143133471810"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>queries</p>
</td>
<td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.1.5.1.2 "><p id="p1445831162619"><a name="p1445831162619"></a><a name="p1445831162619"></a>numpy.ndarray</p>
</td>
<td class="cellrowborder" valign="top" width="29.189999999999998%" headers="mcps1.1.5.1.3 "><p id="p182303331508"><a name="p182303331508"></a><a name="p182303331508"></a>批次内的Queries。</p>
</td>
<td class="cellrowborder" valign="top" width="35.88%" headers="mcps1.1.5.1.4 "><p id="p17143113431814"><a name="p17143113431814"></a><a name="p17143113431814"></a>限制非空。</p>
</td>
</tr>
<tr id="row11230173385019"><td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.1 "><p id="p6412202812239"><a name="p6412202812239"></a><a name="p6412202812239"></a>final_num_neighbors</p>
</td>
<td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.1.5.1.2 "><p id="p645841162611"><a name="p645841162611"></a><a name="p645841162611"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="29.189999999999998%" headers="mcps1.1.5.1.3 "><p id="p10230433115013"><a name="p10230433115013"></a><a name="p10230433115013"></a>最终返回结果数量。</p>
</td>
<td class="cellrowborder" valign="top" width="35.88%" headers="mcps1.1.5.1.4 "><p id="p195481334151716"><a name="p195481334151716"></a><a name="p195481334151716"></a>大于等于1。</p>
</td>
</tr>
<tr id="row92309336505"><td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.1 "><p id="p64119117270"><a name="p64119117270"></a><a name="p64119117270"></a>pre_reorder_num_neighbors</p>
</td>
<td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.1.5.1.2 "><p id="p114581111263"><a name="p114581111263"></a><a name="p114581111263"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="29.189999999999998%" headers="mcps1.1.5.1.3 "><p id="p92301933165017"><a name="p92301933165017"></a><a name="p92301933165017"></a>重排前保存结果数量。</p>
</td>
<td class="cellrowborder" valign="top" width="35.88%" headers="mcps1.1.5.1.4 "><p id="p849114441619"><a name="p849114441619"></a><a name="p849114441619"></a>大于等于final_num_neighbors，其中<span class="parmname" id="parmname16137152615912"><a name="parmname16137152615912"></a><a name="parmname16137152615912"></a>“final_num_neighbors”</span>为最终返回结果数量。</p>
</td>
</tr>
<tr id="row1678511193277"><td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.1 "><p id="p778515193277"><a name="p778515193277"></a><a name="p778515193277"></a>leaves_to_search</p>
</td>
<td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.1.5.1.2 "><p id="p1045821111269"><a name="p1045821111269"></a><a name="p1045821111269"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="29.189999999999998%" headers="mcps1.1.5.1.3 "><p id="p1678617193274"><a name="p1678617193274"></a><a name="p1678617193274"></a>搜索子空间数量。</p>
</td>
<td class="cellrowborder" valign="top" width="35.88%" headers="mcps1.1.5.1.4 "><p id="p5143143471815"><a name="p5143143471815"></a><a name="p5143143471815"></a>[1, num_leaves]，其中<span class="parmname" id="parmname13412142641214"><a name="parmname13412142641214"></a><a name="parmname13412142641214"></a>“num_leaves”</span>为IVF倒排索引分区总子空间个数。</p>
</td>
</tr>
</tbody>
</table>

**返回值<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="28.01%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="71.99%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="28.01%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>tuple(idx, dist)</p>
</td>
<td class="cellrowborder" valign="top" width="71.99%" headers="mcps1.1.3.1.2 "><p id="p16069535361"><a name="p16069535361"></a><a name="p16069535361"></a>idx为包含final_num_neighbors个底库ID的numpy.ndarray；dist为包含final_num_neighbors个距离的numpy.ndarray。</p>
</td>
</tr>
</tbody>
</table>

### search\_batched\_parallel

**接口定义<a name="section172317194488"></a>**

def search\_batched\_parallel\(queries: numpy.ndarray, final\_num\_neighbors: int, pre\_reorder\_num\_neighbors:int, leaves\_to\_search: int, batch\_size: int\) -\> tuple\(idx, dist\)

**接口用途<a name="section1153124784912"></a>**

并行批量query搜索接口，多线程并发执行（与开源算法保持一致）。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="12.518748125187482%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="21.677832216778324%" id="mcps1.1.5.1.2"><p id="p12288121114294"><a name="p12288121114294"></a><a name="p12288121114294"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="31.226877312268776%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="34.57654234576542%" id="mcps1.1.5.1.4"><p id="p0143133471810"><a name="p0143133471810"></a><a name="p0143133471810"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="12.518748125187482%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>queries</p>
</td>
<td class="cellrowborder" valign="top" width="21.677832216778324%" headers="mcps1.1.5.1.2 "><p id="p152881611132912"><a name="p152881611132912"></a><a name="p152881611132912"></a>numpy.ndarray</p>
</td>
<td class="cellrowborder" valign="top" width="31.226877312268776%" headers="mcps1.1.5.1.3 "><p id="p182303331508"><a name="p182303331508"></a><a name="p182303331508"></a>批次内的Queries。</p>
</td>
<td class="cellrowborder" valign="top" width="34.57654234576542%" headers="mcps1.1.5.1.4 "><p id="p626316325199"><a name="p626316325199"></a><a name="p626316325199"></a>限制非空。</p>
</td>
</tr>
<tr id="row11230173385019"><td class="cellrowborder" valign="top" width="12.518748125187482%" headers="mcps1.1.5.1.1 "><p id="p6412202812239"><a name="p6412202812239"></a><a name="p6412202812239"></a>final_num_neighbors</p>
</td>
<td class="cellrowborder" valign="top" width="21.677832216778324%" headers="mcps1.1.5.1.2 "><p id="p82881511122913"><a name="p82881511122913"></a><a name="p82881511122913"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="31.226877312268776%" headers="mcps1.1.5.1.3 "><p id="p10230433115013"><a name="p10230433115013"></a><a name="p10230433115013"></a>最终返回结果数量，TopK。</p>
</td>
<td class="cellrowborder" valign="top" width="34.57654234576542%" headers="mcps1.1.5.1.4 "><p id="p195481334151716"><a name="p195481334151716"></a><a name="p195481334151716"></a>大于等于1。</p>
</td>
</tr>
<tr id="row92309336505"><td class="cellrowborder" valign="top" width="12.518748125187482%" headers="mcps1.1.5.1.1 "><p id="p64119117270"><a name="p64119117270"></a><a name="p64119117270"></a>pre_reorder_num_neighbors</p>
</td>
<td class="cellrowborder" valign="top" width="21.677832216778324%" headers="mcps1.1.5.1.2 "><p id="p1528813115295"><a name="p1528813115295"></a><a name="p1528813115295"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="31.226877312268776%" headers="mcps1.1.5.1.3 "><p id="p92301933165017"><a name="p92301933165017"></a><a name="p92301933165017"></a>重排前保存结果数量。</p>
</td>
<td class="cellrowborder" valign="top" width="34.57654234576542%" headers="mcps1.1.5.1.4 "><p id="p849114441619"><a name="p849114441619"></a><a name="p849114441619"></a>大于等于final_num_neighbors，其中<span class="parmname" id="parmname16137152615912"><a name="parmname16137152615912"></a><a name="parmname16137152615912"></a>“final_num_neighbors”</span>为最终返回结果数量。</p>
</td>
</tr>
<tr id="row1678511193277"><td class="cellrowborder" valign="top" width="12.518748125187482%" headers="mcps1.1.5.1.1 "><p id="p778515193277"><a name="p778515193277"></a><a name="p778515193277"></a>leaves_to_search</p>
</td>
<td class="cellrowborder" valign="top" width="21.677832216778324%" headers="mcps1.1.5.1.2 "><p id="p12288611182911"><a name="p12288611182911"></a><a name="p12288611182911"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="31.226877312268776%" headers="mcps1.1.5.1.3 "><p id="p1678617193274"><a name="p1678617193274"></a><a name="p1678617193274"></a>搜索子空间数量。</p>
</td>
<td class="cellrowborder" valign="top" width="34.57654234576542%" headers="mcps1.1.5.1.4 "><p id="p12639326192"><a name="p12639326192"></a><a name="p12639326192"></a>[1, num_leaves]，其中<span class="parmname" id="parmname13412142641214"><a name="parmname13412142641214"></a><a name="parmname13412142641214"></a>“num_leaves”</span>为IVF倒排索引分区总子空间个数。</p>
</td>
</tr>
<tr id="row9594162711328"><td class="cellrowborder" valign="top" width="12.518748125187482%" headers="mcps1.1.5.1.1 "><p id="p165941527193217"><a name="p165941527193217"></a><a name="p165941527193217"></a>batch_size</p>
</td>
<td class="cellrowborder" valign="top" width="21.677832216778324%" headers="mcps1.1.5.1.2 "><p id="p228812112299"><a name="p228812112299"></a><a name="p228812112299"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="31.226877312268776%" headers="mcps1.1.5.1.3 "><p id="p2594172733212"><a name="p2594172733212"></a><a name="p2594172733212"></a>并行自动分批时优先批次大小，默认值256。</p>
</td>
<td class="cellrowborder" valign="top" width="34.57654234576542%" headers="mcps1.1.5.1.4 "><p id="p13263153214194"><a name="p13263153214194"></a><a name="p13263153214194"></a>大于等于1。</p>
</td>
</tr>
</tbody>
</table>

**返回值<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="38.940000000000005%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="61.06%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="38.940000000000005%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>tuple(idx, dist)</p>
</td>
<td class="cellrowborder" valign="top" width="61.06%" headers="mcps1.1.3.1.2 "><p id="p16069535361"><a name="p16069535361"></a><a name="p16069535361"></a>idx为包含final_num_neighbors个底库ID的numpy.ndarray；dist为包含final_num_neighbors个距离的numpy.ndarray。</p>
</td>
</tr>
</tbody>
</table>

### builder

**接口定义<a name="section172317194488"></a>**

def builder\(db: numpy.ndarray, num\_neighbors: int, distance\_measure: string\) -\> scann.scann\_ops.py.scann\_builder.ScannBuilder

**接口用途<a name="section1153124784912"></a>**

用于开始构建（与开源算法保持一致）。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="17.43%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="16.79%" id="mcps1.1.5.1.2"><p id="p6962093011"><a name="p6962093011"></a><a name="p6962093011"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="31.490000000000002%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="34.29%" id="mcps1.1.5.1.4"><p id="p0143133471810"><a name="p0143133471810"></a><a name="p0143133471810"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="17.43%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>db</p>
</td>
<td class="cellrowborder" valign="top" width="16.79%" headers="mcps1.1.5.1.2 "><p id="p109617083019"><a name="p109617083019"></a><a name="p109617083019"></a>numpy.ndarray</p>
</td>
<td class="cellrowborder" valign="top" width="31.490000000000002%" headers="mcps1.1.5.1.3 "><p id="p182303331508"><a name="p182303331508"></a><a name="p182303331508"></a>底库向量。</p>
</td>
<td class="cellrowborder" valign="top" width="34.29%" headers="mcps1.1.5.1.4 "><p id="p1136510418203"><a name="p1136510418203"></a><a name="p1136510418203"></a>限制非空。</p>
</td>
</tr>
<tr id="row11230173385019"><td class="cellrowborder" valign="top" width="17.43%" headers="mcps1.1.5.1.1 "><p id="p6412202812239"><a name="p6412202812239"></a><a name="p6412202812239"></a>num_neighbors</p>
</td>
<td class="cellrowborder" valign="top" width="16.79%" headers="mcps1.1.5.1.2 "><p id="p096120173012"><a name="p096120173012"></a><a name="p096120173012"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="31.490000000000002%" headers="mcps1.1.5.1.3 "><p id="p10230433115013"><a name="p10230433115013"></a><a name="p10230433115013"></a>最终返回结果数量，TopK。</p>
</td>
<td class="cellrowborder" valign="top" width="34.29%" headers="mcps1.1.5.1.4 "><p id="p53652041152019"><a name="p53652041152019"></a><a name="p53652041152019"></a>大于等于1。</p>
</td>
</tr>
<tr id="row92309336505"><td class="cellrowborder" valign="top" width="17.43%" headers="mcps1.1.5.1.1 "><p id="p64119117270"><a name="p64119117270"></a><a name="p64119117270"></a>distance_measure</p>
</td>
<td class="cellrowborder" valign="top" width="16.79%" headers="mcps1.1.5.1.2 "><p id="p119615033014"><a name="p119615033014"></a><a name="p119615033014"></a>字符串</p>
</td>
<td class="cellrowborder" valign="top" width="31.490000000000002%" headers="mcps1.1.5.1.3 "><p id="p92301933165017"><a name="p92301933165017"></a><a name="p92301933165017"></a>距离度量的方式。</p>
</td>
<td class="cellrowborder" valign="top" width="34.29%" headers="mcps1.1.5.1.4 "><p id="p13651141162017"><a name="p13651141162017"></a><a name="p13651141162017"></a><span class="parmvalue" id="parmvalue045932133313"><a name="parmvalue045932133313"></a><a name="parmvalue045932133313"></a>“dot_product”</span>或<span class="parmvalue" id="parmvalue158238510333"><a name="parmvalue158238510333"></a><a name="parmvalue158238510333"></a>“squared_l2”</span></p>
</td>
</tr>
</tbody>
</table>

**返回值<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="38.940000000000005%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="61.06%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="38.940000000000005%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>scann.scann_ops.py.scann_builder.ScannBuilder</p>
</td>
<td class="cellrowborder" valign="top" width="61.06%" headers="mcps1.1.3.1.2 "><p id="p85639291550"><a name="p85639291550"></a><a name="p85639291550"></a>ScannBuilder类用于接收构建参数。</p>
</td>
</tr>
</tbody>
</table>

### tree

**接口定义<a name="section172317194488"></a>**

def tree\(num\_leaves: int, num\_leaves\_to\_search: int, training\_sample\_size: int, min\_partition\_size: int, training\_iterations: int, spherical: bool, quantize\_centroids: bool, random\_init: bool, soar\_lambda: float, overretrieve\_factor: float, distance\_measure: string\)  -\> scann.scann\_ops.py.scann\_builder.ScannBuilder

**接口用途<a name="section1153124784912"></a>**

添加IVF（Inverted File）倒排索引分区的相关参数（与开源算法保持一致）。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="19.61%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.510000000000002%" id="mcps1.1.5.1.2"><p id="p522410481308"><a name="p522410481308"></a><a name="p522410481308"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="32.43%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="33.45%" id="mcps1.1.5.1.4"><p id="p153921130102117"><a name="p153921130102117"></a><a name="p153921130102117"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="19.61%" headers="mcps1.1.5.1.1 "><p id="p1527511210396"><a name="p1527511210396"></a><a name="p1527511210396"></a>num_leaves</p>
</td>
<td class="cellrowborder" valign="top" width="14.510000000000002%" headers="mcps1.1.5.1.2 "><p id="p172241748123018"><a name="p172241748123018"></a><a name="p172241748123018"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="32.43%" headers="mcps1.1.5.1.3 "><p id="p182303331508"><a name="p182303331508"></a><a name="p182303331508"></a>IVF分区总子空间个数。</p>
</td>
<td class="cellrowborder" valign="top" width="33.45%" headers="mcps1.1.5.1.4 "><p id="p53921430162116"><a name="p53921430162116"></a><a name="p53921430162116"></a>大于等于1。</p>
</td>
</tr>
<tr id="row11230173385019"><td class="cellrowborder" valign="top" width="19.61%" headers="mcps1.1.5.1.1 "><p id="p17276181233915"><a name="p17276181233915"></a><a name="p17276181233915"></a>num_leaves_to_search</p>
</td>
<td class="cellrowborder" valign="top" width="14.510000000000002%" headers="mcps1.1.5.1.2 "><p id="p17224194819307"><a name="p17224194819307"></a><a name="p17224194819307"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="32.43%" headers="mcps1.1.5.1.3 "><p id="p10230433115013"><a name="p10230433115013"></a><a name="p10230433115013"></a>默认搜索子空间个数。</p>
</td>
<td class="cellrowborder" valign="top" width="33.45%" headers="mcps1.1.5.1.4 "><p id="p1839233042113"><a name="p1839233042113"></a><a name="p1839233042113"></a>[1, num_leaves]，其中<span class="parmname" id="parmname13412142641214"><a name="parmname13412142641214"></a><a name="parmname13412142641214"></a>“num_leaves”</span>为IVF倒排索引分区总子空间个数。</p>
</td>
</tr>
<tr id="row92309336505"><td class="cellrowborder" valign="top" width="19.61%" headers="mcps1.1.5.1.1 "><p id="p1527611223913"><a name="p1527611223913"></a><a name="p1527611223913"></a>training_sample_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.510000000000002%" headers="mcps1.1.5.1.2 "><p id="p152241348193015"><a name="p152241348193015"></a><a name="p152241348193015"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="32.43%" headers="mcps1.1.5.1.3 "><p id="p92301933165017"><a name="p92301933165017"></a><a name="p92301933165017"></a>分区训练时底库抽样个数。</p>
</td>
<td class="cellrowborder" valign="top" width="33.45%" headers="mcps1.1.5.1.4 "><p id="p339213012213"><a name="p339213012213"></a><a name="p339213012213"></a>[0, 底库数量]</p>
</td>
</tr>
<tr id="row1665453433815"><td class="cellrowborder" valign="top" width="19.61%" headers="mcps1.1.5.1.1 "><p id="p62764125398"><a name="p62764125398"></a><a name="p62764125398"></a>min_partition_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.510000000000002%" headers="mcps1.1.5.1.2 "><p id="p17224164813018"><a name="p17224164813018"></a><a name="p17224164813018"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="32.43%" headers="mcps1.1.5.1.3 "><p id="p16655113418383"><a name="p16655113418383"></a><a name="p16655113418383"></a>最小分区包含的底库向量个数。</p>
</td>
<td class="cellrowborder" valign="top" width="33.45%" headers="mcps1.1.5.1.4 "><p id="p153926305212"><a name="p153926305212"></a><a name="p153926305212"></a>[0, 底库数量]</p>
</td>
</tr>
<tr id="row1844813505387"><td class="cellrowborder" valign="top" width="19.61%" headers="mcps1.1.5.1.1 "><p id="p22768125390"><a name="p22768125390"></a><a name="p22768125390"></a>training_iterations</p>
</td>
<td class="cellrowborder" valign="top" width="14.510000000000002%" headers="mcps1.1.5.1.2 "><p id="p192248482303"><a name="p192248482303"></a><a name="p192248482303"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="32.43%" headers="mcps1.1.5.1.3 "><p id="p1568640154020"><a name="p1568640154020"></a><a name="p1568640154020"></a>训练循环次数。</p>
</td>
<td class="cellrowborder" valign="top" width="33.45%" headers="mcps1.1.5.1.4 "><p id="p173921830172119"><a name="p173921830172119"></a><a name="p173921830172119"></a>大于等于1。</p>
</td>
</tr>
<tr id="row1750537143820"><td class="cellrowborder" valign="top" width="19.61%" headers="mcps1.1.5.1.1 "><p id="p8276101211398"><a name="p8276101211398"></a><a name="p8276101211398"></a>spherical</p>
</td>
<td class="cellrowborder" valign="top" width="14.510000000000002%" headers="mcps1.1.5.1.2 "><p id="p6224174843018"><a name="p6224174843018"></a><a name="p6224174843018"></a>布尔值</p>
</td>
<td class="cellrowborder" valign="top" width="32.43%" headers="mcps1.1.5.1.3 "><p id="p186862006409"><a name="p186862006409"></a><a name="p186862006409"></a>分区类型是否为spherical。</p>
</td>
<td class="cellrowborder" valign="top" width="33.45%" headers="mcps1.1.5.1.4 "><p id="p8392143042112"><a name="p8392143042112"></a><a name="p8392143042112"></a>-</p>
</td>
</tr>
<tr id="row19598544183817"><td class="cellrowborder" valign="top" width="19.61%" headers="mcps1.1.5.1.1 "><p id="p13276141216397"><a name="p13276141216397"></a><a name="p13276141216397"></a>quantize_centroids</p>
</td>
<td class="cellrowborder" valign="top" width="14.510000000000002%" headers="mcps1.1.5.1.2 "><p id="p122584843013"><a name="p122584843013"></a><a name="p122584843013"></a>布尔值</p>
</td>
<td class="cellrowborder" valign="top" width="32.43%" headers="mcps1.1.5.1.3 "><p id="p66865034011"><a name="p66865034011"></a><a name="p66865034011"></a>是否量化桶中心。</p>
</td>
<td class="cellrowborder" valign="top" width="33.45%" headers="mcps1.1.5.1.4 "><p id="p1039293022110"><a name="p1039293022110"></a><a name="p1039293022110"></a>-</p>
</td>
</tr>
<tr id="row20741194710388"><td class="cellrowborder" valign="top" width="19.61%" headers="mcps1.1.5.1.1 "><p id="p22766124394"><a name="p22766124394"></a><a name="p22766124394"></a>random_init</p>
</td>
<td class="cellrowborder" valign="top" width="14.510000000000002%" headers="mcps1.1.5.1.2 "><p id="p22251548183013"><a name="p22251548183013"></a><a name="p22251548183013"></a>布尔值</p>
</td>
<td class="cellrowborder" valign="top" width="32.43%" headers="mcps1.1.5.1.3 "><p id="p206865010407"><a name="p206865010407"></a><a name="p206865010407"></a>训练时是否随机开始。</p>
</td>
<td class="cellrowborder" valign="top" width="33.45%" headers="mcps1.1.5.1.4 "><p id="p63921305214"><a name="p63921305214"></a><a name="p63921305214"></a>-</p>
</td>
</tr>
<tr id="row868535915594"><td class="cellrowborder" valign="top" width="19.61%" headers="mcps1.1.5.1.1 "><p id="p2138444707"><a name="p2138444707"></a><a name="p2138444707"></a>soar_lambda</p>
</td>
<td class="cellrowborder" valign="top" width="14.510000000000002%" headers="mcps1.1.5.1.2 "><p id="p1413812442018"><a name="p1413812442018"></a><a name="p1413812442018"></a>float</p>
</td>
<td class="cellrowborder" valign="top" width="32.43%" headers="mcps1.1.5.1.3 "><p id="p01381144803"><a name="p01381144803"></a><a name="p01381144803"></a>控制正交性的参数，仅对IP(dot_product)数据集生效。</p>
</td>
<td class="cellrowborder" valign="top" width="33.45%" headers="mcps1.1.5.1.4 "><p id="p113817441403"><a name="p113817441403"></a><a name="p113817441403"></a>大于0，当值为-1时表示不开启此参数。</p>
</td>
</tr>
<tr id="row1944719319012"><td class="cellrowborder" valign="top" width="19.61%" headers="mcps1.1.5.1.1 "><p id="p1538814496016"><a name="p1538814496016"></a><a name="p1538814496016"></a>overretrieve_factor</p>
</td>
<td class="cellrowborder" valign="top" width="14.510000000000002%" headers="mcps1.1.5.1.2 "><p id="p13388749306"><a name="p13388749306"></a><a name="p13388749306"></a>float</p>
</td>
<td class="cellrowborder" valign="top" width="32.43%" headers="mcps1.1.5.1.3 "><p id="p1338813492019"><a name="p1338813492019"></a><a name="p1338813492019"></a>指定过检索因子，与<span class="parmname" id="parmname1866619242116"><a name="parmname1866619242116"></a><a name="parmname1866619242116"></a>“soar_lambda”</span>一起使用，仅对IP(dot_product)数据集生效。</p>
</td>
<td class="cellrowborder" valign="top" width="33.45%" headers="mcps1.1.5.1.4 "><p id="p538819491606"><a name="p538819491606"></a><a name="p538819491606"></a>[1,2]，当值为-1时表示不开启此参数。</p>
</td>
</tr>
<tr id="row1435461002"><td class="cellrowborder" valign="top" width="19.61%" headers="mcps1.1.5.1.1 "><p id="p193885491408"><a name="p193885491408"></a><a name="p193885491408"></a>distance_measure</p>
</td>
<td class="cellrowborder" valign="top" width="14.510000000000002%" headers="mcps1.1.5.1.2 "><p id="p1538884918015"><a name="p1538884918015"></a><a name="p1538884918015"></a>字符串</p>
</td>
<td class="cellrowborder" valign="top" width="32.43%" headers="mcps1.1.5.1.3 "><p id="p238815491409"><a name="p238815491409"></a><a name="p238815491409"></a>向量的距离类型。</p>
</td>
<td class="cellrowborder" valign="top" width="33.45%" headers="mcps1.1.5.1.4 "><p id="p1638804911017"><a name="p1638804911017"></a><a name="p1638804911017"></a><span class="parmvalue" id="parmvalue17469332116"><a name="parmvalue17469332116"></a><a name="parmvalue17469332116"></a>“dot_product”</span>或<span class="parmvalue" id="parmvalue12906641919"><a name="parmvalue12906641919"></a><a name="parmvalue12906641919"></a>“squared_l2”</span></p>
</td>
</tr>
</tbody>
</table>

**返回值<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="38.940000000000005%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="61.06%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="38.940000000000005%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>scann.scann_ops.py.scann_builder.ScannBuilder</p>
</td>
<td class="cellrowborder" valign="top" width="61.06%" headers="mcps1.1.3.1.2 "><p id="p85639291550"><a name="p85639291550"></a><a name="p85639291550"></a>ScannBuilder类用于接收构建参数。</p>
</td>
</tr>
</tbody>
</table>

### score\_ah

**接口定义<a name="section172317194488"></a>**

def score\_ah\(dimensions\_per\_block: int, anisotropic\_quantization\_threshold: float, training\_sample\_size: int, min\_cluster\_size: int, hash\_type: string, training\_iterations: int\) -\> scann.scann\_ops.py.scann\_builder.ScannBuilder

**接口用途<a name="section1153124784912"></a>**

添加PQ分区量化的相关参数（与开源算法保持一致）。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="19.12%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="12.85%" id="mcps1.1.5.1.2"><p id="p241584416319"><a name="p241584416319"></a><a name="p241584416319"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="36.91%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="31.119999999999997%" id="mcps1.1.5.1.4"><p id="p1124319456225"><a name="p1124319456225"></a><a name="p1124319456225"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="19.12%" headers="mcps1.1.5.1.1 "><p id="p1455620136427"><a name="p1455620136427"></a><a name="p1455620136427"></a>dimensions_per_block</p>
</td>
<td class="cellrowborder" valign="top" width="12.85%" headers="mcps1.1.5.1.2 "><p id="p154151244153116"><a name="p154151244153116"></a><a name="p154151244153116"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="36.91%" headers="mcps1.1.5.1.3 "><p id="p1283214411428"><a name="p1283214411428"></a><a name="p1283214411428"></a>PQ量化合并维度数。</p>
</td>
<td class="cellrowborder" valign="top" width="31.119999999999997%" headers="mcps1.1.5.1.4 "><p id="p1324334517220"><a name="p1324334517220"></a><a name="p1324334517220"></a>[1, 数据维度]</p>
</td>
</tr>
<tr id="row11230173385019"><td class="cellrowborder" valign="top" width="19.12%" headers="mcps1.1.5.1.1 "><p id="p11556213164213"><a name="p11556213164213"></a><a name="p11556213164213"></a>anisotropic_quantization_threshold</p>
</td>
<td class="cellrowborder" valign="top" width="12.85%" headers="mcps1.1.5.1.2 "><p id="p16415194403114"><a name="p16415194403114"></a><a name="p16415194403114"></a>float</p>
</td>
<td class="cellrowborder" valign="top" width="36.91%" headers="mcps1.1.5.1.3 "><p id="p6832184114220"><a name="p6832184114220"></a><a name="p6832184114220"></a>不对称分桶参数，仅对L2(squared_l2)数据集生效。</p>
</td>
<td class="cellrowborder" valign="top" width="31.119999999999997%" headers="mcps1.1.5.1.4 "><p id="p52439456228"><a name="p52439456228"></a><a name="p52439456228"></a>[0, 1]</p>
</td>
</tr>
<tr id="row92309336505"><td class="cellrowborder" valign="top" width="19.12%" headers="mcps1.1.5.1.1 "><p id="p1555620130424"><a name="p1555620130424"></a><a name="p1555620130424"></a>training_sample_size</p>
</td>
<td class="cellrowborder" valign="top" width="12.85%" headers="mcps1.1.5.1.2 "><p id="p141519445317"><a name="p141519445317"></a><a name="p141519445317"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="36.91%" headers="mcps1.1.5.1.3 "><p id="p12832141194210"><a name="p12832141194210"></a><a name="p12832141194210"></a>PQ分区训练时底库抽样个数。</p>
</td>
<td class="cellrowborder" valign="top" width="31.119999999999997%" headers="mcps1.1.5.1.4 "><p id="p162435458225"><a name="p162435458225"></a><a name="p162435458225"></a>[0, 底库数量]</p>
</td>
</tr>
<tr id="row1665453433815"><td class="cellrowborder" valign="top" width="19.12%" headers="mcps1.1.5.1.1 "><p id="p14556131384212"><a name="p14556131384212"></a><a name="p14556131384212"></a>min_cluster_size</p>
</td>
<td class="cellrowborder" valign="top" width="12.85%" headers="mcps1.1.5.1.2 "><p id="p17415244123118"><a name="p17415244123118"></a><a name="p17415244123118"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="36.91%" headers="mcps1.1.5.1.3 "><p id="p1483284184214"><a name="p1483284184214"></a><a name="p1483284184214"></a>最小PQ分区包含的底库向量个数。</p>
</td>
<td class="cellrowborder" valign="top" width="31.119999999999997%" headers="mcps1.1.5.1.4 "><p id="p82433459223"><a name="p82433459223"></a><a name="p82433459223"></a>[0, 底库数量]</p>
</td>
</tr>
<tr id="row1844813505387"><td class="cellrowborder" valign="top" width="19.12%" headers="mcps1.1.5.1.1 "><p id="p20556201310421"><a name="p20556201310421"></a><a name="p20556201310421"></a>hash_type</p>
</td>
<td class="cellrowborder" valign="top" width="12.85%" headers="mcps1.1.5.1.2 "><p id="p1241584493117"><a name="p1241584493117"></a><a name="p1241584493117"></a>字符串</p>
</td>
<td class="cellrowborder" valign="top" width="36.91%" headers="mcps1.1.5.1.3 "><p id="p8832194111421"><a name="p8832194111421"></a><a name="p8832194111421"></a>PQ量化类型。</p>
</td>
<td class="cellrowborder" valign="top" width="31.119999999999997%" headers="mcps1.1.5.1.4 "><p id="p124319458228"><a name="p124319458228"></a><a name="p124319458228"></a><span class="parmvalue" id="parmvalue1213762710148"><a name="parmvalue1213762710148"></a><a name="parmvalue1213762710148"></a>“lut16”</span>或<span class="parmvalue" id="parmvalue136951731141410"><a name="parmvalue136951731141410"></a><a name="parmvalue136951731141410"></a>“lut256”</span>。</p>
</td>
</tr>
<tr id="row1750537143820"><td class="cellrowborder" valign="top" width="19.12%" headers="mcps1.1.5.1.1 "><p id="p155561713124216"><a name="p155561713124216"></a><a name="p155561713124216"></a>training_iterations</p>
</td>
<td class="cellrowborder" valign="top" width="12.85%" headers="mcps1.1.5.1.2 "><p id="p104153441311"><a name="p104153441311"></a><a name="p104153441311"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="36.91%" headers="mcps1.1.5.1.3 "><p id="p9832204110428"><a name="p9832204110428"></a><a name="p9832204110428"></a>训练循环次数。</p>
</td>
<td class="cellrowborder" valign="top" width="31.119999999999997%" headers="mcps1.1.5.1.4 "><p id="p4243154562214"><a name="p4243154562214"></a><a name="p4243154562214"></a>大于等于1。</p>
</td>
</tr>
</tbody>
</table>

**返回值<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="38.940000000000005%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="61.06%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="38.940000000000005%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>scann.scann_ops.py.scann_builder.ScannBuilder</p>
</td>
<td class="cellrowborder" valign="top" width="61.06%" headers="mcps1.1.3.1.2 "><p id="p85639291550"><a name="p85639291550"></a><a name="p85639291550"></a>ScannBuilder类用于接收构建参数。</p>
</td>
</tr>
</tbody>
</table>

### reorder

**接口定义<a name="section172317194488"></a>**

def reorder\(reordering\_num\_neighbors: int, quantize: bool\) -\> scann.scann\_ops.py.scann\_builder.ScannBuilder

**接口用途<a name="section1153124784912"></a>**

添加重排的相关参数（与开源算法保持一致）。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="24.41%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.71%" id="mcps1.1.5.1.2"><p id="p990293519329"><a name="p990293519329"></a><a name="p990293519329"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="25.36%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="32.519999999999996%" id="mcps1.1.5.1.4"><p id="p1124319456225"><a name="p1124319456225"></a><a name="p1124319456225"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="24.41%" headers="mcps1.1.5.1.1 "><p id="p1854091217440"><a name="p1854091217440"></a><a name="p1854091217440"></a>reordering_num_neighbors</p>
</td>
<td class="cellrowborder" valign="top" width="17.71%" headers="mcps1.1.5.1.2 "><p id="p1490283519323"><a name="p1490283519323"></a><a name="p1490283519323"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="25.36%" headers="mcps1.1.5.1.3 "><p id="p1283214411428"><a name="p1283214411428"></a><a name="p1283214411428"></a>进入重排的数量。</p>
</td>
<td class="cellrowborder" valign="top" width="32.519999999999996%" headers="mcps1.1.5.1.4 "><p id="p131761349142317"><a name="p131761349142317"></a><a name="p131761349142317"></a>[0, 底库数量]</p>
</td>
</tr>
<tr id="row11230173385019"><td class="cellrowborder" valign="top" width="24.41%" headers="mcps1.1.5.1.1 "><p id="p11556213164213"><a name="p11556213164213"></a><a name="p11556213164213"></a>quantize</p>
</td>
<td class="cellrowborder" valign="top" width="17.71%" headers="mcps1.1.5.1.2 "><p id="p99022035133216"><a name="p99022035133216"></a><a name="p99022035133216"></a>布尔值</p>
</td>
<td class="cellrowborder" valign="top" width="25.36%" headers="mcps1.1.5.1.3 "><p id="p6832184114220"><a name="p6832184114220"></a><a name="p6832184114220"></a>是否量化。</p>
</td>
<td class="cellrowborder" valign="top" width="32.519999999999996%" headers="mcps1.1.5.1.4 "><p id="p19176144942317"><a name="p19176144942317"></a><a name="p19176144942317"></a>-</p>
</td>
</tr>
</tbody>
</table>

**返回值<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="38.940000000000005%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="61.06%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="38.940000000000005%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>scann.scann_ops.py.scann_builder.ScannBuilder</p>
</td>
<td class="cellrowborder" valign="top" width="61.06%" headers="mcps1.1.3.1.2 "><p id="p85639291550"><a name="p85639291550"></a><a name="p85639291550"></a>ScannBuilder类用于接收构建参数。</p>
</td>
</tr>
</tbody>
</table>

### build

**接口定义<a name="section172317194488"></a>**

def build\(\) -\> scann.scann\_ops.ScannSearcher

**接口用途<a name="section1153124784912"></a>**

用于构建索引（与开源算法保持一致）。

**参数说明<a name="section157501312135019"></a>**

无入参。

**返回值<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="38.940000000000005%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="61.06%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="38.940000000000005%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>scann.scann_ops.ScannSearcher</p>
</td>
<td class="cellrowborder" valign="top" width="61.06%" headers="mcps1.1.3.1.2 "><p id="p162342271911"><a name="p162342271911"></a><a name="p162342271911"></a>开始构建并返回构建好的ScannSearcher。</p>
</td>
</tr>
</tbody>
</table>

### serialize\_to\_mem

**接口定义<a name="section172317194488"></a>**

def serialize\_to\_mem\(\) -\> numpy.ndarray

**接口用途<a name="section1153124784912"></a>**

将构建好的索引储存在数组中（相比开源算法新增的接口）。

**参数说明<a name="section157501312135019"></a>**

无入参。

**返回值<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="38.940000000000005%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="61.06%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="38.940000000000005%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>numpy.ndarray</p>
</td>
<td class="cellrowborder" valign="top" width="61.06%" headers="mcps1.1.3.1.2 "><p id="p11245194815244"><a name="p11245194815244"></a><a name="p11245194815244"></a>存储序列化内容的数组。</p>
</td>
</tr>
</tbody>
</table>

### deserialize\_from\_mem

**接口定义<a name="section172317194488"></a>**

def deserialize\_to\_mem\(serialize\_data: numpy.ndarray\) -\> int

**接口用途<a name="section1153124784912"></a>**

给定存储序列化内容的数组，还原一个检索器的索引实例（相比开源算法新增的接口）。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="19.15%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="15.5%" id="mcps1.1.5.1.2"><p id="p990293519329"><a name="p990293519329"></a><a name="p990293519329"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="30.98%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="34.37%" id="mcps1.1.5.1.4"><p id="p1124319456225"><a name="p1124319456225"></a><a name="p1124319456225"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="19.15%" headers="mcps1.1.5.1.1 "><p id="p1854091217440"><a name="p1854091217440"></a><a name="p1854091217440"></a>serialize_data</p>
</td>
<td class="cellrowborder" valign="top" width="15.5%" headers="mcps1.1.5.1.2 "><p id="p5738165216253"><a name="p5738165216253"></a><a name="p5738165216253"></a>numpy.ndarray</p>
</td>
<td class="cellrowborder" valign="top" width="30.98%" headers="mcps1.1.5.1.3 "><p id="p1283214411428"><a name="p1283214411428"></a><a name="p1283214411428"></a>存储序列化内容的数组。</p>
</td>
<td class="cellrowborder" valign="top" width="34.37%" headers="mcps1.1.5.1.4 "><p id="p51185910251"><a name="p51185910251"></a><a name="p51185910251"></a>限制非空。</p>
</td>
</tr>
</tbody>
</table>

**返回值<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="38.940000000000005%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="61.06%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="38.940000000000005%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="61.06%" headers="mcps1.1.3.1.2 "><p id="p19997736105"><a name="p19997736105"></a><a name="p19997736105"></a>接口由底层C++接口封装而来，异常抛出由底层C++接口控制。</p>
</td>
</tr>
</tbody>
</table>

### get\_num

**接口定义<a name="section172317194488"></a>**

def get\_num\(\) -\> int

**接口用途<a name="section1153124784912"></a>**

获取底库向量的数量（相比开源算法新增的接口）。

**参数说明<a name="section157501312135019"></a>**

无入参。

**返回值<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="38.940000000000005%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="61.06%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="38.940000000000005%" headers="mcps1.1.3.1.1 "><p id="p12716362716"><a name="p12716362716"></a><a name="p12716362716"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="61.06%" headers="mcps1.1.3.1.2 "><p id="p11245194815244"><a name="p11245194815244"></a><a name="p11245194815244"></a>返回底库向量的数量。</p>
</td>
</tr>
</tbody>
</table>

### get\_dim

**接口定义<a name="section172317194488"></a>**

def get\_dim\(\) -\> int

**接口用途<a name="section1153124784912"></a>**

获取底库向量的维度（相比开源算法新增的接口）。

**参数说明<a name="section157501312135019"></a>**

无入参。

**返回值<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="38.940000000000005%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="61.06%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="38.940000000000005%" headers="mcps1.1.3.1.1 "><p id="p12716362716"><a name="p12716362716"></a><a name="p12716362716"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="61.06%" headers="mcps1.1.3.1.2 "><p id="p11245194815244"><a name="p11245194815244"></a><a name="p11245194815244"></a>返回底库向量的维度。</p>
</td>
</tr>
</tbody>
</table>

### create\_searcher

**接口定义<a name="section172317194488"></a>**

def create\_searcher\(db: numpy.ndarray, scann\_config: str, training\_threads: int, docids: numpy.ndarray, kmopt\_pq\_iter: int, kmopt\_pq\_sample: int, kmopt\_pq\_init: int, kmopt\_ivf\_iter: int, kmopt\_ivf\_sample: int, kmopt\_ivf\_init: int, filter\_thr: float, filter\_type: int\) -\> scann.scann\_ops.ScannSearcher

**接口用途<a name="section1153124784912"></a>**

基于入参构建索引并返回ScannSearcher（与开源算法相比增加filter\_thr和filter\_type参数）。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="19.15%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="15.5%" id="mcps1.1.5.1.2"><p id="p990293519329"><a name="p990293519329"></a><a name="p990293519329"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="30.98%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="34.37%" id="mcps1.1.5.1.4"><p id="p1124319456225"><a name="p1124319456225"></a><a name="p1124319456225"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="19.15%" headers="mcps1.1.5.1.1 "><p id="p27282142019"><a name="p27282142019"></a><a name="p27282142019"></a>db</p>
</td>
<td class="cellrowborder" valign="top" width="15.5%" headers="mcps1.1.5.1.2 "><p id="p47284141806"><a name="p47284141806"></a><a name="p47284141806"></a>numpy.ndarray</p>
</td>
<td class="cellrowborder" valign="top" width="30.98%" headers="mcps1.1.5.1.3 "><p id="p13728101417015"><a name="p13728101417015"></a><a name="p13728101417015"></a>底库向量。</p>
</td>
<td class="cellrowborder" valign="top" width="34.37%" headers="mcps1.1.5.1.4 "><p id="p57289141105"><a name="p57289141105"></a><a name="p57289141105"></a>限制非空。</p>
</td>
</tr>
<tr id="row1636620413570"><td class="cellrowborder" valign="top" width="19.15%" headers="mcps1.1.5.1.1 "><p id="p197282143013"><a name="p197282143013"></a><a name="p197282143013"></a>scann_config</p>
</td>
<td class="cellrowborder" valign="top" width="15.5%" headers="mcps1.1.5.1.2 "><p id="p27288142011"><a name="p27288142011"></a><a name="p27288142011"></a>字符串</p>
</td>
<td class="cellrowborder" valign="top" width="30.98%" headers="mcps1.1.5.1.3 "><p id="p97284141307"><a name="p97284141307"></a><a name="p97284141307"></a>构建索引所需的配置文件，包含所有配置参数。</p>
</td>
<td class="cellrowborder" valign="top" width="34.37%" headers="mcps1.1.5.1.4 "><p id="p1072818144017"><a name="p1072818144017"></a><a name="p1072818144017"></a>-</p>
</td>
</tr>
<tr id="row159018433576"><td class="cellrowborder" valign="top" width="19.15%" headers="mcps1.1.5.1.1 "><p id="p9728191418018"><a name="p9728191418018"></a><a name="p9728191418018"></a>training_threads</p>
</td>
<td class="cellrowborder" valign="top" width="15.5%" headers="mcps1.1.5.1.2 "><p id="p2072813147011"><a name="p2072813147011"></a><a name="p2072813147011"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="30.98%" headers="mcps1.1.5.1.3 "><p id="p1572818146018"><a name="p1572818146018"></a><a name="p1572818146018"></a>设置用于索引构建的线程数。</p>
</td>
<td class="cellrowborder" valign="top" width="34.37%" headers="mcps1.1.5.1.4 "><p id="p172861413012"><a name="p172861413012"></a><a name="p172861413012"></a>[0, MAXINT]，默认为0。</p>
</td>
</tr>
<tr id="row45159449576"><td class="cellrowborder" valign="top" width="19.15%" headers="mcps1.1.5.1.1 "><p id="p15728414005"><a name="p15728414005"></a><a name="p15728414005"></a>docids</p>
</td>
<td class="cellrowborder" valign="top" width="15.5%" headers="mcps1.1.5.1.2 "><p id="p1872817141501"><a name="p1872817141501"></a><a name="p1872817141501"></a>numpy.ndarray</p>
</td>
<td class="cellrowborder" valign="top" width="30.98%" headers="mcps1.1.5.1.3 "><p id="p5728111420017"><a name="p5728111420017"></a><a name="p5728111420017"></a>文档ID。</p>
</td>
<td class="cellrowborder" valign="top" width="34.37%" headers="mcps1.1.5.1.4 "><p id="p177289141605"><a name="p177289141605"></a><a name="p177289141605"></a>默认None</p>
</td>
</tr>
<tr id="row135180468578"><td class="cellrowborder" valign="top" width="19.15%" headers="mcps1.1.5.1.1 "><p id="p97288145010"><a name="p97288145010"></a><a name="p97288145010"></a>kmopt_pq_iter</p>
</td>
<td class="cellrowborder" valign="top" width="15.5%" headers="mcps1.1.5.1.2 "><p id="p10728151410013"><a name="p10728151410013"></a><a name="p10728151410013"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="30.98%" headers="mcps1.1.5.1.3 "><p id="p2728814701"><a name="p2728814701"></a><a name="p2728814701"></a>PQ中Kmeans迭代次数。</p>
</td>
<td class="cellrowborder" valign="top" width="34.37%" headers="mcps1.1.5.1.4 "><p id="p87289141603"><a name="p87289141603"></a><a name="p87289141603"></a>[0, MAXINT]，默认为0。</p>
</td>
</tr>
<tr id="row9574144845717"><td class="cellrowborder" valign="top" width="19.15%" headers="mcps1.1.5.1.1 "><p id="p57281014906"><a name="p57281014906"></a><a name="p57281014906"></a>kmopt_pq_sample</p>
</td>
<td class="cellrowborder" valign="top" width="15.5%" headers="mcps1.1.5.1.2 "><p id="p12728151412019"><a name="p12728151412019"></a><a name="p12728151412019"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="30.98%" headers="mcps1.1.5.1.3 "><p id="p97288141013"><a name="p97288141013"></a><a name="p97288141013"></a>PQ中KMeans聚类采样子集大小。</p>
</td>
<td class="cellrowborder" valign="top" width="34.37%" headers="mcps1.1.5.1.4 "><p id="p1872813141500"><a name="p1872813141500"></a><a name="p1872813141500"></a>[0, MAXINT]，默认为0。</p>
</td>
</tr>
<tr id="row553518556578"><td class="cellrowborder" valign="top" width="19.15%" headers="mcps1.1.5.1.1 "><p id="p77288141705"><a name="p77288141705"></a><a name="p77288141705"></a>kmopt_pq_init</p>
</td>
<td class="cellrowborder" valign="top" width="15.5%" headers="mcps1.1.5.1.2 "><p id="p47282014503"><a name="p47282014503"></a><a name="p47282014503"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="30.98%" headers="mcps1.1.5.1.3 "><p id="p9728191420011"><a name="p9728191420011"></a><a name="p9728191420011"></a>PQ中KMeans初始化类型。</p>
</td>
<td class="cellrowborder" valign="top" width="34.37%" headers="mcps1.1.5.1.4 "><p id="p5728161415020"><a name="p5728161415020"></a><a name="p5728161415020"></a>{0,1,2,3}，默认为0。</p>
<a name="ul4248355772"></a><a name="ul4248355772"></a><ul id="ul4248355772"><li>1：基于“平均距离”初始化。</li><li>2：K-Means++ 初始化。</li><li>3：随机初始化。</li><li>0：不开启PQ中KMeans优化。</li></ul>
</td>
</tr>
<tr id="row499605614572"><td class="cellrowborder" valign="top" width="19.15%" headers="mcps1.1.5.1.1 "><p id="p872815141508"><a name="p872815141508"></a><a name="p872815141508"></a>kmopt_ivf_iter</p>
</td>
<td class="cellrowborder" valign="top" width="15.5%" headers="mcps1.1.5.1.2 "><p id="p872811141806"><a name="p872811141806"></a><a name="p872811141806"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="30.98%" headers="mcps1.1.5.1.3 "><p id="p1672811415017"><a name="p1672811415017"></a><a name="p1672811415017"></a>IVF中Kmeans迭代次数。</p>
</td>
<td class="cellrowborder" valign="top" width="34.37%" headers="mcps1.1.5.1.4 "><p id="p1372831413011"><a name="p1372831413011"></a><a name="p1372831413011"></a>[0, MAXINT]，默认为0。</p>
</td>
</tr>
<tr id="row1643755885714"><td class="cellrowborder" valign="top" width="19.15%" headers="mcps1.1.5.1.1 "><p id="p1728414102"><a name="p1728414102"></a><a name="p1728414102"></a>kmopt_ivf_sample</p>
</td>
<td class="cellrowborder" valign="top" width="15.5%" headers="mcps1.1.5.1.2 "><p id="p772812141301"><a name="p772812141301"></a><a name="p772812141301"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="30.98%" headers="mcps1.1.5.1.3 "><p id="p1572815148011"><a name="p1572815148011"></a><a name="p1572815148011"></a>IVF中KMeans聚类采样子集大小。</p>
</td>
<td class="cellrowborder" valign="top" width="34.37%" headers="mcps1.1.5.1.4 "><p id="p14728814103"><a name="p14728814103"></a><a name="p14728814103"></a>[0, MAXINT]，默认为0。</p>
</td>
</tr>
<tr id="row413120105819"><td class="cellrowborder" valign="top" width="19.15%" headers="mcps1.1.5.1.1 "><p id="p799642417014"><a name="p799642417014"></a><a name="p799642417014"></a>kmopt_ivf_init</p>
</td>
<td class="cellrowborder" valign="top" width="15.5%" headers="mcps1.1.5.1.2 "><p id="p599618241406"><a name="p599618241406"></a><a name="p599618241406"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="30.98%" headers="mcps1.1.5.1.3 "><p id="p179968241606"><a name="p179968241606"></a><a name="p179968241606"></a>IVF中KMeans初始化类型。</p>
</td>
<td class="cellrowborder" valign="top" width="34.37%" headers="mcps1.1.5.1.4 "><p id="p16996924209"><a name="p16996924209"></a><a name="p16996924209"></a>{0,1,2,3}，默认为0。</p>
<a name="ul149618472811"></a><a name="ul149618472811"></a><ul id="ul149618472811"><li>1：基于“平均距离”初始化。</li><li>2：K-Means++ 初始化。</li><li>3：随机初始化。</li><li>0：不开启IVF中KMeans优化。</li></ul>
</td>
</tr>
<tr id="row1585616175817"><td class="cellrowborder" valign="top" width="19.15%" headers="mcps1.1.5.1.1 "><p id="p799610241405"><a name="p799610241405"></a><a name="p799610241405"></a>filter_thr</p>
</td>
<td class="cellrowborder" valign="top" width="15.5%" headers="mcps1.1.5.1.2 "><p id="p699613243015"><a name="p699613243015"></a><a name="p699613243015"></a>float</p>
</td>
<td class="cellrowborder" valign="top" width="30.98%" headers="mcps1.1.5.1.3 "><p id="p099662410015"><a name="p099662410015"></a><a name="p099662410015"></a>过滤阈值。</p>
</td>
<td class="cellrowborder" valign="top" width="34.37%" headers="mcps1.1.5.1.4 "><p id="p10996152419010"><a name="p10996152419010"></a><a name="p10996152419010"></a>[0, 1]，默认为0。</p>
</td>
</tr>
<tr id="row6521103175811"><td class="cellrowborder" valign="top" width="19.15%" headers="mcps1.1.5.1.1 "><p id="p139967244015"><a name="p139967244015"></a><a name="p139967244015"></a>filter_type</p>
</td>
<td class="cellrowborder" valign="top" width="15.5%" headers="mcps1.1.5.1.2 "><p id="p1399682411017"><a name="p1399682411017"></a><a name="p1399682411017"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="30.98%" headers="mcps1.1.5.1.3 "><p id="p1199714241403"><a name="p1199714241403"></a><a name="p1199714241403"></a>过滤类型。</p>
</td>
<td class="cellrowborder" valign="top" width="34.37%" headers="mcps1.1.5.1.4 "><p id="p799717243014"><a name="p799717243014"></a><a name="p799717243014"></a>0 或 1，默认为0。</p>
<a name="ul1556112894"></a><a name="ul1556112894"></a><ul id="ul1556112894"><li>0：根据向量中0的元素个数进行过滤</li><li>1：根据向量中各个数与均值偏差大小进行过滤</li></ul>
</td>
</tr>
</tbody>
</table>

**返回值<a name="section19841444181515"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="38.940000000000005%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="61.06%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="38.940000000000005%" headers="mcps1.1.3.1.1 "><p id="p12704198101020"><a name="p12704198101020"></a><a name="p12704198101020"></a>scann.scann_ops.ScannSearcher</p>
</td>
<td class="cellrowborder" valign="top" width="61.06%" headers="mcps1.1.3.1.2 "><p id="p167042821017"><a name="p167042821017"></a><a name="p167042821017"></a>开始构建并返回构建好的ScannSearcher。</p>
</td>
</tr>
</tbody>
</table>

## C++接口

### 接口说明

KScaNN不提供对外接口，基于开源ScaNN算法做侵入式修改，对开源核心工具类ScannInterface里的类方法有新增。为获得最优性能，KScaNN接口内部不做完整入参校验，入参合法性由调用方业务来保证。KScaNN侵入式修改后的ScannInterface类方法如[**表 1** KScaNN修改后的ScannInterface类方法](#KScaNN修改后的ScannInterface类方法)所示。

**表 1** KScaNN修改后的ScannInterface类方法<a id="KScaNN修改后的ScannInterface类方法"></a>

<a name="table1194910128449"></a>
<table><thead align="left"><tr id="row99491812134412"><th class="cellrowborder" valign="top" width="31.269999999999996%" id="mcps1.2.3.1.1"><p id="p1794951224415"><a name="p1794951224415"></a><a name="p1794951224415"></a>接口名称</p>
</th>
<th class="cellrowborder" valign="top" width="68.73%" id="mcps1.2.3.1.2"><p id="p6949612124415"><a name="p6949612124415"></a><a name="p6949612124415"></a>接口作用</p>
</th>
</tr>
</thead>
<tbody><tr id="row712018285575"><td class="cellrowborder" valign="top" width="31.269999999999996%" headers="mcps1.2.3.1.1 "><p id="p12121102835714"><a name="p12121102835714"></a><a name="p12121102835714"></a>SetNumThreads</p>
</td>
<td class="cellrowborder" valign="top" width="68.73%" headers="mcps1.2.3.1.2 "><p id="p111217289571"><a name="p111217289571"></a><a name="p111217289571"></a>配置搜索时启用线程数（相比开源算法新增方法）。</p>
</td>
</tr>
<tr id="row119491112174414"><td class="cellrowborder" valign="top" width="31.269999999999996%" headers="mcps1.2.3.1.1 "><p id="p539219519167"><a name="p539219519167"></a><a name="p539219519167"></a>SearchAdditionalParams</p>
</td>
<td class="cellrowborder" valign="top" width="68.73%" headers="mcps1.2.3.1.2 "><p id="p3949012174411"><a name="p3949012174411"></a><a name="p3949012174411"></a>用于扩展ScaNN检索功能，提供额外的检索参数配置方法（相比开源算法新增方法）。</p>
</td>
</tr>
<tr id="row9949131219443"><td class="cellrowborder" valign="top" width="31.269999999999996%" headers="mcps1.2.3.1.1 "><p id="p1094921294415"><a name="p1094921294415"></a><a name="p1094921294415"></a>Search</p>
</td>
<td class="cellrowborder" valign="top" width="68.73%" headers="mcps1.2.3.1.2 "><p id="p1794941284418"><a name="p1794941284418"></a><a name="p1794941284418"></a>单query搜索方法，单线程执行（与开源算法方法保持一致）。</p>
</td>
</tr>
<tr id="row1594913120443"><td class="cellrowborder" valign="top" width="31.269999999999996%" headers="mcps1.2.3.1.1 "><p id="p4949012144417"><a name="p4949012144417"></a><a name="p4949012144417"></a>SearchBatched</p>
</td>
<td class="cellrowborder" valign="top" width="68.73%" headers="mcps1.2.3.1.2 "><p id="p1509193871710"><a name="p1509193871710"></a><a name="p1509193871710"></a>批量query搜索方法，单线程执行（与开源算法方法保持一致）。</p>
</td>
</tr>
<tr id="row6949131274416"><td class="cellrowborder" valign="top" width="31.269999999999996%" headers="mcps1.2.3.1.1 "><p id="p18867143114163"><a name="p18867143114163"></a><a name="p18867143114163"></a>SearchBatchedParallel</p>
</td>
<td class="cellrowborder" valign="top" width="68.73%" headers="mcps1.2.3.1.2 "><p id="p794971214414"><a name="p794971214414"></a><a name="p794971214414"></a>并行批量query搜索方法，多线程并发执行（与开源算法方法保持一致）。</p>
</td>
</tr>
<tr id="row694916124445"><td class="cellrowborder" valign="top" width="31.269999999999996%" headers="mcps1.2.3.1.1 "><p id="p136701839191615"><a name="p136701839191615"></a><a name="p136701839191615"></a>Initialize</p>
</td>
<td class="cellrowborder" valign="top" width="68.73%" headers="mcps1.2.3.1.2 "><p id="p894941210443"><a name="p894941210443"></a><a name="p894941210443"></a>用于构建索引（与开源算法方法保持一致）。</p>
</td>
</tr>
<tr id="row159491712174414"><td class="cellrowborder" valign="top" width="31.269999999999996%" headers="mcps1.2.3.1.1 "><p id="p10497124591619"><a name="p10497124591619"></a><a name="p10497124591619"></a>SerializeToMemory</p>
</td>
<td class="cellrowborder" valign="top" width="68.73%" headers="mcps1.2.3.1.2 "><p id="p2094917128448"><a name="p2094917128448"></a><a name="p2094917128448"></a>将索引序列化储存在内存中（相比开源算法新增方法）。</p>
</td>
</tr>
<tr id="row198655487161"><td class="cellrowborder" valign="top" width="31.269999999999996%" headers="mcps1.2.3.1.1 "><p id="p11866448181619"><a name="p11866448181619"></a><a name="p11866448181619"></a>LoadFromMemory</p>
</td>
<td class="cellrowborder" valign="top" width="68.73%" headers="mcps1.2.3.1.2 "><p id="p786624801615"><a name="p786624801615"></a><a name="p786624801615"></a>从内存中还原索引实例（相比开源算法新增方法）。</p>
</td>
</tr>
<tr id="row132215567163"><td class="cellrowborder" valign="top" width="31.269999999999996%" headers="mcps1.2.3.1.1 "><p id="p102211256151619"><a name="p102211256151619"></a><a name="p102211256151619"></a>GetNum</p>
</td>
<td class="cellrowborder" valign="top" width="68.73%" headers="mcps1.2.3.1.2 "><p id="p18221256191618"><a name="p18221256191618"></a><a name="p18221256191618"></a>获取底库向量的数量（相比开源算法新增方法）。</p>
</td>
</tr>
<tr id="row12818101418175"><td class="cellrowborder" valign="top" width="31.269999999999996%" headers="mcps1.2.3.1.1 "><p id="p9818141401711"><a name="p9818141401711"></a><a name="p9818141401711"></a>GetDim</p>
</td>
<td class="cellrowborder" valign="top" width="68.73%" headers="mcps1.2.3.1.2 "><p id="p1818181431719"><a name="p1818181431719"></a><a name="p1818181431719"></a>获取底库向量的维度（相比开源算法新增方法）。</p>
</td>
</tr>
</tbody>
</table>

### SetNumThreads

**接口定义<a name="section194415111419"></a>**

void ScannInterface::SetNumThreads\(int num\_threads\);

**接口用途<a name="section1153124784912"></a>**

配置搜索时启用线程数（相比开源算法新增方法）。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.898410158984102%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.31826817318268%" id="mcps1.1.5.1.2"><p id="p18620101081116"><a name="p18620101081116"></a><a name="p18620101081116"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="20.94790520947905%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="45.83541645835416%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.898410158984102%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>num_threads</p>
</td>
<td class="cellrowborder" valign="top" width="17.31826817318268%" headers="mcps1.1.5.1.2 "><p id="p15620161014116"><a name="p15620161014116"></a><a name="p15620161014116"></a><span>int</span></p>
</td>
<td class="cellrowborder" valign="top" width="20.94790520947905%" headers="mcps1.1.5.1.3 "><p id="p182303331508"><a name="p182303331508"></a><a name="p182303331508"></a>线程数量。</p>
</td>
<td class="cellrowborder" valign="top" width="45.83541645835416%" headers="mcps1.1.5.1.4 "><p id="p1151275553412"><a name="p1151275553412"></a><a name="p1151275553412"></a>大于等于2。推荐设置为运行时CPU核数。</p>
</td>
</tr>
</tbody>
</table>

### SearchAdditionalParams

**接口定义<a name="section172317194488"></a>**

void ScannInterface::SearchAdditionalParams\(float adp\_threshold, float refine\_prm, int adp\_refined, int leaves\_to\_search\);

**接口用途<a name="section1153124784912"></a>**

用于扩展ScaNN检索功能，提供额外的检索参数配置接口（相比开源算法新增方法）。应在索引构建后、检索前调用设置，接口参数具备缓存功能，一次设置，后续检索均生效。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="21.12%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="13.4%" id="mcps1.1.5.1.2"><p id="p73401941182314"><a name="p73401941182314"></a><a name="p73401941182314"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="34.98%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="30.5%" id="mcps1.1.5.1.4"><p id="p232514861412"><a name="p232514861412"></a><a name="p232514861412"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="21.12%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>adp_threshold</p>
</td>
<td class="cellrowborder" valign="top" width="13.4%" headers="mcps1.1.5.1.2 "><p id="p634084116239"><a name="p634084116239"></a><a name="p634084116239"></a>float</p>
</td>
<td class="cellrowborder" valign="top" width="34.98%" headers="mcps1.1.5.1.3 "><p id="p1551821410413"><a name="p1551821410413"></a><a name="p1551821410413"></a>决策阈值，典型值0.3。</p>
</td>
<td class="cellrowborder" valign="top" width="30.5%" headers="mcps1.1.5.1.4 "><p id="p2223102401510"><a name="p2223102401510"></a><a name="p2223102401510"></a>[0.1, 0.8]</p>
</td>
</tr>
<tr id="row175381054161617"><td class="cellrowborder" valign="top" width="21.12%" headers="mcps1.1.5.1.1 "><p id="p188543596166"><a name="p188543596166"></a><a name="p188543596166"></a>refine_prm</p>
</td>
<td class="cellrowborder" valign="top" width="13.4%" headers="mcps1.1.5.1.2 "><p id="p18541959181613"><a name="p18541959181613"></a><a name="p18541959181613"></a>float</p>
</td>
<td class="cellrowborder" valign="top" width="34.98%" headers="mcps1.1.5.1.3 "><p id="p285455916165"><a name="p285455916165"></a><a name="p285455916165"></a>精细化控制过滤策略，典型值0.2。</p>
</td>
<td class="cellrowborder" valign="top" width="30.5%" headers="mcps1.1.5.1.4 "><p id="p6854759151617"><a name="p6854759151617"></a><a name="p6854759151617"></a>[0.0, 1.0]，默认为0.0。值越大则过滤的子空间个数越少，精度越高，但性能会下降。</p>
</td>
</tr>
<tr id="row11230173385019"><td class="cellrowborder" valign="top" width="21.12%" headers="mcps1.1.5.1.1 "><p id="p6412202812239"><a name="p6412202812239"></a><a name="p6412202812239"></a>adp_refined</p>
</td>
<td class="cellrowborder" valign="top" width="13.4%" headers="mcps1.1.5.1.2 "><p id="p153407416237"><a name="p153407416237"></a><a name="p153407416237"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="34.98%" headers="mcps1.1.5.1.3 "><p id="p27308382419"><a name="p27308382419"></a><a name="p27308382419"></a>简单query所采用的子空间个数，典型值0，为训练自适应值（75分位点）。</p>
</td>
<td class="cellrowborder" valign="top" width="30.5%" headers="mcps1.1.5.1.4 "><p id="p9223152491519"><a name="p9223152491519"></a><a name="p9223152491519"></a>[0, leaves_to_search]，其中<span class="parmname" id="parmname2089000161016"><a name="parmname2089000161016"></a><a name="parmname2089000161016"></a>“leaves_to_search”</span>表示复杂query所采用的子空间个数。</p>
</td>
</tr>
<tr id="row92309336505"><td class="cellrowborder" valign="top" width="21.12%" headers="mcps1.1.5.1.1 "><p id="p162309336505"><a name="p162309336505"></a><a name="p162309336505"></a>leaves_to_search</p>
</td>
<td class="cellrowborder" valign="top" width="13.4%" headers="mcps1.1.5.1.2 "><p id="p14340141122314"><a name="p14340141122314"></a><a name="p14340141122314"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="34.98%" headers="mcps1.1.5.1.3 "><p id="p764411521247"><a name="p764411521247"></a><a name="p764411521247"></a>复杂query所采用的子空间个数，应与实际检索（Search*）接口参数一致。</p>
</td>
<td class="cellrowborder" valign="top" width="30.5%" headers="mcps1.1.5.1.4 "><p id="p19223324111511"><a name="p19223324111511"></a><a name="p19223324111511"></a>[1, num_leaves]，其中<span class="parmname" id="parmname1935718105112"><a name="parmname1935718105112"></a><a name="parmname1935718105112"></a>“num_leaves”</span>表示IVF（Inverted File）倒排索引分区总子空间个数。</p>
</td>
</tr>
</tbody>
</table>

### Search

**接口定义<a name="section172317194488"></a>**

Status ScannInterface::Search\(const DatapointPtr<float\> query, NNResultsVector\* res, int final\_nn, int pre\_reorder\_nn, int leaves\) const;

**接口用途<a name="section1153124784912"></a>**

单query搜索接口，单线程执行（与开源算法方法保持一致）。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="16.830000000000002%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.57%" id="mcps1.1.5.1.2"><p id="p73401941182314"><a name="p73401941182314"></a><a name="p73401941182314"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="35.099999999999994%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="30.5%" id="mcps1.1.5.1.4"><p id="p232514861412"><a name="p232514861412"></a><a name="p232514861412"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="16.830000000000002%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>query</p>
</td>
<td class="cellrowborder" valign="top" width="17.57%" headers="mcps1.1.5.1.2 "><p id="p634084116239"><a name="p634084116239"></a><a name="p634084116239"></a>const DatapointPtr&lt;float&gt;</p>
</td>
<td class="cellrowborder" valign="top" width="35.099999999999994%" headers="mcps1.1.5.1.3 "><p id="p1551821410413"><a name="p1551821410413"></a><a name="p1551821410413"></a>Query。</p>
</td>
<td class="cellrowborder" valign="top" width="30.5%" headers="mcps1.1.5.1.4 "><p id="p2223102401510"><a name="p2223102401510"></a><a name="p2223102401510"></a>限制非空。</p>
</td>
</tr>
<tr id="row11230173385019"><td class="cellrowborder" valign="top" width="16.830000000000002%" headers="mcps1.1.5.1.1 "><p id="p6412202812239"><a name="p6412202812239"></a><a name="p6412202812239"></a>res</p>
</td>
<td class="cellrowborder" valign="top" width="17.57%" headers="mcps1.1.5.1.2 "><p id="p153407416237"><a name="p153407416237"></a><a name="p153407416237"></a>NNResultsVector*</p>
</td>
<td class="cellrowborder" valign="top" width="35.099999999999994%" headers="mcps1.1.5.1.3 "><p id="p27308382419"><a name="p27308382419"></a><a name="p27308382419"></a>用于存储最终需要的结果（labals, distances），每一项长度为final_nn，其中<span class="parmname" id="parmname2295133316124"><a name="parmname2295133316124"></a><a name="parmname2295133316124"></a>“final_nn”</span>为最终返回结果数量。</p>
</td>
<td class="cellrowborder" valign="top" width="30.5%" headers="mcps1.1.5.1.4 "><p id="p9223152491519"><a name="p9223152491519"></a><a name="p9223152491519"></a>限制非空，长度为查询向量的数量。</p>
</td>
</tr>
<tr id="row92309336505"><td class="cellrowborder" valign="top" width="16.830000000000002%" headers="mcps1.1.5.1.1 "><p id="p3223153018443"><a name="p3223153018443"></a><a name="p3223153018443"></a>final_nn</p>
</td>
<td class="cellrowborder" valign="top" width="17.57%" headers="mcps1.1.5.1.2 "><p id="p14340141122314"><a name="p14340141122314"></a><a name="p14340141122314"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="35.099999999999994%" headers="mcps1.1.5.1.3 "><p id="p764411521247"><a name="p764411521247"></a><a name="p764411521247"></a>最终返回结果数量，TopK。</p>
</td>
<td class="cellrowborder" valign="top" width="30.5%" headers="mcps1.1.5.1.4 "><p id="p195481334151716"><a name="p195481334151716"></a><a name="p195481334151716"></a>大于等于1，与构建时保持一致。</p>
</td>
</tr>
<tr id="row115518116154"><td class="cellrowborder" valign="top" width="16.830000000000002%" headers="mcps1.1.5.1.1 "><p id="p7569116152"><a name="p7569116152"></a><a name="p7569116152"></a>pre_reorder_nn</p>
</td>
<td class="cellrowborder" valign="top" width="17.57%" headers="mcps1.1.5.1.2 "><p id="p1456111121515"><a name="p1456111121515"></a><a name="p1456111121515"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="35.099999999999994%" headers="mcps1.1.5.1.3 "><p id="p92301933165017"><a name="p92301933165017"></a><a name="p92301933165017"></a>重排前保存结果数量。</p>
</td>
<td class="cellrowborder" valign="top" width="30.5%" headers="mcps1.1.5.1.4 "><p id="p849114441619"><a name="p849114441619"></a><a name="p849114441619"></a>大于等于final_nn，其中<span class="parmname" id="parmname16137152615912"><a name="parmname16137152615912"></a><a name="parmname16137152615912"></a>“final_nn”</span>为最终返回结果数量。</p>
</td>
</tr>
<tr id="row02257841513"><td class="cellrowborder" valign="top" width="16.830000000000002%" headers="mcps1.1.5.1.1 "><p id="p1822517815157"><a name="p1822517815157"></a><a name="p1822517815157"></a>leaves</p>
</td>
<td class="cellrowborder" valign="top" width="17.57%" headers="mcps1.1.5.1.2 "><p id="p02251989153"><a name="p02251989153"></a><a name="p02251989153"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="35.099999999999994%" headers="mcps1.1.5.1.3 "><p id="p1678617193274"><a name="p1678617193274"></a><a name="p1678617193274"></a>搜索子空间数量。</p>
</td>
<td class="cellrowborder" valign="top" width="30.5%" headers="mcps1.1.5.1.4 "><p id="p54914451617"><a name="p54914451617"></a><a name="p54914451617"></a>[1, n_leaves]，其中<span class="parmname" id="parmname13412142641214"><a name="parmname13412142641214"></a><a name="parmname13412142641214"></a>“n_leaves”</span>为IVF倒排索引分区总子空间个数。</p>
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
<tbody><tr id="row769192744612"><td class="cellrowborder" valign="top" width="34.599999999999994%" headers="mcps1.1.3.1.1 "><p id="p106910272463"><a name="p106910272463"></a><a name="p106910272463"></a>Status</p>
</td>
<td class="cellrowborder" valign="top" width="65.4%" headers="mcps1.1.3.1.2 "><p id="p14195191116393"><a name="p14195191116393"></a><a name="p14195191116393"></a>表示方法执行状态，通过status.ok()判断是否成功。</p>
</td>
</tr>
</tbody>
</table>

### SearchBatched

**接口定义<a name="section172317194488"></a>**

Status ScannInterface::SearchBatched\(const DenseDataset<float\>& queries, MutableSpan<NNResultsVector\> res, int final\_nn, int pre\_reorder\_nn, int leaves\) const;

**接口用途<a name="section1153124784912"></a>**

批量query搜索接口，单线程执行（与开源算法方法保持一致）。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="17.28%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="16.509999999999998%" id="mcps1.1.5.1.2"><p id="p73401941182314"><a name="p73401941182314"></a><a name="p73401941182314"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="35.839999999999996%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="30.37%" id="mcps1.1.5.1.4"><p id="p232514861412"><a name="p232514861412"></a><a name="p232514861412"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="17.28%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>queries</p>
</td>
<td class="cellrowborder" valign="top" width="16.509999999999998%" headers="mcps1.1.5.1.2 "><p id="p634084116239"><a name="p634084116239"></a><a name="p634084116239"></a>const DatapointPtr&lt;float&gt;&amp;</p>
</td>
<td class="cellrowborder" valign="top" width="35.839999999999996%" headers="mcps1.1.5.1.3 "><p id="p1551821410413"><a name="p1551821410413"></a><a name="p1551821410413"></a>批次内的Queries。</p>
</td>
<td class="cellrowborder" valign="top" width="30.37%" headers="mcps1.1.5.1.4 "><p id="p2223102401510"><a name="p2223102401510"></a><a name="p2223102401510"></a>限制非空。</p>
</td>
</tr>
<tr id="row11230173385019"><td class="cellrowborder" valign="top" width="17.28%" headers="mcps1.1.5.1.1 "><p id="p6412202812239"><a name="p6412202812239"></a><a name="p6412202812239"></a>res</p>
</td>
<td class="cellrowborder" valign="top" width="16.509999999999998%" headers="mcps1.1.5.1.2 "><p id="p1278518581195"><a name="p1278518581195"></a><a name="p1278518581195"></a>MutableSpan&lt;NNResultsVector&gt;</p>
</td>
<td class="cellrowborder" valign="top" width="35.839999999999996%" headers="mcps1.1.5.1.3 "><p id="p27308382419"><a name="p27308382419"></a><a name="p27308382419"></a>用于存储最终需要的结果（labals, distances），每一项长度为final_nn，其中<span class="parmname" id="parmname2295133316124"><a name="parmname2295133316124"></a><a name="parmname2295133316124"></a>“final_nn”</span>为最终返回结果数量。</p>
</td>
<td class="cellrowborder" valign="top" width="30.37%" headers="mcps1.1.5.1.4 "><p id="p9223152491519"><a name="p9223152491519"></a><a name="p9223152491519"></a>限制非空，长度为查询向量的数量。</p>
</td>
</tr>
<tr id="row92309336505"><td class="cellrowborder" valign="top" width="17.28%" headers="mcps1.1.5.1.1 "><p id="p3223153018443"><a name="p3223153018443"></a><a name="p3223153018443"></a>final_nn</p>
</td>
<td class="cellrowborder" valign="top" width="16.509999999999998%" headers="mcps1.1.5.1.2 "><p id="p14340141122314"><a name="p14340141122314"></a><a name="p14340141122314"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="35.839999999999996%" headers="mcps1.1.5.1.3 "><p id="p764411521247"><a name="p764411521247"></a><a name="p764411521247"></a>最终返回结果数量，TopK。</p>
</td>
<td class="cellrowborder" valign="top" width="30.37%" headers="mcps1.1.5.1.4 "><p id="p195481334151716"><a name="p195481334151716"></a><a name="p195481334151716"></a>大于等于1，与构建时保持一致。</p>
</td>
</tr>
<tr id="row115518116154"><td class="cellrowborder" valign="top" width="17.28%" headers="mcps1.1.5.1.1 "><p id="p7569116152"><a name="p7569116152"></a><a name="p7569116152"></a>pre_reorder_nn</p>
</td>
<td class="cellrowborder" valign="top" width="16.509999999999998%" headers="mcps1.1.5.1.2 "><p id="p1456111121515"><a name="p1456111121515"></a><a name="p1456111121515"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="35.839999999999996%" headers="mcps1.1.5.1.3 "><p id="p92301933165017"><a name="p92301933165017"></a><a name="p92301933165017"></a>重排前保存结果数量。</p>
</td>
<td class="cellrowborder" valign="top" width="30.37%" headers="mcps1.1.5.1.4 "><p id="p849114441619"><a name="p849114441619"></a><a name="p849114441619"></a>大于等于final_nn，其中<span class="parmname" id="parmname16137152615912"><a name="parmname16137152615912"></a><a name="parmname16137152615912"></a>“final_nn”</span>为最终返回结果数量。</p>
</td>
</tr>
<tr id="row02257841513"><td class="cellrowborder" valign="top" width="17.28%" headers="mcps1.1.5.1.1 "><p id="p1822517815157"><a name="p1822517815157"></a><a name="p1822517815157"></a>leaves</p>
</td>
<td class="cellrowborder" valign="top" width="16.509999999999998%" headers="mcps1.1.5.1.2 "><p id="p02251989153"><a name="p02251989153"></a><a name="p02251989153"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="35.839999999999996%" headers="mcps1.1.5.1.3 "><p id="p1678617193274"><a name="p1678617193274"></a><a name="p1678617193274"></a>搜索子空间数量。</p>
</td>
<td class="cellrowborder" valign="top" width="30.37%" headers="mcps1.1.5.1.4 "><p id="p54914451617"><a name="p54914451617"></a><a name="p54914451617"></a>[1, n_leaves]，其中<span class="parmname" id="parmname13412142641214"><a name="parmname13412142641214"></a><a name="parmname13412142641214"></a>“n_leaves”</span>为IVF倒排索引分区总子空间个数。</p>
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
<tbody><tr id="row769192744612"><td class="cellrowborder" valign="top" width="34.599999999999994%" headers="mcps1.1.3.1.1 "><p id="p106910272463"><a name="p106910272463"></a><a name="p106910272463"></a>Status</p>
</td>
<td class="cellrowborder" valign="top" width="65.4%" headers="mcps1.1.3.1.2 "><p id="p14195191116393"><a name="p14195191116393"></a><a name="p14195191116393"></a>表示方法执行状态，通过status.ok()判断是否成功。</p>
</td>
</tr>
</tbody>
</table>

### SearchBatchedParallel

**接口定义<a name="section172317194488"></a>**

1）Status ScannInterface::SearchBatchedParallel\(const DenseDataset<float\>& queries, MutableSpan<NNResultsVector\> res, int final\_nn, int pre\_reorder\_nn, int leaves, int batch\_size\) const;

2）Status ScannInterface::SearchBatchedParallel\(const DenseDataset<float\>& queries, const std::vector<int64\_t\>& indices, MutableSpan<NNResultsVector\> res, int final\_nn, int pre\_reorder\_nn, int leaves, int batch\_size\) const;

**接口用途<a name="section1153124784912"></a>**

1. 并行批量query搜索接口，多线程并发执行（与开源算法方法保持一致）。
2. 并行批量query搜索重载函数，开启component filtering后需要引入过滤元素的索引列表（相比开源算法新增方法）。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.53%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.630000000000003%" id="mcps1.1.5.1.2"><p id="p73401941182314"><a name="p73401941182314"></a><a name="p73401941182314"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="37.72%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="29.12%" id="mcps1.1.5.1.4"><p id="p232514861412"><a name="p232514861412"></a><a name="p232514861412"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.53%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>queries</p>
</td>
<td class="cellrowborder" valign="top" width="17.630000000000003%" headers="mcps1.1.5.1.2 "><p id="p634084116239"><a name="p634084116239"></a><a name="p634084116239"></a>const DatapointPtr&lt;float&gt;&amp;</p>
</td>
<td class="cellrowborder" valign="top" width="37.72%" headers="mcps1.1.5.1.3 "><p id="p1551821410413"><a name="p1551821410413"></a><a name="p1551821410413"></a>批次内的Queries。</p>
</td>
<td class="cellrowborder" valign="top" width="29.12%" headers="mcps1.1.5.1.4 "><p id="p2223102401510"><a name="p2223102401510"></a><a name="p2223102401510"></a>限制非空。</p>
</td>
</tr>
<tr id="row11230173385019"><td class="cellrowborder" valign="top" width="15.53%" headers="mcps1.1.5.1.1 "><p id="p6412202812239"><a name="p6412202812239"></a><a name="p6412202812239"></a>res</p>
</td>
<td class="cellrowborder" valign="top" width="17.630000000000003%" headers="mcps1.1.5.1.2 "><p id="p1278518581195"><a name="p1278518581195"></a><a name="p1278518581195"></a>MutableSpan&lt;NNResultsVector&gt;</p>
</td>
<td class="cellrowborder" valign="top" width="37.72%" headers="mcps1.1.5.1.3 "><p id="p27308382419"><a name="p27308382419"></a><a name="p27308382419"></a>用于存储最终需要的结果（labals, distances），每一项长度为final_nn，其中<span class="parmname" id="parmname2295133316124"><a name="parmname2295133316124"></a><a name="parmname2295133316124"></a>“final_nn”</span>为最终返回结果数量。</p>
</td>
<td class="cellrowborder" valign="top" width="29.12%" headers="mcps1.1.5.1.4 "><p id="p9223152491519"><a name="p9223152491519"></a><a name="p9223152491519"></a>限制非空，长度为查询向量的数量。</p>
</td>
</tr>
<tr id="row92309336505"><td class="cellrowborder" valign="top" width="15.53%" headers="mcps1.1.5.1.1 "><p id="p3223153018443"><a name="p3223153018443"></a><a name="p3223153018443"></a>final_nn</p>
</td>
<td class="cellrowborder" valign="top" width="17.630000000000003%" headers="mcps1.1.5.1.2 "><p id="p14340141122314"><a name="p14340141122314"></a><a name="p14340141122314"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="37.72%" headers="mcps1.1.5.1.3 "><p id="p764411521247"><a name="p764411521247"></a><a name="p764411521247"></a>最终返回结果数量。</p>
</td>
<td class="cellrowborder" valign="top" width="29.12%" headers="mcps1.1.5.1.4 "><p id="p195481334151716"><a name="p195481334151716"></a><a name="p195481334151716"></a>大于等于1，与构建时保持一致。</p>
</td>
</tr>
<tr id="row115518116154"><td class="cellrowborder" valign="top" width="15.53%" headers="mcps1.1.5.1.1 "><p id="p7569116152"><a name="p7569116152"></a><a name="p7569116152"></a>pre_reorder_nn</p>
</td>
<td class="cellrowborder" valign="top" width="17.630000000000003%" headers="mcps1.1.5.1.2 "><p id="p1456111121515"><a name="p1456111121515"></a><a name="p1456111121515"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="37.72%" headers="mcps1.1.5.1.3 "><p id="p92301933165017"><a name="p92301933165017"></a><a name="p92301933165017"></a>重排前保存结果数量。</p>
</td>
<td class="cellrowborder" valign="top" width="29.12%" headers="mcps1.1.5.1.4 "><p id="p849114441619"><a name="p849114441619"></a><a name="p849114441619"></a>大于等于final_nn，其中<span class="parmname" id="parmname16137152615912"><a name="parmname16137152615912"></a><a name="parmname16137152615912"></a>“final_nn”</span>为最终返回结果数量。</p>
</td>
</tr>
<tr id="row02257841513"><td class="cellrowborder" valign="top" width="15.53%" headers="mcps1.1.5.1.1 "><p id="p1822517815157"><a name="p1822517815157"></a><a name="p1822517815157"></a>leaves</p>
</td>
<td class="cellrowborder" valign="top" width="17.630000000000003%" headers="mcps1.1.5.1.2 "><p id="p02251989153"><a name="p02251989153"></a><a name="p02251989153"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="37.72%" headers="mcps1.1.5.1.3 "><p id="p1678617193274"><a name="p1678617193274"></a><a name="p1678617193274"></a>搜索子空间数量。</p>
</td>
<td class="cellrowborder" valign="top" width="29.12%" headers="mcps1.1.5.1.4 "><p id="p54914451617"><a name="p54914451617"></a><a name="p54914451617"></a>[1, n_leaves]，其中<span class="parmname" id="parmname13412142641214"><a name="parmname13412142641214"></a><a name="parmname13412142641214"></a>“n_leaves”</span>为IVF倒排索引分区总子空间个数。</p>
</td>
</tr>
<tr id="row415513253710"><td class="cellrowborder" valign="top" width="15.53%" headers="mcps1.1.5.1.1 "><p id="p1115518218374"><a name="p1115518218374"></a><a name="p1115518218374"></a>indices</p>
</td>
<td class="cellrowborder" valign="top" width="17.630000000000003%" headers="mcps1.1.5.1.2 "><p id="p1115582173710"><a name="p1115582173710"></a><a name="p1115582173710"></a>const std::vector&lt;int64_t&gt;&amp;</p>
</td>
<td class="cellrowborder" valign="top" width="37.72%" headers="mcps1.1.5.1.3 "><p id="p1915512214377"><a name="p1915512214377"></a><a name="p1915512214377"></a>过滤元素的索引。</p>
</td>
<td class="cellrowborder" valign="top" width="29.12%" headers="mcps1.1.5.1.4 "><p id="p15155142173720"><a name="p15155142173720"></a><a name="p15155142173720"></a>限制非空。</p>
</td>
</tr>
<tr id="row58921714141811"><td class="cellrowborder" valign="top" width="15.53%" headers="mcps1.1.5.1.1 "><p id="p1015082111188"><a name="p1015082111188"></a><a name="p1015082111188"></a>batch_size</p>
</td>
<td class="cellrowborder" valign="top" width="17.630000000000003%" headers="mcps1.1.5.1.2 "><p id="p17150152115185"><a name="p17150152115185"></a><a name="p17150152115185"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="37.72%" headers="mcps1.1.5.1.3 "><p id="p13150112115184"><a name="p13150112115184"></a><a name="p13150112115184"></a>批量搜索大小。</p>
</td>
<td class="cellrowborder" valign="top" width="29.12%" headers="mcps1.1.5.1.4 "><p id="p9150421151812"><a name="p9150421151812"></a><a name="p9150421151812"></a>[1, MAXINT]，默认为256。</p>
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
<tbody><tr id="row769192744612"><td class="cellrowborder" valign="top" width="34.599999999999994%" headers="mcps1.1.3.1.1 "><p id="p106910272463"><a name="p106910272463"></a><a name="p106910272463"></a>Status</p>
</td>
<td class="cellrowborder" valign="top" width="65.4%" headers="mcps1.1.3.1.2 "><p id="p14195191116393"><a name="p14195191116393"></a><a name="p14195191116393"></a>表示方法执行状态，通过status.ok()判断是否成功。</p>
</td>
</tr>
</tbody>
</table>

### Initialize

**接口定义<a name="section172317194488"></a>**

1. Status ScannInterface::Initialize\(ConstSpan<float\> dataset, DatapointIndex n\_points, const std::string& config, int training\_threads\);
2. Status ScannInterface::Initialize\(ConstSpan<float\> dataset, DatapointIndex n\_points, const std::string& config, int training\_threads, GmmUtils::KMeansParams kmOpt\);
3. Status ScannInterface::Initialize\(ConstSpan<float\> dataset, DatapointIndex n\_points, const std::string& config, int training\_threads, GmmUtils::KMeansParams kmOpt, float filter\_thr, int filter\_type\);

**接口用途<a name="section1153124784912"></a>**

1. 用于构建索引（与开源算法方法保持一致）。
2. 用于构建索引，第2种Initialize重载函数，为IVF和PQ中的KMeans聚类设置额外参数用于调优（相比开源算法新增方法）。
3. 用于构建索引，第3种Initialize重载函数，为IVF和PQ中的KMeans聚类和Component filtering设置额外参数（相比开源算法新增方法）。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="25%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="18.22%" id="mcps1.1.5.1.2"><p id="p73401941182314"><a name="p73401941182314"></a><a name="p73401941182314"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="27.43%" id="mcps1.1.5.1.3"><p id="p19873319153116"><a name="p19873319153116"></a><a name="p19873319153116"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="29.349999999999998%" id="mcps1.1.5.1.4"><p id="p232514861412"><a name="p232514861412"></a><a name="p232514861412"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>dataset</p>
</td>
<td class="cellrowborder" valign="top" width="18.22%" headers="mcps1.1.5.1.2 "><p id="p1853984510229"><a name="p1853984510229"></a><a name="p1853984510229"></a>ConstSpan&lt;float&gt;</p>
</td>
<td class="cellrowborder" valign="top" width="27.43%" headers="mcps1.1.5.1.3 "><p id="p4954194617364"><a name="p4954194617364"></a><a name="p4954194617364"></a>底库向量。</p>
</td>
<td class="cellrowborder" valign="top" width="29.349999999999998%" headers="mcps1.1.5.1.4 "><p id="p2223102401510"><a name="p2223102401510"></a><a name="p2223102401510"></a>限制非空。</p>
</td>
</tr>
<tr id="row11230173385019"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.1 "><p id="p6412202812239"><a name="p6412202812239"></a><a name="p6412202812239"></a>n_points</p>
</td>
<td class="cellrowborder" valign="top" width="18.22%" headers="mcps1.1.5.1.2 "><p id="p1278518581195"><a name="p1278518581195"></a><a name="p1278518581195"></a>DatapointIndex</p>
</td>
<td class="cellrowborder" valign="top" width="27.43%" headers="mcps1.1.5.1.3 "><p id="p16517949143614"><a name="p16517949143614"></a><a name="p16517949143614"></a>底库向量的数量。</p>
</td>
<td class="cellrowborder" valign="top" width="29.349999999999998%" headers="mcps1.1.5.1.4 "><p id="p9223152491519"><a name="p9223152491519"></a><a name="p9223152491519"></a>限制与dataset的长度保持一致，其中<span class="parmname" id="parmname6229104813232"><a name="parmname6229104813232"></a><a name="parmname6229104813232"></a>“dataset”</span>表示底库向量。</p>
</td>
</tr>
<tr id="row92309336505"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.1 "><p id="p3223153018443"><a name="p3223153018443"></a><a name="p3223153018443"></a>config</p>
</td>
<td class="cellrowborder" valign="top" width="18.22%" headers="mcps1.1.5.1.2 "><p id="p99811123192420"><a name="p99811123192420"></a><a name="p99811123192420"></a>const std::string&amp;</p>
</td>
<td class="cellrowborder" valign="top" width="27.43%" headers="mcps1.1.5.1.3 "><p id="p7873319193113"><a name="p7873319193113"></a><a name="p7873319193113"></a>构建索引所需的配置文件，包含所有配置参数。</p>
</td>
<td class="cellrowborder" valign="top" width="29.349999999999998%" headers="mcps1.1.5.1.4 "><p id="p673671716253"><a name="p673671716253"></a><a name="p673671716253"></a>-</p>
</td>
</tr>
<tr id="row115518116154"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.1 "><p id="p7569116152"><a name="p7569116152"></a><a name="p7569116152"></a>training_threads</p>
</td>
<td class="cellrowborder" valign="top" width="18.22%" headers="mcps1.1.5.1.2 "><p id="p1456111121515"><a name="p1456111121515"></a><a name="p1456111121515"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="27.43%" headers="mcps1.1.5.1.3 "><p id="p20873519183110"><a name="p20873519183110"></a><a name="p20873519183110"></a>构建索引时的线程数。</p>
</td>
<td class="cellrowborder" valign="top" width="29.349999999999998%" headers="mcps1.1.5.1.4 "><p id="p849114441619"><a name="p849114441619"></a><a name="p849114441619"></a>大于等于1。</p>
</td>
</tr>
<tr id="row337943113413"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.1 "><p id="p45881149144115"><a name="p45881149144115"></a><a name="p45881149144115"></a>kmOpt</p>
</td>
<td class="cellrowborder" valign="top" width="18.22%" headers="mcps1.1.5.1.2 "><p id="p7588124944119"><a name="p7588124944119"></a><a name="p7588124944119"></a>GmmUtils::KMeansParams</p>
</td>
<td class="cellrowborder" valign="top" width="27.43%" headers="mcps1.1.5.1.3 "><p id="p0653162773111"><a name="p0653162773111"></a><a name="p0653162773111"></a>配置KMeans的调优参数。</p>
</td>
<td class="cellrowborder" valign="top" width="29.349999999999998%" headers="mcps1.1.5.1.4 "><p id="p9588174994118"><a name="p9588174994118"></a><a name="p9588174994118"></a>-</p>
</td>
</tr>
<tr id="row77062423410"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.1 "><p id="p10169105764218"><a name="p10169105764218"></a><a name="p10169105764218"></a>filter_thr</p>
</td>
<td class="cellrowborder" valign="top" width="18.22%" headers="mcps1.1.5.1.2 "><p id="p12169195710421"><a name="p12169195710421"></a><a name="p12169195710421"></a>float</p>
</td>
<td class="cellrowborder" valign="top" width="27.43%" headers="mcps1.1.5.1.3 "><p id="p1187361920317"><a name="p1187361920317"></a><a name="p1187361920317"></a>过滤阈值。</p>
</td>
<td class="cellrowborder" valign="top" width="29.349999999999998%" headers="mcps1.1.5.1.4 "><p id="p31691657164211"><a name="p31691657164211"></a><a name="p31691657164211"></a>[0, 1]，默认为0。</p>
</td>
</tr>
<tr id="row1170634212410"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.1 "><p id="p201696575428"><a name="p201696575428"></a><a name="p201696575428"></a>filter_type</p>
</td>
<td class="cellrowborder" valign="top" width="18.22%" headers="mcps1.1.5.1.2 "><p id="p3169135714212"><a name="p3169135714212"></a><a name="p3169135714212"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="27.43%" headers="mcps1.1.5.1.3 "><p id="p158731619133115"><a name="p158731619133115"></a><a name="p158731619133115"></a>过滤类型。</p>
</td>
<td class="cellrowborder" valign="top" width="29.349999999999998%" headers="mcps1.1.5.1.4 "><a name="ul9634542183819"></a><a name="ul9634542183819"></a><ul id="ul9634542183819"><li>0：根据向量中0的元素个数进行过滤。默认为0。</li><li>1：根据向量中各个数与均值偏差大小进行过滤。</li></ul>
</td>
</tr>
<tr id="row170634210411"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.1 "><p id="p13596320134313"><a name="p13596320134313"></a><a name="p13596320134313"></a>config_pbtxt</p>
</td>
<td class="cellrowborder" valign="top" width="18.22%" headers="mcps1.1.5.1.2 "><p id="p185960209431"><a name="p185960209431"></a><a name="p185960209431"></a>const std::string&amp;</p>
</td>
<td class="cellrowborder" valign="top" width="27.43%" headers="mcps1.1.5.1.3 "><p id="p14873171916311"><a name="p14873171916311"></a><a name="p14873171916311"></a>加载索引所需的配置文件。</p>
</td>
<td class="cellrowborder" valign="top" width="29.349999999999998%" headers="mcps1.1.5.1.4 "><p id="p1559632064314"><a name="p1559632064314"></a><a name="p1559632064314"></a>-</p>
</td>
</tr>
<tr id="row29007144439"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.1 "><p id="p959692094320"><a name="p959692094320"></a><a name="p959692094320"></a>scann_assets_pbtxt</p>
</td>
<td class="cellrowborder" valign="top" width="18.22%" headers="mcps1.1.5.1.2 "><p id="p25961720154320"><a name="p25961720154320"></a><a name="p25961720154320"></a>const std::string&amp;</p>
</td>
<td class="cellrowborder" valign="top" width="27.43%" headers="mcps1.1.5.1.3 "><p id="p198731419173117"><a name="p198731419173117"></a><a name="p198731419173117"></a>索引文件列表。</p>
</td>
<td class="cellrowborder" valign="top" width="29.349999999999998%" headers="mcps1.1.5.1.4 "><p id="p18596220194314"><a name="p18596220194314"></a><a name="p18596220194314"></a>-</p>
</td>
</tr>
</tbody>
</table>

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
<table><thead align="left"><tr id="row162653455531"><th class="cellrowborder" valign="top" id="mcps1.2.6.1.1"><p id="p1226544585317"><a name="p1226544585317"></a><a name="p1226544585317"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" id="mcps1.2.6.1.2"><p id="p19265134505310"><a name="p19265134505310"></a><a name="p19265134505310"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" id="mcps1.2.6.1.3"><p id="p42651745195310"><a name="p42651745195310"></a><a name="p42651745195310"></a>描述</p>
</th>
<th class="cellrowborder" colspan="2" valign="top" id="mcps1.2.6.1.4"><p id="p1626514513535"><a name="p1626514513535"></a><a name="p1626514513535"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row526514575318"><td class="cellrowborder" valign="top" headers="mcps1.2.6.1.1 "><p id="p69229577539"><a name="p69229577539"></a><a name="p69229577539"></a>iter</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.6.1.2 "><p id="p626584585315"><a name="p626584585315"></a><a name="p626584585315"></a>int32_t</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.6.1.3 "><p id="p3549223185415"><a name="p3549223185415"></a><a name="p3549223185415"></a>表示K-Means算法的迭代次数。</p>
</td>
<td class="cellrowborder" colspan="2" valign="top" headers="mcps1.2.6.1.4 "><p id="p1173013114573"><a name="p1173013114573"></a><a name="p1173013114573"></a>[0, MAXINT]，默认为0。</p>
</td>
</tr>
<tr id="row5265184515532"><td class="cellrowborder" valign="top" headers="mcps1.2.6.1.1 "><p id="p89221557105310"><a name="p89221557105310"></a><a name="p89221557105310"></a>sample</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.6.1.2 "><p id="p202651745135315"><a name="p202651745135315"></a><a name="p202651745135315"></a>int32_t</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.6.1.3 "><p id="p1726518459535"><a name="p1726518459535"></a><a name="p1726518459535"></a>表示采样子集的大小。</p>
</td>
<td class="cellrowborder" colspan="2" valign="top" headers="mcps1.2.6.1.4 "><p id="p626524545310"><a name="p626524545310"></a><a name="p626524545310"></a>-</p>
</td>
</tr>
<tr id="row62651045135319"><td class="cellrowborder" valign="top" headers="mcps1.2.6.1.1 "><p id="p992265755314"><a name="p992265755314"></a><a name="p992265755314"></a>init</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.6.1.2 "><p id="p02651458531"><a name="p02651458531"></a><a name="p02651458531"></a>int32_t</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.6.1.3 "><p id="p8455136115412"><a name="p8455136115412"></a><a name="p8455136115412"></a>表示K-Means聚类中心的初始化方式。</p>
</td>
<td class="cellrowborder" colspan="2" valign="top" headers="mcps1.2.6.1.4 "><p id="p5728161415020"><a name="p5728161415020"></a><a name="p5728161415020"></a>{0,1,2,3}，默认为0。</p>
<a name="ul4248355772"></a><a name="ul4248355772"></a><ul id="ul4248355772"><li>1：基于“平均距离”初始化。</li><li>2：K-Means++初始化。</li><li>3：随机初始化。</li><li>0：不开启PQ中KMeans优化。</li></ul>
</td>
</tr>
</tbody>
</table>

“config“由create\_config.py结合如[**表 2** 参数说明](#参数说明)所示的参数生成。

**表 2** 参数说明<a id="参数说明"></a>

<a name="table7549205762512"></a>
<table><thead align="left"><tr id="row12550185792516"><th class="cellrowborder" valign="top" id="mcps1.2.6.1.1"><p id="p4550185711256"><a name="p4550185711256"></a><a name="p4550185711256"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" id="mcps1.2.6.1.2"><p id="p3550657142514"><a name="p3550657142514"></a><a name="p3550657142514"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" id="mcps1.2.6.1.3"><p id="p1955035716253"><a name="p1955035716253"></a><a name="p1955035716253"></a>描述</p>
</th>
<th class="cellrowborder" colspan="2" valign="top" id="mcps1.2.6.1.4"><p id="p455055792519"><a name="p455055792519"></a><a name="p455055792519"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row355045722520"><td class="cellrowborder" valign="top" headers="mcps1.2.6.1.1 "><p id="p855015715254"><a name="p855015715254"></a><a name="p855015715254"></a>n_leaves</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.6.1.2 "><p id="p1555015772516"><a name="p1555015772516"></a><a name="p1555015772516"></a>int</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.6.1.3 "><p id="p182303331508"><a name="p182303331508"></a><a name="p182303331508"></a>IVF分区总子空间个数。</p>
</td>
<td class="cellrowborder" colspan="2" valign="top" headers="mcps1.2.6.1.4 "><p id="p1755015742513"><a name="p1755015742513"></a><a name="p1755015742513"></a>大于等于1。</p>
</td>
</tr>
<tr id="row1550157142516"><td class="cellrowborder" valign="top" headers="mcps1.2.6.1.1 "><p id="p19550145719251"><a name="p19550145719251"></a><a name="p19550145719251"></a>nb</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.6.1.2 "><p id="p19550195711253"><a name="p19550195711253"></a><a name="p19550195711253"></a>int32_t</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.6.1.3 "><p id="p8550657202516"><a name="p8550657202516"></a><a name="p8550657202516"></a>底库向量的数量。</p>
</td>
<td class="cellrowborder" colspan="2" valign="top" headers="mcps1.2.6.1.4 "><p id="p99161199328"><a name="p99161199328"></a><a name="p99161199328"></a>限制与dataset的长度保持一致，其中<span class="parmname" id="parmname9916161915320"><a name="parmname9916161915320"></a><a name="parmname9916161915320"></a>“dataset”</span>表示底库向量。</p>
</td>
</tr>
<tr id="row8550145715257"><td class="cellrowborder" valign="top" headers="mcps1.2.6.1.1 "><p id="p855018571256"><a name="p855018571256"></a><a name="p855018571256"></a>metricType</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.6.1.2 "><p id="p165501057132518"><a name="p165501057132518"></a><a name="p165501057132518"></a>std::string</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.6.1.3 "><p id="p1455045715254"><a name="p1455045715254"></a><a name="p1455045715254"></a>向量的距离类型。</p>
</td>
<td class="cellrowborder" colspan="2" valign="top" headers="mcps1.2.6.1.4 "><p id="p1638804911017"><a name="p1638804911017"></a><a name="p1638804911017"></a><span class="parmvalue" id="parmvalue17469332116"><a name="parmvalue17469332116"></a><a name="parmvalue17469332116"></a>“dot_product”</span>或<span class="parmvalue" id="parmvalue12906641919"><a name="parmvalue12906641919"></a><a name="parmvalue12906641919"></a>“squared_l2”</span></p>
</td>
</tr>
<tr id="row7550657172510"><td class="cellrowborder" valign="top" headers="mcps1.2.6.1.1 "><p id="p2055015710250"><a name="p2055015710250"></a><a name="p2055015710250"></a>dims_per_block</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.6.1.2 "><p id="p1955045732516"><a name="p1955045732516"></a><a name="p1955045732516"></a>int</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.6.1.3 "><p id="p1283214411428"><a name="p1283214411428"></a><a name="p1283214411428"></a>PQ量化合并维度数。</p>
</td>
<td class="cellrowborder" colspan="2" valign="top" headers="mcps1.2.6.1.4 "><p id="p1324334517220"><a name="p1324334517220"></a><a name="p1324334517220"></a>[1, dim]，其中<span class="parmname" id="parmname318945793312"><a name="parmname318945793312"></a><a name="parmname318945793312"></a>“dim”</span>表示底库向量的维度。</p>
</td>
</tr>
<tr id="row1179242714263"><td class="cellrowborder" valign="top" headers="mcps1.2.6.1.1 "><p id="p8792827102618"><a name="p8792827102618"></a><a name="p8792827102618"></a>avq_threshold</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.6.1.2 "><p id="p17792627142619"><a name="p17792627142619"></a><a name="p17792627142619"></a>float</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.6.1.3 "><p id="p6832184114220"><a name="p6832184114220"></a><a name="p6832184114220"></a>不对称分桶参数，仅对L2（squared_l2）数据集生效。</p>
</td>
<td class="cellrowborder" colspan="2" valign="top" headers="mcps1.2.6.1.4 "><p id="p14557151711313"><a name="p14557151711313"></a><a name="p14557151711313"></a>[0,1]</p>
</td>
</tr>
<tr id="row16263203214267"><td class="cellrowborder" valign="top" headers="mcps1.2.6.1.1 "><p id="p426411321264"><a name="p426411321264"></a><a name="p426411321264"></a>dim</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.6.1.2 "><p id="p19264193211265"><a name="p19264193211265"></a><a name="p19264193211265"></a>int32_t</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.6.1.3 "><p id="p0264113222612"><a name="p0264113222612"></a><a name="p0264113222612"></a>底库向量的维度。</p>
</td>
<td class="cellrowborder" colspan="2" valign="top" headers="mcps1.2.6.1.4 "><p id="p22171321183117"><a name="p22171321183117"></a><a name="p22171321183117"></a>限制与dataset的维度保持一致，其中<span class="parmname" id="parmname1821442115495"><a name="parmname1821442115495"></a><a name="parmname1821442115495"></a>“dataset”</span>表示底库向量。</p>
</td>
</tr>
<tr id="row1101335202619"><td class="cellrowborder" valign="top" headers="mcps1.2.6.1.1 "><p id="p20101435132615"><a name="p20101435132615"></a><a name="p20101435132615"></a>topK</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.6.1.2 "><p id="p16101103572618"><a name="p16101103572618"></a><a name="p16101103572618"></a>int</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.6.1.3 "><p id="p8101435162614"><a name="p8101435162614"></a><a name="p8101435162614"></a>最终返回结果数量。</p>
</td>
<td class="cellrowborder" colspan="2" valign="top" headers="mcps1.2.6.1.4 "><p id="p1253792318317"><a name="p1253792318317"></a><a name="p1253792318317"></a>大于等于1。</p>
</td>
</tr>
<tr id="row89363711267"><td class="cellrowborder" valign="top" headers="mcps1.2.6.1.1 "><p id="p8931137182616"><a name="p8931137182616"></a><a name="p8931137182616"></a>soar_lambda</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.6.1.2 "><p id="p993183720267"><a name="p993183720267"></a><a name="p993183720267"></a>float</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.6.1.3 "><p id="p01381144803"><a name="p01381144803"></a><a name="p01381144803"></a>控制正交性的参数，仅对IP（dot product）数据集生效。</p>
</td>
<td class="cellrowborder" colspan="2" valign="top" headers="mcps1.2.6.1.4 "><p id="p113817441403"><a name="p113817441403"></a><a name="p113817441403"></a>大于0，当值为<span class="parmvalue" id="parmvalue13682293485"><a name="parmvalue13682293485"></a><a name="parmvalue13682293485"></a>“-1”</span>时表示不开启此参数。</p>
</td>
</tr>
<tr id="row10622183992617"><td class="cellrowborder" valign="top" headers="mcps1.2.6.1.1 "><p id="p1362283942612"><a name="p1362283942612"></a><a name="p1362283942612"></a>overretrieve_factor</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.6.1.2 "><p id="p1162214391266"><a name="p1162214391266"></a><a name="p1162214391266"></a>float</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.6.1.3 "><p id="p1338813492019"><a name="p1338813492019"></a><a name="p1338813492019"></a>指定过检索因子，与<span class="parmname" id="parmname1866619242116"><a name="parmname1866619242116"></a><a name="parmname1866619242116"></a>“soar_lambda”</span>一起使用，仅对IP（dot_product）数据集生效。</p>
</td>
<td class="cellrowborder" colspan="2" valign="top" headers="mcps1.2.6.1.4 "><p id="p538819491606"><a name="p538819491606"></a><a name="p538819491606"></a>[1,2]，当值为<span class="parmvalue" id="parmvalue5851133124814"><a name="parmvalue5851133124814"></a><a name="parmvalue5851133124814"></a>“-1”</span>时表示不开启此参数。</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **说明：** 
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
<table><thead align="left"><tr id="row1569152711463"><th class="cellrowborder" valign="top" width="34.599999999999994%" id="mcps1.1.3.1.1"><p id="p146911527174618"><a name="p146911527174618"></a><a name="p146911527174618"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="65.4%" id="mcps1.1.3.1.2"><p id="p136911627194618"><a name="p136911627194618"></a><a name="p136911627194618"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row769192744612"><td class="cellrowborder" valign="top" width="34.599999999999994%" headers="mcps1.1.3.1.1 "><p id="p106910272463"><a name="p106910272463"></a><a name="p106910272463"></a>Status</p>
</td>
<td class="cellrowborder" valign="top" width="65.4%" headers="mcps1.1.3.1.2 "><p id="p14195191116393"><a name="p14195191116393"></a><a name="p14195191116393"></a>表示方法执行状态，通过status.ok()判断是否成功。</p>
</td>
</tr>
</tbody>
</table>

### SerializeToMemory

**接口定义<a name="section172317194488"></a>**

int ScannInterface::SerializeToMemory\(uint8\_t\*& dataPtr, size\_t& Length\);

**接口用途<a name="section1153124784912"></a>**

将索引序列化储存在内存中，内存长度为Length字节，起始地址为dataPtr（相比开源算法新增方法）。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="14.97%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="15.409999999999998%" id="mcps1.1.5.1.2"><p id="p73401941182314"><a name="p73401941182314"></a><a name="p73401941182314"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="35.67%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="33.95%" id="mcps1.1.5.1.4"><p id="p232514861412"><a name="p232514861412"></a><a name="p232514861412"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="14.97%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>dataPtr</p>
</td>
<td class="cellrowborder" valign="top" width="15.409999999999998%" headers="mcps1.1.5.1.2 "><p id="p1853984510229"><a name="p1853984510229"></a><a name="p1853984510229"></a>uint8_t*&amp;</p>
</td>
<td class="cellrowborder" valign="top" width="35.67%" headers="mcps1.1.5.1.3 "><p id="p1551821410413"><a name="p1551821410413"></a><a name="p1551821410413"></a>指向存储序列化数据的内存的起始地址。</p>
</td>
<td class="cellrowborder" valign="top" width="33.95%" headers="mcps1.1.5.1.4 "><p id="p2223102401510"><a name="p2223102401510"></a><a name="p2223102401510"></a>限制为空指针。</p>
</td>
</tr>
<tr id="row11230173385019"><td class="cellrowborder" valign="top" width="14.97%" headers="mcps1.1.5.1.1 "><p id="p6412202812239"><a name="p6412202812239"></a><a name="p6412202812239"></a>Length</p>
</td>
<td class="cellrowborder" valign="top" width="15.409999999999998%" headers="mcps1.1.5.1.2 "><p id="p1278518581195"><a name="p1278518581195"></a><a name="p1278518581195"></a>size_t&amp;</p>
</td>
<td class="cellrowborder" valign="top" width="35.67%" headers="mcps1.1.5.1.3 "><p id="p27308382419"><a name="p27308382419"></a><a name="p27308382419"></a>存储序列化数据的内存的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="33.95%" headers="mcps1.1.5.1.4 "><p id="p9223152491519"><a name="p9223152491519"></a><a name="p9223152491519"></a>限制为0。</p>
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
<td class="cellrowborder" valign="top" width="65.4%" headers="mcps1.1.3.1.2 "><p id="p14195191116393"><a name="p14195191116393"></a><a name="p14195191116393"></a>执行成功返回0，否则返回-1。</p>
</td>
</tr>
</tbody>
</table>

### LoadFromMemory

**接口定义<a name="section172317194488"></a>**

int ScannInterface::LoadFromMemory\(uint8\_t\*& dataPtr, size\_t& Length\);

**接口用途<a name="section1153124784912"></a>**

从内存中还原索引实例（相比开源算法新增方法）。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="16.97%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.540000000000001%" id="mcps1.1.5.1.2"><p id="p73401941182314"><a name="p73401941182314"></a><a name="p73401941182314"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="34.54%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="33.95%" id="mcps1.1.5.1.4"><p id="p232514861412"><a name="p232514861412"></a><a name="p232514861412"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="16.97%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>dataPtr</p>
</td>
<td class="cellrowborder" valign="top" width="14.540000000000001%" headers="mcps1.1.5.1.2 "><p id="p1853984510229"><a name="p1853984510229"></a><a name="p1853984510229"></a>uint8_t*&amp;</p>
</td>
<td class="cellrowborder" valign="top" width="34.54%" headers="mcps1.1.5.1.3 "><p id="p1551821410413"><a name="p1551821410413"></a><a name="p1551821410413"></a>指向存储序列化数据的内存的起始地址。</p>
</td>
<td class="cellrowborder" valign="top" width="33.95%" headers="mcps1.1.5.1.4 "><p id="p2223102401510"><a name="p2223102401510"></a><a name="p2223102401510"></a>限制为非空指针。</p>
</td>
</tr>
<tr id="row11230173385019"><td class="cellrowborder" valign="top" width="16.97%" headers="mcps1.1.5.1.1 "><p id="p6412202812239"><a name="p6412202812239"></a><a name="p6412202812239"></a>Length</p>
</td>
<td class="cellrowborder" valign="top" width="14.540000000000001%" headers="mcps1.1.5.1.2 "><p id="p1278518581195"><a name="p1278518581195"></a><a name="p1278518581195"></a>size_t&amp;</p>
</td>
<td class="cellrowborder" valign="top" width="34.54%" headers="mcps1.1.5.1.3 "><p id="p27308382419"><a name="p27308382419"></a><a name="p27308382419"></a>存储序列化数据的内存的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="33.95%" headers="mcps1.1.5.1.4 "><p id="p9223152491519"><a name="p9223152491519"></a><a name="p9223152491519"></a>限制为非0。</p>
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
<td class="cellrowborder" valign="top" width="65.4%" headers="mcps1.1.3.1.2 "><p id="p14195191116393"><a name="p14195191116393"></a><a name="p14195191116393"></a>执行成功返回0，否则返回-1。</p>
</td>
</tr>
</tbody>
</table>

### GetNum

**接口定义<a name="section172317194488"></a>**

int GetNum\(\) const;

**接口用途<a name="section1153124784912"></a>**

返回底库向量的数量（相比开源算法新增方法）。

**参数说明<a name="section157501312135019"></a>**

无入参。

**返回值<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>
<table><thead align="left"><tr id="row1569152711463"><th class="cellrowborder" valign="top" width="29.509999999999998%" id="mcps1.1.3.1.1"><p id="p146911527174618"><a name="p146911527174618"></a><a name="p146911527174618"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="70.49%" id="mcps1.1.3.1.2"><p id="p136911627194618"><a name="p136911627194618"></a><a name="p136911627194618"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row769192744612"><td class="cellrowborder" valign="top" width="29.509999999999998%" headers="mcps1.1.3.1.1 "><p id="p106910272463"><a name="p106910272463"></a><a name="p106910272463"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="70.49%" headers="mcps1.1.3.1.2 "><p id="p790415573313"><a name="p790415573313"></a><a name="p790415573313"></a>返回底库向量的数量。</p>
</td>
</tr>
</tbody>
</table>

### GetDim

**接口定义<a name="section172317194488"></a>**

int GetDim\(\) const;

**接口用途<a name="section1153124784912"></a>**

返回底库向量的维度（相比开源算法新增方法）。

**参数说明<a name="section157501312135019"></a>**

无入参。

**返回值<a name="section11100202063420"></a>**

<a name="table1690172718466"></a>
<table><thead align="left"><tr id="row1569152711463"><th class="cellrowborder" valign="top" width="29.509999999999998%" id="mcps1.1.3.1.1"><p id="p146911527174618"><a name="p146911527174618"></a><a name="p146911527174618"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="70.49%" id="mcps1.1.3.1.2"><p id="p136911627194618"><a name="p136911627194618"></a><a name="p136911627194618"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row769192744612"><td class="cellrowborder" valign="top" width="29.509999999999998%" headers="mcps1.1.3.1.1 "><p id="p106910272463"><a name="p106910272463"></a><a name="p106910272463"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="70.49%" headers="mcps1.1.3.1.2 "><p id="p790415573313"><a name="p790415573313"></a><a name="p790415573313"></a>返回底库向量的维度。</p>
</td>
</tr>
</tbody>
</table>
