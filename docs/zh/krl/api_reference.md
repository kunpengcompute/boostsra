# API参考

## 接口列表

KRL提供的接口如[**表 1** KRL提供的接口](#KRL提供的接口)所示。

**表 1** KRL提供的接口<a id="KRL提供的接口"></a>

<a name="table1194910128449"></a>
<table><thead align="left"><tr id="row99491812134412"><th class="cellrowborder" valign="top" width="13.059999999999999%" id="mcps1.2.4.1.1"><p id="p768563014173"><a name="p768563014173"></a><a name="p768563014173"></a>接口类型</p>
</th>
<th class="cellrowborder" valign="top" width="23.380000000000003%" id="mcps1.2.4.1.2"><p id="p1794951224415"><a name="p1794951224415"></a><a name="p1794951224415"></a>接口名称</p>
</th>
<th class="cellrowborder" valign="top" width="63.56%" id="mcps1.2.4.1.3"><p id="p6949612124415"><a name="p6949612124415"></a><a name="p6949612124415"></a>接口作用</p>
</th>
</tr>
</thead>
<tbody><tr id="row712018285575"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p1468583012176"><a name="p1468583012176"></a><a name="p1468583012176"></a>Handle类接口</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p8993524101814"><a name="p8993524101814"></a><a name="p8993524101814"></a>krl_create_distance_handle</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p14993924101811"><a name="p14993924101811"></a><a name="p14993924101811"></a>初始化构建一个KRLDistanceHandle实例，稠密距离计算时使用。</p>
</td>
</tr>
<tr id="row119491112174414"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p163141052196"><a name="p163141052196"></a><a name="p163141052196"></a>Handle类接口</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p175854912238"><a name="p175854912238"></a><a name="p175854912238"></a>krl_create_reorder_handle</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p09931024131816"><a name="p09931024131816"></a><a name="p09931024131816"></a>初始化构建一个KRLDistanceHandle实例，重排计算时使用。</p>
</td>
</tr>
<tr id="row9949131219443"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p831619512197"><a name="p831619512197"></a><a name="p831619512197"></a>Handle类接口</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p19936249184"><a name="p19936249184"></a><a name="p19936249184"></a>krl_clean_distance_handle</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p7729162612418"><a name="p7729162612418"></a><a name="p7729162612418"></a>析构KRLDistanceHandle实例，释放内存空间。</p>
</td>
</tr>
<tr id="row1594913120443"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p16317151193"><a name="p16317151193"></a><a name="p16317151193"></a>Handle类接口</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p799319246182"><a name="p799319246182"></a><a name="p799319246182"></a>krl_create_LUT8b_handle</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p7993122417187"><a name="p7993122417187"></a><a name="p7993122417187"></a>初始化构建一个KRLLUT8bHandle实例，8bit查表累和时使用。</p>
</td>
</tr>
<tr id="row6949131274416"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p13180551910"><a name="p13180551910"></a><a name="p13180551910"></a>Handle类接口</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p12993324191819"><a name="p12993324191819"></a><a name="p12993324191819"></a>krl_clean_LUT8b_handle</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p139801643145818"><a name="p139801643145818"></a><a name="p139801643145818"></a>析构KRLLUT8bHandle实例，释放内存空间。</p>
</td>
</tr>
<tr id="row13975184141820"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p531917514195"><a name="p531917514195"></a><a name="p531917514195"></a>Handle类接口</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p7975114191820"><a name="p7975114191820"></a><a name="p7975114191820"></a>krl_get_idx_pointer</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p192601719115616"><a name="p192601719115616"></a><a name="p192601719115616"></a>获取KRLLUT8bHandle实例中存储的需要计算的底库向量ID。</p>
</td>
</tr>
<tr id="row1682414614182"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p183211558190"><a name="p183211558190"></a><a name="p183211558190"></a>Handle类接口</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p621722142419"><a name="p621722142419"></a><a name="p621722142419"></a>krl_get_dist_pointer</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p2824164621814"><a name="p2824164621814"></a><a name="p2824164621814"></a>获取KRLLUT8bHandle实例中存储的距离数组首地址，在调用查表累和计算算子之前为随机数，调用之后为计算得到的距离。</p>
</td>
</tr>
<tr id="row891194810189"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p6685230201716"><a name="p6685230201716"></a><a name="p6685230201716"></a>距离计算接口</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p12911154891819"><a name="p12911154891819"></a><a name="p12911154891819"></a>krl_L2sqr</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p5911184810186"><a name="p5911184810186"></a><a name="p5911184810186"></a>进行数据类型为float的一对一欧氏距离计算。</p>
</td>
</tr>
<tr id="row1710165116183"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p120601371911"><a name="p120601371911"></a><a name="p120601371911"></a>距离计算接口</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p710165111184"><a name="p710165111184"></a><a name="p710165111184"></a>krl_L2sqr_f16f32</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p1693388205916"><a name="p1693388205916"></a><a name="p1693388205916"></a>进行数据类型为fp16的一对一欧氏距离计算。</p>
</td>
</tr>
<tr id="row490119533188"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p14208191316192"><a name="p14208191316192"></a><a name="p14208191316192"></a>距离计算接口</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p179011053151819"><a name="p179011053151819"></a><a name="p179011053151819"></a>krl_L2sqr_u8u32</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p790155315187"><a name="p790155315187"></a><a name="p790155315187"></a>进行数据类型为uint8的一对一欧氏距离计算。</p>
</td>
</tr>
<tr id="row1785925518184"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p11209713131919"><a name="p11209713131919"></a><a name="p11209713131919"></a>距离计算接口</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p4860165531811"><a name="p4860165531811"></a><a name="p4860165531811"></a>krl_ipdis</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p158609551186"><a name="p158609551186"></a><a name="p158609551186"></a>进行数据类型为float的一对一内积距离计算。</p>
</td>
</tr>
<tr id="row197613573181"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p321121341919"><a name="p321121341919"></a><a name="p321121341919"></a>距离计算接口</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p5761135713185"><a name="p5761135713185"></a><a name="p5761135713185"></a>krl_negative_ipdis_f16f32</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p20381543012"><a name="p20381543012"></a><a name="p20381543012"></a>进行数据类型为fp16的一对一内积距离计算。</p>
</td>
</tr>
<tr id="row2030213041919"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p521251381911"><a name="p521251381911"></a><a name="p521251381911"></a>距离计算接口</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p15619557252"><a name="p15619557252"></a><a name="p15619557252"></a>krl_negative_ipdis_s8s32</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p17303140191918"><a name="p17303140191918"></a><a name="p17303140191918"></a>进行数据类型为int8的一对一内积距离计算。</p>
</td>
</tr>
<tr id="row238412241914"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p15213213161920"><a name="p15213213161920"></a><a name="p15213213161920"></a>距离计算接口</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p1138418201911"><a name="p1138418201911"></a><a name="p1138418201911"></a>krl_L2sqr_by_idx</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p203841126192"><a name="p203841126192"></a><a name="p203841126192"></a>进行数据类型为float的一对多欧氏距离计算。</p>
</td>
</tr>
<tr id="row0391358193"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p192142139194"><a name="p192142139194"></a><a name="p192142139194"></a>距离计算接口</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p2725181712253"><a name="p2725181712253"></a><a name="p2725181712253"></a>krl_L2sqr_by_idx_f16f32</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p133913511915"><a name="p133913511915"></a><a name="p133913511915"></a>进行数据类型为fp16的一对多欧氏距离计算。</p>
</td>
</tr>
<tr id="row151611671195"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p12215201391920"><a name="p12215201391920"></a><a name="p12215201391920"></a>距离计算接口</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p20161197101911"><a name="p20161197101911"></a><a name="p20161197101911"></a>krl_L2sqr_by_idx_u8f32</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p1616177151919"><a name="p1616177151919"></a><a name="p1616177151919"></a>进行数据类型为uint8的一对多欧氏距离计算。</p>
</td>
</tr>
<tr id="row5354120161911"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p321691321913"><a name="p321691321913"></a><a name="p321691321913"></a>距离计算接口</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p0354420111913"><a name="p0354420111913"></a><a name="p0354420111913"></a>krl_inner_product_by_idx</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p2354132010196"><a name="p2354132010196"></a><a name="p2354132010196"></a>进行数据类型为float的一对多内积距离计算。</p>
</td>
</tr>
<tr id="row1423643420194"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p221741341915"><a name="p221741341915"></a><a name="p221741341915"></a>距离计算接口</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p5233173872520"><a name="p5233173872520"></a><a name="p5233173872520"></a>krl_inner_product_by_idx_f16f32</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p5236113431915"><a name="p5236113431915"></a><a name="p5236113431915"></a>进行数据类型为fp16的一对多内积距离计算。</p>
</td>
</tr>
<tr id="row1792738101914"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p10218111381917"><a name="p10218111381917"></a><a name="p10218111381917"></a>距离计算接口</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p18810342182514"><a name="p18810342182514"></a><a name="p18810342182514"></a>krl_negative_inner_product_by_idx_f16f32</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p27921838121916"><a name="p27921838121916"></a><a name="p27921838121916"></a>进行数据类型为fp16的一对多内积距离计算，对结果取反。</p>
</td>
</tr>
<tr id="row7651940121918"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p32191513101918"><a name="p32191513101918"></a><a name="p32191513101918"></a>距离计算接口</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p186516406195"><a name="p186516406195"></a><a name="p186516406195"></a>krl_inner_product_by_idx_s8f32</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p196511640121916"><a name="p196511640121916"></a><a name="p196511640121916"></a>进行数据类型为int8的一对多内积距离计算。</p>
</td>
</tr>
<tr id="row283274219196"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p822001319194"><a name="p822001319194"></a><a name="p822001319194"></a>距离计算接口</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p383264213197"><a name="p383264213197"></a><a name="p383264213197"></a>krl_L2sqr_ny</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p168329424199"><a name="p168329424199"></a><a name="p168329424199"></a>进行数据类型为float的一对多欧氏距离计算。</p>
</td>
</tr>
<tr id="row47661344161914"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p1922131381913"><a name="p1922131381913"></a><a name="p1922131381913"></a>距离计算接口</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p207661044101919"><a name="p207661044101919"></a><a name="p207661044101919"></a>krl_L2sqr_ny_f16f32</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p1176710447191"><a name="p1176710447191"></a><a name="p1176710447191"></a>进行数据类型为fp16的一对多欧氏距离计算。</p>
</td>
</tr>
<tr id="row0904184681920"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p112221813111918"><a name="p112221813111918"></a><a name="p112221813111918"></a>距离计算接口</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p1090416468197"><a name="p1090416468197"></a><a name="p1090416468197"></a>krl_L2sqr_ny_u8f32</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p19047462196"><a name="p19047462196"></a><a name="p19047462196"></a>进行数据类型为uint8的一对多欧氏距离计算。</p>
</td>
</tr>
<tr id="row1149011486191"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p222361351918"><a name="p222361351918"></a><a name="p222361351918"></a>距离计算接口</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p9490144814199"><a name="p9490144814199"></a><a name="p9490144814199"></a>krl_L2sqr_ny_with_handle</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p64901848191916"><a name="p64901848191916"></a><a name="p64901848191916"></a>进行数据类型为float的一对多欧氏距离计算，底库向量与维度存储于Handle中。</p>
</td>
</tr>
<tr id="row221135114193"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p15224131313192"><a name="p15224131313192"></a><a name="p15224131313192"></a>距离计算接口</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p13221351171919"><a name="p13221351171919"></a><a name="p13221351171919"></a>krl_inner_product_ny</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p1022851141912"><a name="p1022851141912"></a><a name="p1022851141912"></a>进行数据类型为float的一对多内积距离计算。</p>
</td>
</tr>
<tr id="row1670318531197"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p022551361914"><a name="p022551361914"></a><a name="p022551361914"></a>距离计算接口</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p370305310196"><a name="p370305310196"></a><a name="p370305310196"></a>krl_inner_product_ny_f16f32</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p1570335316191"><a name="p1570335316191"></a><a name="p1570335316191"></a>进行数据类型为fp16的一对多内积距离计算。</p>
</td>
</tr>
<tr id="row1659115614196"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p222621316199"><a name="p222621316199"></a><a name="p222621316199"></a>距离计算接口</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p05910561199"><a name="p05910561199"></a><a name="p05910561199"></a>krl_inner_product_ny_s8f32</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p135911256161914"><a name="p135911256161914"></a><a name="p135911256161914"></a>进行数据类型为int8的一对多内积距离计算。</p>
</td>
</tr>
<tr id="row86397594196"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p11227813101917"><a name="p11227813101917"></a><a name="p11227813101917"></a>距离计算接口</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p2640125961913"><a name="p2640125961913"></a><a name="p2640125961913"></a>krl_inner_product_ny_with_handle</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p8640159201914"><a name="p8640159201914"></a><a name="p8640159201914"></a>进行数据类型为float的一对多内积距离计算，底库向量与维度存储于Handle中。</p>
</td>
</tr>
<tr id="row166751616206"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p206851730131710"><a name="p206851730131710"></a><a name="p206851730131710"></a>8bit查表累和接口</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p196762119202"><a name="p196762119202"></a><a name="p196762119202"></a>krl_table_lookup_8b_f32</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p126761515204"><a name="p126761515204"></a><a name="p126761515204"></a>使用8bit索引在float类型表项中查询距离并累和，将累和结果加上dis0后存入distance。</p>
</td>
</tr>
<tr id="row1380243132018"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p3506620151918"><a name="p3506620151918"></a><a name="p3506620151918"></a>8bit查表累和接口</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p28034302020"><a name="p28034302020"></a><a name="p28034302020"></a>krl_table_lookup_8b_f32_by_idx</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p4803034206"><a name="p4803034206"></a><a name="p4803034206"></a>使用8bit索引在float类型表项中查询距离并累和，将累和结果加上dis0后存入distance。ID在idx数组中出现的底库向量结果才会参与计算。</p>
</td>
</tr>
<tr id="row13704145182016"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p45071220161916"><a name="p45071220161916"></a><a name="p45071220161916"></a>8bit查表累和接口</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p270425132019"><a name="p270425132019"></a><a name="p270425132019"></a>krl_table_lookup_8b_f32_with_handle</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p27041512013"><a name="p27041512013"></a><a name="p27041512013"></a>使用8bit索引在float类型表项中查询距离并累和，将累和结果加上dis0后存入distance。idx数组与distance数组被包含在KRLLUT8bHandle实例中，ID在idx数组中出现的底库向量结果才会参与计算。</p>
</td>
</tr>
<tr id="row1040647122014"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p46851630141710"><a name="p46851630141710"></a><a name="p46851630141710"></a>4bit查表累和接口</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p12407197202019"><a name="p12407197202019"></a><a name="p12407197202019"></a>krl_fast_table_lookup_step</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p040757182014"><a name="p040757182014"></a><a name="p040757182014"></a>批量处理数据类型为float的查询向量的4bit查表累和过滤压缩算子。算子支持计算至多16个查询向量与32个底库向量间的距离。在距离计算完成后，将其与阈值进行比较，满足比较条件的底库向量的lt_mask对应位置将会设置为1，反之为0。</p>
</td>
</tr>
<tr id="row187412920207"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p1962812276198"><a name="p1962812276198"></a><a name="p1962812276198"></a>4bit查表累和接口</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p1332135182717"><a name="p1332135182717"></a><a name="p1332135182717"></a>krl_L2_table_lookup_fast_scan_bs64</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p1974249132015"><a name="p1974249132015"></a><a name="p1974249132015"></a>单独处理数据类型为float的查询向量的4比特查表累和过滤压缩算子。计算1个查询向量与64个底库向量间的欧氏距离。根据距离类型决定比较规则，将距离值满足比较规则的底库向量的lt_mask设置为1，反之为0。</p>
</td>
</tr>
<tr id="row10185812122010"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p1630327101916"><a name="p1630327101916"></a><a name="p1630327101916"></a>4bit查表累和接口</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p1618516126202"><a name="p1618516126202"></a><a name="p1618516126202"></a>krl_IP_table_lookup_fast_scan_bs64</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p2405162815416"><a name="p2405162815416"></a><a name="p2405162815416"></a>单独处理数据类型为float的查询向量的4比特查表累和过滤压缩算子。计算1个查询向量与64个底库向量间的内积距离。根据距离类型决定比较规则，将距离值满足比较规则的底库向量的lt_mask设置为1，反之为0。</p>
</td>
</tr>
<tr id="row17962171310208"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p3631162715196"><a name="p3631162715196"></a><a name="p3631162715196"></a>4bit查表累和接口</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p3585133102819"><a name="p3585133102819"></a><a name="p3585133102819"></a>krl_L2_table_lookup_fast_scan_bs96</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p18962121362013"><a name="p18962121362013"></a><a name="p18962121362013"></a>单独处理数据类型为float的查询向量的4比特查表累和过滤压缩算子。计算1个查询向量与96个底库向量间的欧氏距离。根据距离类型决定比较规则，将距离值满足比较规则的底库向量的lt_mask设置为1，反之为0。</p>
</td>
</tr>
<tr id="row39991716192015"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p56321127121916"><a name="p56321127121916"></a><a name="p56321127121916"></a>4bit查表累和接口</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p1999916102012"><a name="p1999916102012"></a><a name="p1999916102012"></a>krl_IP_table_lookup_fast_scan_bs96</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p8999816192019"><a name="p8999816192019"></a><a name="p8999816192019"></a>单独处理数据类型为float的查询向量的4比特查表累和过滤压缩算子。计算1个查询向量与96个底库向量间的内积距离。根据距离类型决定比较规则，将距离值满足比较规则的底库向量的lt_mask设置为1，反之为0。</p>
</td>
</tr>
<tr id="row879313188203"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p106331927191916"><a name="p106331927191916"></a><a name="p106331927191916"></a>4bit查表累和接口</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p979311816203"><a name="p979311816203"></a><a name="p979311816203"></a>krl_table_lookup_4b_f16</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p1479391832015"><a name="p1479391832015"></a><a name="p1479391832015"></a>单独处理数据类型为fp16的查询向量的4比特查表累和过滤压缩算子。计算1个查询向量与多个底库向量间的内积距离，距离的初始值为dis_f16。此接口不会进行过滤压缩（与阈值进行比较）。</p>
</td>
</tr>
<tr id="row54279217209"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p136351727111911"><a name="p136351727111911"></a><a name="p136351727111911"></a>4bit查表累和接口</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p1120132012282"><a name="p1120132012282"></a><a name="p1120132012282"></a>krl_pack_codes_4b</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p16427162162010"><a name="p16427162162010"></a><a name="p16427162162010"></a>单独处理数据类型为fp16的查询向量的4比特查表累和过滤压缩算子。计算1个查询向量与多个底库向量间的内积距离，距离的初始值为dis_f16。此接口不会进行过滤压缩（与阈值进行比较）。</p>
</td>
</tr>
<tr id="row2013422482018"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p18685113014176"><a name="p18685113014176"></a><a name="p18685113014176"></a>重排接口</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p5134202413207"><a name="p5134202413207"></a><a name="p5134202413207"></a>krl_reorder_2_vector</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p6358251857"><a name="p6358251857"></a><a name="p6358251857"></a>计算1个查询向量与多个不连续底库向量间的高精度距离并排序。</p>
</td>
</tr>
<tr id="row071714259208"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p1177182991910"><a name="p1177182991910"></a><a name="p1177182991910"></a>重排接口</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p671762518203"><a name="p671762518203"></a><a name="p671762518203"></a>krl_reorder_2_vector_continuous</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p157171825162016"><a name="p157171825162016"></a><a name="p157171825162016"></a>计算1个查询向量与多个连续底库向量间的高精度距离并排序。</p>
</td>
</tr>
<tr id="row101930282204"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p17685630131711"><a name="p17685630131711"></a><a name="p17685630131711"></a>保存/加载接口</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p619382822013"><a name="p619382822013"></a><a name="p619382822013"></a>krl_store_LUT8Handle</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p15193228102018"><a name="p15193228102018"></a><a name="p15193228102018"></a>将8bit查找表句柄保存到文件中。</p>
</td>
</tr>
<tr id="row418063172011"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p188531538101912"><a name="p188531538101912"></a><a name="p188531538101912"></a>保存/加载接口</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p4180133110202"><a name="p4180133110202"></a><a name="p4180133110202"></a>krl_build_LUT8Handle_fromfile</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p157004230511"><a name="p157004230511"></a><a name="p157004230511"></a>从文件中读取并重建8bit查找表句柄。</p>
</td>
</tr>
<tr id="row4520183315206"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p385513812191"><a name="p385513812191"></a><a name="p385513812191"></a>保存/加载接口</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p11520103311205"><a name="p11520103311205"></a><a name="p11520103311205"></a>krl_store_distanceHandle</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p952053342012"><a name="p952053342012"></a><a name="p952053342012"></a>将距离计算句柄保存到文件中。</p>
</td>
</tr>
<tr id="row514503519205"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p2856173821913"><a name="p2856173821913"></a><a name="p2856173821913"></a>保存/加载接口</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p3146835102018"><a name="p3146835102018"></a><a name="p3146835102018"></a>krl_build_distanceHandle_fromfile</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p144261417573"><a name="p144261417573"></a><a name="p144261417573"></a>从文件中读取并重建距离计算句柄。</p>
</td>
</tr>
</tbody>
</table>

## Handle类接口

### krl\_create\_distance\_handle

**接口定义<a name="section172317194488"></a>**

int krl\_create\_distance\_handle\(KRLDistanceHandle\*\* kdh, size\_t accu\_level, size\_t blocksize, size\_t codes\_num, size\_t dim, size\_t num\_base, int metric\_type, const uint8\_t\* codes, size\_t codes\_size\);

**接口用途<a name="section1153124784912"></a>**

初始化构建一个KRLDistanceHandle实例，稠密距离计算时使用。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.56155615561556%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.591459145914593%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>kdh</p>
</td>
<td class="cellrowborder" valign="top" width="14.591459145914593%" headers="mcps1.1.5.1.2 "><p id="p98931015893"><a name="p98931015893"></a><a name="p98931015893"></a>KRLDistanceHandle**</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p182303331508"><a name="p182303331508"></a><a name="p182303331508"></a>需要被初始化构建的KRLDistanceHandle指针。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>限制为非空指针，指向一个空指针。</p>
</td>
</tr>
<tr id="row11230173385019"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p22301333165015"><a name="p22301333165015"></a><a name="p22301333165015"></a>accu_level</p>
</td>
<td class="cellrowborder" valign="top" width="14.591459145914593%" headers="mcps1.1.5.1.2 "><p id="p5893141517919"><a name="p5893141517919"></a><a name="p5893141517919"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p10230433115013"><a name="p10230433115013"></a><a name="p10230433115013"></a>计算时的量化等级。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p77289581198"><a name="p77289581198"></a><a name="p77289581198"></a>[1,3]，取值表示不同的量化等级：</p>
<a name="ul164886121012"></a><a name="ul164886121012"></a><ul id="ul164886121012"><li>1：int8。</li><li>2：fp16。</li><li>3：fp32。</li></ul>
</td>
</tr>
<tr id="row1368063274610"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p116802032174613"><a name="p116802032174613"></a><a name="p116802032174613"></a>blocksize</p>
</td>
<td class="cellrowborder" valign="top" width="14.591459145914593%" headers="mcps1.1.5.1.2 "><p id="p489312151893"><a name="p489312151893"></a><a name="p489312151893"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p268013224617"><a name="p268013224617"></a><a name="p268013224617"></a>数据分块大小。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p6989158192510"><a name="p6989158192510"></a><a name="p6989158192510"></a>16或32或64。选择最大能除尽底库向量数量的分块。</p>
</td>
</tr>
<tr id="row8597534164617"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p4597734184616"><a name="p4597734184616"></a><a name="p4597734184616"></a>codes_num</p>
</td>
<td class="cellrowborder" valign="top" width="14.591459145914593%" headers="mcps1.1.5.1.2 "><p id="p178931015394"><a name="p178931015394"></a><a name="p178931015394"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p65975343465"><a name="p65975343465"></a><a name="p65975343465"></a>每个查询向量计算的底库向量数量。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p16989883251"><a name="p16989883251"></a><a name="p16989883251"></a>[1,2^30-1]</p>
</td>
</tr>
<tr id="row523013315504"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p10230123316509"><a name="p10230123316509"></a><a name="p10230123316509"></a>dim</p>
</td>
<td class="cellrowborder" valign="top" width="14.591459145914593%" headers="mcps1.1.5.1.2 "><p id="p2894215596"><a name="p2894215596"></a><a name="p2894215596"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p102301133105015"><a name="p102301133105015"></a><a name="p102301133105015"></a>向量维度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p296864410116"><a name="p296864410116"></a><a name="p296864410116"></a>[1,65535]</p>
</td>
</tr>
<tr id="row1523083315012"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p10230433105020"><a name="p10230433105020"></a><a name="p10230433105020"></a>num_base</p>
</td>
<td class="cellrowborder" valign="top" width="14.591459145914593%" headers="mcps1.1.5.1.2 "><p id="p15894141519917"><a name="p15894141519917"></a><a name="p15894141519917"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p623053365015"><a name="p623053365015"></a><a name="p623053365015"></a>单次处理的向量个数。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1946832961016"><a name="p1946832961016"></a><a name="p1946832961016"></a>[1,65535]</p>
</td>
</tr>
<tr id="row387211011106"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p2023791201011"><a name="p2023791201011"></a><a name="p2023791201011"></a>metric_type</p>
</td>
<td class="cellrowborder" valign="top" width="14.591459145914593%" headers="mcps1.1.5.1.2 "><p id="p198722006101"><a name="p198722006101"></a><a name="p198722006101"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p10237212111013"><a name="p10237212111013"></a><a name="p10237212111013"></a>距离度量类型。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p5904125914109"><a name="p5904125914109"></a><a name="p5904125914109"></a>[0,1]，取值表示不同的距离度量类型：</p>
<a name="ul396901541013"></a><a name="ul396901541013"></a><ul id="ul396901541013"><li>0：内积距离。</li><li>1：欧氏距离。</li></ul>
</td>
</tr>
<tr id="row7131153011107"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p1546185591017"><a name="p1546185591017"></a><a name="p1546185591017"></a>codes</p>
</td>
<td class="cellrowborder" valign="top" width="14.591459145914593%" headers="mcps1.1.5.1.2 "><p id="p19131103031011"><a name="p19131103031011"></a><a name="p19131103031011"></a>const uint8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p55461255161011"><a name="p55461255161011"></a><a name="p55461255161011"></a>底库向量（float）。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p213293001016"><a name="p213293001016"></a><a name="p213293001016"></a>限制长度为codes_size，其中<span class="parmname" id="parmname17671637191415"><a name="parmname17671637191415"></a><a name="parmname17671637191415"></a>“codes_size”</span>为底库向量codes的长度。</p>
</td>
</tr>
<tr id="row1351603315418"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p1151717330417"><a name="p1151717330417"></a><a name="p1151717330417"></a>codes_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.591459145914593%" headers="mcps1.1.5.1.2 "><p id="p351703319417"><a name="p351703319417"></a><a name="p351703319417"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p6517433144111"><a name="p6517433144111"></a><a name="p6517433144111"></a>底库向量codes的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p135171733184112"><a name="p135171733184112"></a><a name="p135171733184112"></a>num_base * codes_num * dim * 4，其中<span class="parmname" id="parmname8230125864315"><a name="parmname8230125864315"></a><a name="parmname8230125864315"></a>“num_base”</span>为单次处理的查询向量个数，<span class="parmname" id="parmname11230185824311"><a name="parmname11230185824311"></a><a name="parmname11230185824311"></a>“codes_num”</span>为每个查询向量计算的底库向量数量，<span class="parmname" id="parmname152302580436"><a name="parmname152302580436"></a><a name="parmname152302580436"></a>“dim”</span>为向量维度。</p>
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
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a>正常运行时返回0，异常退出返回对应错误码。</p>
</td>
</tr>
</tbody>
</table>

**使用示例**

```c
#include <stdio.h>
#include <stdlib.h>
#include <string.h>
#include "krl.h"

int main() {
    // 参数配置
    size_t dim = 128;           // 向量维度
    size_t num_base = 1;        // 单次处理的查询向量个数
    size_t codes_num = 1000;    // 底库向量数量
    size_t accu_level = 3;      // 量化等级
    size_t blocksize = 32;      // 数据分块大小（需能整除codes_num）
    int metric_type = 1;        // 欧氏距离

    // 准备底库向量数据
    size_t codes_size = num_base * codes_num * dim * sizeof(float);
    float* codes_data = (float*)malloc(codes_size);
    // ... 填充codes_data数据 ...

    // 创建Handle
    KRLDistanceHandle* kdh = NULL;
    int ret = krl_create_distance_handle(
        &kdh,
        accu_level,
        blocksize,
        codes_num,
        dim,
        num_base,
        metric_type,
        (const uint8_t*)codes_data,
        codes_size
    );

    if (ret != 0) {
        printf("创建Handle失败，错误码: %d\n", ret);
        free(codes_data);
        return -1;
    }

    printf("成功创建KRLDistanceHandle\n");

    // ... 使用kdh进行距离计算 ...

    // 清理资源
    krl_clean_distance_handle(&kdh);
    free(codes_data);

    return 0;
}
```

### krl\_create\_reorder\_handle

**接口定义<a name="section172317194488"></a>**

int krl\_create\_reorder\_handle\(KRLDistanceHandle\*\* kdh, size\_t accu\_level, size\_t full\_accu\_level, size\_t codes\_num, size\_t dim, int metric\_type, const uint8\_t\* codes, size\_t codes\_size\);

**接口用途<a name="section1153124784912"></a>**

初始化构建一个KRLDistanceHandle实例，重排计算时使用。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.56155615561556%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.591459145914593%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="30.29302930293029%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="39.55395539553955%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>kdh</p>
</td>
<td class="cellrowborder" valign="top" width="14.591459145914593%" headers="mcps1.1.5.1.2 "><p id="p98931015893"><a name="p98931015893"></a><a name="p98931015893"></a>KRLDistanceHandle**</p>
</td>
<td class="cellrowborder" valign="top" width="30.29302930293029%" headers="mcps1.1.5.1.3 "><p id="p182303331508"><a name="p182303331508"></a><a name="p182303331508"></a>需要被初始化构建的KRLDistanceHandle指针。</p>
</td>
<td class="cellrowborder" valign="top" width="39.55395539553955%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>限制为非空指针，指向一个空指针。</p>
</td>
</tr>
<tr id="row11230173385019"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p22301333165015"><a name="p22301333165015"></a><a name="p22301333165015"></a>accu_level</p>
</td>
<td class="cellrowborder" valign="top" width="14.591459145914593%" headers="mcps1.1.5.1.2 "><p id="p5893141517919"><a name="p5893141517919"></a><a name="p5893141517919"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="30.29302930293029%" headers="mcps1.1.5.1.3 "><p id="p10230433115013"><a name="p10230433115013"></a><a name="p10230433115013"></a>低精度粗排量化等级。</p>
</td>
<td class="cellrowborder" valign="top" width="39.55395539553955%" headers="mcps1.1.5.1.4 "><p id="p77289581198"><a name="p77289581198"></a><a name="p77289581198"></a>[1,3]，取值表示不同的量化等级：</p>
<a name="ul164886121012"></a><a name="ul164886121012"></a><ul id="ul164886121012"><li>1：int8。</li><li>2：fp16。</li><li>3：fp32。</li></ul>
</td>
</tr>
<tr id="row1368063274610"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p116802032174613"><a name="p116802032174613"></a><a name="p116802032174613"></a>full_accu_level</p>
</td>
<td class="cellrowborder" valign="top" width="14.591459145914593%" headers="mcps1.1.5.1.2 "><p id="p489312151893"><a name="p489312151893"></a><a name="p489312151893"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="30.29302930293029%" headers="mcps1.1.5.1.3 "><p id="p268013224617"><a name="p268013224617"></a><a name="p268013224617"></a>高精度重排量化等级。</p>
</td>
<td class="cellrowborder" valign="top" width="39.55395539553955%" headers="mcps1.1.5.1.4 "><p id="p11884449121914"><a name="p11884449121914"></a><a name="p11884449121914"></a>[1,3]，取值表示不同的量化等级：</p>
<a name="ul1588418498192"></a><a name="ul1588418498192"></a><ul id="ul1588418498192"><li>1：int8。</li><li>2：fp16。</li><li>3：fp32。</li></ul>
</td>
</tr>
<tr id="row8597534164617"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p4597734184616"><a name="p4597734184616"></a><a name="p4597734184616"></a>codes_num</p>
</td>
<td class="cellrowborder" valign="top" width="14.591459145914593%" headers="mcps1.1.5.1.2 "><p id="p178931015394"><a name="p178931015394"></a><a name="p178931015394"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="30.29302930293029%" headers="mcps1.1.5.1.3 "><p id="p65975343465"><a name="p65975343465"></a><a name="p65975343465"></a>每个查询向量计算的底库向量数量。</p>
</td>
<td class="cellrowborder" valign="top" width="39.55395539553955%" headers="mcps1.1.5.1.4 "><p id="p16989883251"><a name="p16989883251"></a><a name="p16989883251"></a>[1,2^30-1]</p>
</td>
</tr>
<tr id="row523013315504"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p10230123316509"><a name="p10230123316509"></a><a name="p10230123316509"></a>dim</p>
</td>
<td class="cellrowborder" valign="top" width="14.591459145914593%" headers="mcps1.1.5.1.2 "><p id="p2894215596"><a name="p2894215596"></a><a name="p2894215596"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="30.29302930293029%" headers="mcps1.1.5.1.3 "><p id="p102301133105015"><a name="p102301133105015"></a><a name="p102301133105015"></a>向量维度。</p>
</td>
<td class="cellrowborder" valign="top" width="39.55395539553955%" headers="mcps1.1.5.1.4 "><p id="p296864410116"><a name="p296864410116"></a><a name="p296864410116"></a>[1,65535]</p>
</td>
</tr>
<tr id="row387211011106"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p2023791201011"><a name="p2023791201011"></a><a name="p2023791201011"></a>metric_type</p>
</td>
<td class="cellrowborder" valign="top" width="14.591459145914593%" headers="mcps1.1.5.1.2 "><p id="p198722006101"><a name="p198722006101"></a><a name="p198722006101"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="30.29302930293029%" headers="mcps1.1.5.1.3 "><p id="p10237212111013"><a name="p10237212111013"></a><a name="p10237212111013"></a>距离度量类型。</p>
</td>
<td class="cellrowborder" valign="top" width="39.55395539553955%" headers="mcps1.1.5.1.4 "><p id="p5904125914109"><a name="p5904125914109"></a><a name="p5904125914109"></a>[0,1]，取值表示不同的距离度量类型：</p>
<a name="ul396901541013"></a><a name="ul396901541013"></a><ul id="ul396901541013"><li>0：内积距离。</li><li>1：欧氏距离。</li></ul>
</td>
</tr>
<tr id="row7131153011107"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p1546185591017"><a name="p1546185591017"></a><a name="p1546185591017"></a>codes</p>
</td>
<td class="cellrowborder" valign="top" width="14.591459145914593%" headers="mcps1.1.5.1.2 "><p id="p19131103031011"><a name="p19131103031011"></a><a name="p19131103031011"></a>const uint8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="30.29302930293029%" headers="mcps1.1.5.1.3 "><p id="p55461255161011"><a name="p55461255161011"></a><a name="p55461255161011"></a>底库向量（float）。</p>
</td>
<td class="cellrowborder" valign="top" width="39.55395539553955%" headers="mcps1.1.5.1.4 "><p id="p213293001016"><a name="p213293001016"></a><a name="p213293001016"></a>限制长度为codes_size，其中<span class="parmname" id="parmname17671637191415"><a name="parmname17671637191415"></a><a name="parmname17671637191415"></a>“codes_size”</span>为底库向量codes的长度。</p>
</td>
</tr>
<tr id="row104562557484"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p1151717330417"><a name="p1151717330417"></a><a name="p1151717330417"></a>codes_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.591459145914593%" headers="mcps1.1.5.1.2 "><p id="p351703319417"><a name="p351703319417"></a><a name="p351703319417"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="30.29302930293029%" headers="mcps1.1.5.1.3 "><p id="p6517433144111"><a name="p6517433144111"></a><a name="p6517433144111"></a>底库向量codes的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="39.55395539553955%" headers="mcps1.1.5.1.4 "><p id="p135171733184112"><a name="p135171733184112"></a><a name="p135171733184112"></a>codes_num * dim * 4，其中<span class="parmname" id="parmname11230185824311"><a name="parmname11230185824311"></a><a name="parmname11230185824311"></a>“codes_num”</span>为每个查询向量计算的底库向量数量，<span class="parmname" id="parmname152302580436"><a name="parmname152302580436"></a><a name="parmname152302580436"></a>“dim”</span>为向量维度。</p>
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
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a>正常运行时返回0，异常退出返回对应错误码。</p>
</td>
</tr>
</tbody>
</table>

**使用示例**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

int main() {
    // 参数配置
    size_t dim = 128;               // 向量维度
    size_t codes_num = 100;         // 重排候选向量数量
    size_t accu_level = 1;          // 粗排使用int8
    size_t full_accu_level = 3;     // 重排使用fp32
    int metric_type = 1;            // 欧氏距离

    // 准备底库向量数据
    size_t codes_size = codes_num * dim * sizeof(float);
    float* codes_data = (float*)malloc(codes_size);
    // ... 填充codes_data数据 ...

    // 创建重排Handle
    KRLDistanceHandle* kdh = NULL;
    int ret = krl_create_reorder_handle(
        &kdh,
        accu_level,
        full_accu_level,
        codes_num,
        dim,
        metric_type,
        (const uint8_t*)codes_data,
        codes_size
    );

    if (ret != 0) {
        printf("创建重排Handle失败，错误码: %d\n", ret);
        free(codes_data);
        return -1;
    }

    printf("成功创建重排KRLDistanceHandle\n");

    // ... 使用kdh进行重排计算 ...

    // 清理资源
    krl_clean_distance_handle(&kdh);
    free(codes_data);

    return 0;
}
```

### krl\_clean\_distance\_handle

**接口定义<a name="section172317194488"></a>**

void krl\_clean\_distance\_handle\(KRLDistanceHandle\*\* kdh\);

**接口用途<a name="section1153124784912"></a>**

析构KRLDistanceHandle实例，释放内存空间。

**参数说明<a name="section157501312135019"></a>**

<a name="table1646711617442"></a>
<table><thead align="left"><tr id="row846751612442"><th class="cellrowborder" valign="top" width="21.349999999999998%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="28.82%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="22.98%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="26.85%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row146815169448"><td class="cellrowborder" valign="top" width="21.349999999999998%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>kdh</p>
</td>
<td class="cellrowborder" valign="top" width="28.82%" headers="mcps1.1.5.1.2 "><p id="p98931015893"><a name="p98931015893"></a><a name="p98931015893"></a>KRLDistanceHandle**</p>
</td>
<td class="cellrowborder" valign="top" width="22.98%" headers="mcps1.1.5.1.3 "><p id="p182303331508"><a name="p182303331508"></a><a name="p182303331508"></a>需要被析构的KRLDistanceHandle指针。</p>
</td>
<td class="cellrowborder" valign="top" width="26.85%" headers="mcps1.1.5.1.4 "><p id="p12182012132917"><a name="p12182012132917"></a><a name="p12182012132917"></a>其指向的指针需要被krl_create_distance_handle初始化。</p>
</td>
</tr>
</tbody>
</table>

**使用示例**

```c
#include <stdio.h>
#include "krl.h"

int main() {
    KRLDistanceHandle* kdh = NULL;
    
    // 前置步骤：创建Handle
    size_t dim = 128;
    size_t codes_num = 1000;
    size_t codes_size = 1 * codes_num * dim * sizeof(float);
    float* codes_data = (float*)malloc(codes_size);
    // ... 填充数据 ...

    int ret = krl_create_distance_handle(&kdh, 3, 32, codes_num, dim, 1, 1, 
                                          (const uint8_t*)codes_data, codes_size);
    if (ret != 0) {
        free(codes_data);
        return -1;
    }

    // ... 使用kdh进行计算 ...

    // 清理Handle
    krl_clean_distance_handle(&kdh);
    // 此时kdh指向的指针已被置为NULL

    free(codes_data);
    printf("资源清理完成\n");

    return 0;
}
```

### krl\_create\_LUT8b\_handle

**接口定义<a name="section172317194488"></a>**

int krl\_create\_LUT8b\_handle\(KRLLUT8bHandle\*\* klh, int use\_idx, size\_t capacity\);

**接口用途<a name="section1153124784912"></a>**

初始化构建一个KRLLUT8bHandle实例，8bit查表累和时使用。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.56155615561556%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.591459145914593%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.96339633963397%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="35.88358835883588%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>klh</p>
</td>
<td class="cellrowborder" valign="top" width="14.591459145914593%" headers="mcps1.1.5.1.2 "><p id="p98931015893"><a name="p98931015893"></a><a name="p98931015893"></a>KRLLUT8bHandle**</p>
</td>
<td class="cellrowborder" valign="top" width="33.96339633963397%" headers="mcps1.1.5.1.3 "><p id="p182303331508"><a name="p182303331508"></a><a name="p182303331508"></a>需要被初始化构建的KRLLUT8bHandle指针。</p>
</td>
<td class="cellrowborder" valign="top" width="35.88358835883588%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>限制为非空指针，指向一个空指针。</p>
</td>
</tr>
<tr id="row11230173385019"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p22301333165015"><a name="p22301333165015"></a><a name="p22301333165015"></a>use_idx</p>
</td>
<td class="cellrowborder" valign="top" width="14.591459145914593%" headers="mcps1.1.5.1.2 "><p id="p5893141517919"><a name="p5893141517919"></a><a name="p5893141517919"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="33.96339633963397%" headers="mcps1.1.5.1.3 "><p id="p10230433115013"><a name="p10230433115013"></a><a name="p10230433115013"></a>是否进行底库向量筛选。</p>
</td>
<td class="cellrowborder" valign="top" width="35.88358835883588%" headers="mcps1.1.5.1.4 "><p id="p77289581198"><a name="p77289581198"></a><a name="p77289581198"></a>[0,1]，取值表示是否进行底库向量筛选：</p>
<a name="ul164886121012"></a><a name="ul164886121012"></a><ul id="ul164886121012"><li>0：不进行筛选。</li><li>1：进行筛选。</li></ul>
</td>
</tr>
<tr id="row1368063274610"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p10579191284217"><a name="p10579191284217"></a><a name="p10579191284217"></a>capacity</p>
</td>
<td class="cellrowborder" valign="top" width="14.591459145914593%" headers="mcps1.1.5.1.2 "><p id="p489312151893"><a name="p489312151893"></a><a name="p489312151893"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.96339633963397%" headers="mcps1.1.5.1.3 "><p id="p268013224617"><a name="p268013224617"></a><a name="p268013224617"></a>Handle类容量，最大可能的距离向量与筛选向量的大小。</p>
</td>
<td class="cellrowborder" valign="top" width="35.88358835883588%" headers="mcps1.1.5.1.4 "><p id="p173108137452"><a name="p173108137452"></a><a name="p173108137452"></a>大于等于1。大于等于调用krl_table_lookup_8b_f32_with_handle时的ncode，其中<span class="parmname" id="parmname103291726314"><a name="parmname103291726314"></a><a name="parmname103291726314"></a>“ncode”</span>为底库向量总数。</p>
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
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a>正常运行时返回0，异常退出返回对应错误码。</p>
</td>
</tr>
</tbody>
</table>

**使用示例**

```c
#include <stdio.h>
#include "krl.h"

int main() {
    // 参数配置
    int use_idx = 1;            // 启用底库向量筛选
    size_t capacity = 10000;    // 最大支持10000个底库向量

    // 创建LUT8b Handle
    KRLLUT8bHandle* klh = NULL;
    int ret = krl_create_LUT8b_handle(&klh, use_idx, capacity);

    if (ret != 0) {
        printf("创建LUT8b Handle失败，错误码: %d\n", ret);
        return -1;
    }

    printf("成功创建KRLLUT8bHandle\n");

    // 获取索引数组指针（用于设置需要计算的向量ID）
    size_t* idx_ptr = krl_get_idx_pointer(klh);

    // 获取距离数组指针（用于存储计算结果）
    float* dist_ptr = krl_get_dist_pointer(klh);

    // ... 使用klh进行查表累和计算 ...

    // 清理资源
    krl_clean_LUT8b_handle(&klh);

    return 0;
}
```

### krl\_clean\_LUT8b\_handle

**接口定义<a name="section172317194488"></a>**

void krl\_clean\_LUT8b\_handle\(KRLLUT8bHandle\*\* klh\);

**接口用途<a name="section1153124784912"></a>**

析构KRLLUT8bHandle实例，释放内存空间。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.56155615561556%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.591459145914593%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>klh</p>
</td>
<td class="cellrowborder" valign="top" width="14.591459145914593%" headers="mcps1.1.5.1.2 "><p id="p98931015893"><a name="p98931015893"></a><a name="p98931015893"></a>KRLLUT8bHandle**</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p182303331508"><a name="p182303331508"></a><a name="p182303331508"></a>需要被析构的KRLLUT8bHandle指针。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>其指向的指针需要被krl_create_LUT8b_handle初始化。</p>
</td>
</tr>
</tbody>
</table>

**使用示例**

```c
#include <stdio.h>
#include "krl.h"

int main() {
    KRLLUT8bHandle* klh = NULL;

    // 前置步骤：创建Handle
    int ret = krl_create_LUT8b_handle(&klh, 1, 10000);
    if (ret != 0) {
        return -1;
    }

    // ... 使用klh进行计算 ...

    // 清理Handle
    krl_clean_LUT8b_handle(&klh);
    // 此时klh指向的指针已被置为NULL

    printf("KRLLUT8bHandle资源清理完成\n");

    return 0;
}
```

### krl\_get\_idx\_pointer

**接口定义<a name="section172317194488"></a>**

size\_t\* krl\_get\_idx\_pointer\(const KRLLUT8bHandle\* klh\);

**接口用途<a name="section1153124784912"></a>**

获取KRLLUT8bHandle实例中存储的需要计算的底库向量ID。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.56155615561556%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.591459145914593%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>klh</p>
</td>
<td class="cellrowborder" valign="top" width="14.591459145914593%" headers="mcps1.1.5.1.2 "><p id="p98931015893"><a name="p98931015893"></a><a name="p98931015893"></a>KRLLUT8bHandle**</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p182303331508"><a name="p182303331508"></a><a name="p182303331508"></a>KRLLUT8bHandle指针。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>限制非空。</p>
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
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>size_t*</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p3457449204814"><a name="p3457449204814"></a><a name="p3457449204814"></a>KRLLUT8bHandle实例中存储的需要计算的底库向量ID。</p>
</td>
</tr>
</tbody>
</table>

**使用示例**

```c
#include <stdio.h>
#include "krl.h"

int main() {
    KRLLUT8bHandle* klh = NULL;
    size_t capacity = 1000;

    // 前置步骤：创建Handle
    int ret = krl_create_LUT8b_handle(&klh, 1, capacity);
    if (ret != 0) {
        return -1;
    }

    // 获取索引数组指针
    size_t* idx_ptr = krl_get_idx_pointer(klh);

    // 设置需要计算距离的底库向量ID
    // 例如：只计算ID为0, 5, 10, 15, 20的向量
    size_t selected_count = 5;
    idx_ptr[0] = 0;
    idx_ptr[1] = 5;
    idx_ptr[2] = 10;
    idx_ptr[3] = 15;
    idx_ptr[4] = 20;

    printf("已设置%zu个待计算的底库向量ID\n", selected_count);

    // ... 后续调用查表累和计算接口 ...

    krl_clean_LUT8b_handle(&klh);

    return 0;
}
```

### krl\_get\_dist\_pointer

**接口定义<a name="section172317194488"></a>**

float\* krl\_get\_dist\_pointer\(const KRLLUT8bHandle\* klh\);

**接口用途<a name="section1153124784912"></a>**

获取KRLLUT8bHandle实例中存储的距离数组首地址，在调用查表累和计算算子之前为随机数，调用之后为计算得到的距离。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.56155615561556%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.591459145914593%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>klh</p>
</td>
<td class="cellrowborder" valign="top" width="14.591459145914593%" headers="mcps1.1.5.1.2 "><p id="p98931015893"><a name="p98931015893"></a><a name="p98931015893"></a>KRLLUT8bHandle*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p182303331508"><a name="p182303331508"></a><a name="p182303331508"></a>KRLLUT8bHandle指针。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>限制非空。</p>
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
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>float*</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p3457449204814"><a name="p3457449204814"></a><a name="p3457449204814"></a>KRLLUT8bHandle实例中存储的距离数组首地址，在调用查表累和计算算子之前为随机数，调用之后为计算得到的距离。</p>
</td>
</tr>
</tbody>
</table>

**使用示例**

```c
#include <stdio.h>
#include "krl.h"

int main() {
    KRLLUT8bHandle* klh = NULL;
    size_t capacity = 1000;

    // 前置步骤：创建Handle
    int ret = krl_create_LUT8b_handle(&klh, 0, capacity);
    if (ret != 0) {
        return -1;
    }

    // 获取距离数组指针
    float* dist_ptr = krl_get_dist_pointer(klh);

    // 注意：此时dist_ptr中的值为随机数
    // 需要调用查表累和计算接口后才有有效距离值

    // ... 调用查表累和计算接口 ...

    // 计算完成后，读取距离结果
    size_t num_results = 100;  // 假设计算了100个向量的距离
    printf("前5个距离结果:\n");
    for (size_t i = 0; i < 5 && i < num_results; i++) {
        printf("  dist[%zu] = %f\n", i, dist_ptr[i]);
    }

    krl_clean_LUT8b_handle(&klh);

    return 0;
}
```

## 距离计算接口

### krl\_L2sqr

**接口定义<a name="section172317194488"></a>**

int krl\_L2sqr\(const float\* x, const float\* \_\_restrict y, const size\_t d, float\* dis, size\_t dis\_size\);

**接口用途<a name="section1153124784912"></a>**

进行数据类型为float的一对一欧氏距离计算。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.601460146014599%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p953215815518"><a name="p953215815518"></a><a name="p953215815518"></a>const float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p18661136253"><a name="p18661136253"></a><a name="p18661136253"></a>参与距离计算的查询向量。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>限制长度为d，其中<span class="parmname" id="parmname76117481457"><a name="parmname76117481457"></a><a name="parmname76117481457"></a>“d”</span>为向量维度。</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4982142445414"><a name="p4982142445414"></a><a name="p4982142445414"></a>y</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7532158856"><a name="p7532158856"></a><a name="p7532158856"></a>const float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p36611261054"><a name="p36611261054"></a><a name="p36611261054"></a>参与距离计算的底库向量。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>限制长度为d，其中<span class="parmname" id="parmname551215813519"><a name="parmname551215813519"></a><a name="parmname551215813519"></a>“d”</span>为向量维度。</p>
</td>
</tr>
<tr id="row106882715416"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p46812710547"><a name="p46812710547"></a><a name="p46812710547"></a>d</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p45311183519"><a name="p45311183519"></a><a name="p45311183519"></a>const size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p17661261256"><a name="p17661261256"></a><a name="p17661261256"></a>向量维度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p46952755416"><a name="p46952755416"></a><a name="p46952755416"></a>[1,65535]</p>
</td>
</tr>
<tr id="row2848154911529"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4849194916526"><a name="p4849194916526"></a><a name="p4849194916526"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p484916497520"><a name="p484916497520"></a><a name="p484916497520"></a>float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p184912496525"><a name="p184912496525"></a><a name="p184912496525"></a>存储计算所得的距离结果。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1984914498527"><a name="p1984914498527"></a><a name="p1984914498527"></a>限制长度为dis_size，其中<span class="parmname" id="parmname133743422533"><a name="parmname133743422533"></a><a name="parmname133743422533"></a>“dis_size”</span>为存储距离结果数组的长度。需要预先分配内存。</p>
</td>
</tr>
<tr id="row13612117522"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p271521115212"><a name="p271521115212"></a><a name="p271521115212"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p10722125214"><a name="p10722125214"></a><a name="p10722125214"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p1762116529"><a name="p1762116529"></a><a name="p1762116529"></a>存储距离结果数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p17182165214"><a name="p17182165214"></a><a name="p17182165214"></a>限制为1。</p>
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
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a>正常运行时返回0，异常退出返回对应错误码。</p>
</td>
</tr>
</tbody>
</table>

**使用示例**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

int main() {
    size_t dim = 128;  // 向量维度

    // 准备查询向量和底库向量
    float* query_vec = (float*)malloc(dim * sizeof(float));
    float* base_vec = (float*)malloc(dim * sizeof(float));

    // 填充示例数据
    for (size_t i = 0; i < dim; i++) {
        query_vec[i] = (float)i / dim;
        base_vec[i] = (float)(dim - i) / dim;
    }

    // 存储距离结果
    float distance = 0.0f;

    // 计算欧氏距离
    int ret = krl_L2sqr(query_vec, base_vec, dim, &distance, 1);

    if (ret != 0) {
        printf("距离计算失败，错误码: %d\n", ret);
        free(query_vec);
        free(base_vec);
        return -1;
    }

    printf("欧氏距离（L2平方）: %f\n", distance);

    free(query_vec);
    free(base_vec);

    return 0;
}
```

### krl\_L2sqr\_f16f32

**接口定义<a name="section172317194488"></a>**

int krl\_L2sqr\_f16f32\(const uint16\_t\* x, const uint16\_t\* \_\_restrict y, size\_t d, float\* dis, size\_t dis\_size\);

**接口用途<a name="section1153124784912"></a>**

进行数据类型为fp16的一对一欧氏距离计算。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.601460146014599%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p953215815518"><a name="p953215815518"></a><a name="p953215815518"></a>const uint16_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p18661136253"><a name="p18661136253"></a><a name="p18661136253"></a>参与距离计算的查询向量。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>限制长度为d，其中<span class="parmname" id="parmname76117481457"><a name="parmname76117481457"></a><a name="parmname76117481457"></a>“d”</span>为向量维度。</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4982142445414"><a name="p4982142445414"></a><a name="p4982142445414"></a>y</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7532158856"><a name="p7532158856"></a><a name="p7532158856"></a>const uint16_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p36611261054"><a name="p36611261054"></a><a name="p36611261054"></a>参与距离计算的底库向量。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>限制长度为d，其中<span class="parmname" id="parmname551215813519"><a name="parmname551215813519"></a><a name="parmname551215813519"></a>“d”</span>为向量维度。</p>
</td>
</tr>
<tr id="row106882715416"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p46812710547"><a name="p46812710547"></a><a name="p46812710547"></a>d</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p45311183519"><a name="p45311183519"></a><a name="p45311183519"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p17661261256"><a name="p17661261256"></a><a name="p17661261256"></a>向量维度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p46952755416"><a name="p46952755416"></a><a name="p46952755416"></a>[1,65535]</p>
</td>
</tr>
<tr id="row6435174117149"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4849194916526"><a name="p4849194916526"></a><a name="p4849194916526"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p484916497520"><a name="p484916497520"></a><a name="p484916497520"></a>float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p184912496525"><a name="p184912496525"></a><a name="p184912496525"></a>存储计算所得的距离结果。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1984914498527"><a name="p1984914498527"></a><a name="p1984914498527"></a>限制长度为dis_size，其中<span class="parmname" id="parmname133743422533"><a name="parmname133743422533"></a><a name="parmname133743422533"></a>“dis_size”</span>为存储距离结果数组的长度。需要预先分配内存。</p>
</td>
</tr>
<tr id="row14276273554"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p271521115212"><a name="p271521115212"></a><a name="p271521115212"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p10722125214"><a name="p10722125214"></a><a name="p10722125214"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p1762116529"><a name="p1762116529"></a><a name="p1762116529"></a>存储距离结果数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p17182165214"><a name="p17182165214"></a><a name="p17182165214"></a>限制为1。</p>
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
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a>正常运行时返回0，异常退出返回对应错误码。</p>
</td>
</tr>
</tbody>
</table>

**使用示例**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

// 辅助函数：将float转换为fp16
uint16_t float_to_fp16(float value);

int main() {
    size_t dim = 128;  // 向量维度

    // 准备fp16格式的查询向量和底库向量
    uint16_t* query_vec_fp16 = (uint16_t*)malloc(dim * sizeof(uint16_t));
    uint16_t* base_vec_fp16 = (uint16_t*)malloc(dim * sizeof(uint16_t));

    // 填充示例数据（先转换为fp16格式）
    for (size_t i = 0; i < dim; i++) {
        query_vec_fp16[i] = float_to_fp16((float)i / dim);
        base_vec_fp16[i] = float_to_fp16((float)(dim - i) / dim);
    }

    // 存储距离结果（输出为float类型）
    float distance = 0.0f;

    // 计算fp16向量的欧氏距离
    int ret = krl_L2sqr_f16f32(query_vec_fp16, base_vec_fp16, dim, &distance, 1);

    if (ret != 0) {
        printf("fp16距离计算失败，错误码: %d\n", ret);
        free(query_vec_fp16);
        free(base_vec_fp16);
        return -1;
    }

    printf("fp16欧氏距离（L2平方）: %f\n", distance);

    free(query_vec_fp16);
    free(base_vec_fp16);

    return 0;
}
```

### krl\_L2sqr\_u8u32

**接口定义<a name="section172317194488"></a>**

int krl\_L2sqr\_u8u32\(const uint8\_t\* x, const uint8\_t\* \_\_restrict y, size\_t d, uint32\_t\* dis, size\_t dis\_size\);

**接口用途<a name="section1153124784912"></a>**

进行数据类型为uint8的一对一欧氏距离计算。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.601460146014599%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.77337733773377%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="36.07360736073608%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p953215815518"><a name="p953215815518"></a><a name="p953215815518"></a>const uint8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.77337733773377%" headers="mcps1.1.5.1.3 "><p id="p18661136253"><a name="p18661136253"></a><a name="p18661136253"></a>参与距离计算的查询向量。</p>
</td>
<td class="cellrowborder" valign="top" width="36.07360736073608%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>限制长度为d，其中<span class="parmname" id="parmname76117481457"><a name="parmname76117481457"></a><a name="parmname76117481457"></a>“d”</span>为向量维度。</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4982142445414"><a name="p4982142445414"></a><a name="p4982142445414"></a>y</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7532158856"><a name="p7532158856"></a><a name="p7532158856"></a>const uint8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.77337733773377%" headers="mcps1.1.5.1.3 "><p id="p36611261054"><a name="p36611261054"></a><a name="p36611261054"></a>参与距离计算的底库向量。</p>
</td>
<td class="cellrowborder" valign="top" width="36.07360736073608%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>限制长度为d，其中<span class="parmname" id="parmname551215813519"><a name="parmname551215813519"></a><a name="parmname551215813519"></a>“d”</span>为向量维度。</p>
</td>
</tr>
<tr id="row106882715416"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p46812710547"><a name="p46812710547"></a><a name="p46812710547"></a>d</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p45311183519"><a name="p45311183519"></a><a name="p45311183519"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.77337733773377%" headers="mcps1.1.5.1.3 "><p id="p17661261256"><a name="p17661261256"></a><a name="p17661261256"></a>向量维度。</p>
</td>
<td class="cellrowborder" valign="top" width="36.07360736073608%" headers="mcps1.1.5.1.4 "><p id="p46952755416"><a name="p46952755416"></a><a name="p46952755416"></a>[1,65535]</p>
</td>
</tr>
<tr id="row5811550198"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4849194916526"><a name="p4849194916526"></a><a name="p4849194916526"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p484916497520"><a name="p484916497520"></a><a name="p484916497520"></a>uint32_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.77337733773377%" headers="mcps1.1.5.1.3 "><p id="p184912496525"><a name="p184912496525"></a><a name="p184912496525"></a>存储计算所得的距离结果。</p>
</td>
<td class="cellrowborder" valign="top" width="36.07360736073608%" headers="mcps1.1.5.1.4 "><p id="p1984914498527"><a name="p1984914498527"></a><a name="p1984914498527"></a>限制长度为dis_size，其中<span class="parmname" id="parmname133743422533"><a name="parmname133743422533"></a><a name="parmname133743422533"></a>“dis_size”</span>为存储距离结果数组的长度。需要预先分配内存。</p>
</td>
</tr>
<tr id="row1971384576"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p271521115212"><a name="p271521115212"></a><a name="p271521115212"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p10722125214"><a name="p10722125214"></a><a name="p10722125214"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.77337733773377%" headers="mcps1.1.5.1.3 "><p id="p1762116529"><a name="p1762116529"></a><a name="p1762116529"></a>存储距离结果数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="36.07360736073608%" headers="mcps1.1.5.1.4 "><p id="p17182165214"><a name="p17182165214"></a><a name="p17182165214"></a>限制为1。</p>
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
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a>正常运行时返回0，异常退出返回对应错误码。</p>
</td>
</tr>
</tbody>
</table>

**使用示例**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

int main() {
    size_t dim = 128;  // 向量维度

    // 准备uint8类型的查询向量和底库向量
    uint8_t* query_vec = (uint8_t*)malloc(dim * sizeof(uint8_t));
    uint8_t* base_vec = (uint8_t*)malloc(dim * sizeof(uint8_t));

    // 填充示例数据（0-255范围的整数）
    for (size_t i = 0; i < dim; i++) {
        query_vec[i] = (uint8_t)(i * 2 % 256);
        base_vec[i] = (uint8_t)((dim - i) * 2 % 256);
    }

    // 存储距离结果（uint32类型）
    uint32_t distance = 0;

    // 计算uint8向量的欧氏距离
    int ret = krl_L2sqr_u8u32(query_vec, base_vec, dim, &distance, 1);

    if (ret != 0) {
        printf("uint8距离计算失败，错误码: %d\n", ret);
        free(query_vec);
        free(base_vec);
        return -1;
    }

    printf("uint8欧氏距离（L2平方）: %u\n", distance);

    free(query_vec);
    free(base_vec);

    return 0;
}
```

### krl\_ipdis

**接口定义<a name="section172317194488"></a>**

int krl\_ipdis\(const float\* x, const float\* \_\_restrict y, const size\_t d, float\* dis, size\_t dis\_size\);

**接口用途<a name="section1153124784912"></a>**

进行数据类型为float的一对一内积距离计算。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.591459145914593%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="34.003400340034005%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="14.591459145914593%" headers="mcps1.1.5.1.2 "><p id="p953215815518"><a name="p953215815518"></a><a name="p953215815518"></a>const float*</p>
</td>
<td class="cellrowborder" valign="top" width="34.003400340034005%" headers="mcps1.1.5.1.3 "><p id="p18661136253"><a name="p18661136253"></a><a name="p18661136253"></a>参与距离计算的查询向量。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>限制长度为d，其中<span class="parmname" id="parmname76117481457"><a name="parmname76117481457"></a><a name="parmname76117481457"></a>“d”</span>为向量维度。</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4982142445414"><a name="p4982142445414"></a><a name="p4982142445414"></a>y</p>
</td>
<td class="cellrowborder" valign="top" width="14.591459145914593%" headers="mcps1.1.5.1.2 "><p id="p7532158856"><a name="p7532158856"></a><a name="p7532158856"></a>const float*</p>
</td>
<td class="cellrowborder" valign="top" width="34.003400340034005%" headers="mcps1.1.5.1.3 "><p id="p36611261054"><a name="p36611261054"></a><a name="p36611261054"></a>参与距离计算的底库向量。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>限制长度为d，其中<span class="parmname" id="parmname551215813519"><a name="parmname551215813519"></a><a name="parmname551215813519"></a>“d”</span>为向量维度。</p>
</td>
</tr>
<tr id="row106882715416"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p46812710547"><a name="p46812710547"></a><a name="p46812710547"></a>d</p>
</td>
<td class="cellrowborder" valign="top" width="14.591459145914593%" headers="mcps1.1.5.1.2 "><p id="p45311183519"><a name="p45311183519"></a><a name="p45311183519"></a>const size_t</p>
</td>
<td class="cellrowborder" valign="top" width="34.003400340034005%" headers="mcps1.1.5.1.3 "><p id="p17661261256"><a name="p17661261256"></a><a name="p17661261256"></a>向量维度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p46952755416"><a name="p46952755416"></a><a name="p46952755416"></a>[1,65535]</p>
</td>
</tr>
<tr id="row6516613222"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p8546192216"><a name="p8546192216"></a><a name="p8546192216"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.591459145914593%" headers="mcps1.1.5.1.2 "><p id="p484916497520"><a name="p484916497520"></a><a name="p484916497520"></a>float*</p>
</td>
<td class="cellrowborder" valign="top" width="34.003400340034005%" headers="mcps1.1.5.1.3 "><p id="p184912496525"><a name="p184912496525"></a><a name="p184912496525"></a>存储计算所得的距离结果。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1984914498527"><a name="p1984914498527"></a><a name="p1984914498527"></a>限制长度为dis_size，其中<span class="parmname" id="parmname133743422533"><a name="parmname133743422533"></a><a name="parmname133743422533"></a>“dis_size”</span>为存储距离结果数组的长度。需要预先分配内存。</p>
</td>
</tr>
<tr id="row976544717599"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p271521115212"><a name="p271521115212"></a><a name="p271521115212"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.591459145914593%" headers="mcps1.1.5.1.2 "><p id="p10722125214"><a name="p10722125214"></a><a name="p10722125214"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="34.003400340034005%" headers="mcps1.1.5.1.3 "><p id="p1762116529"><a name="p1762116529"></a><a name="p1762116529"></a>存储距离结果数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p17182165214"><a name="p17182165214"></a><a name="p17182165214"></a>限制为1。</p>
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
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a>正常运行时返回0，异常退出返回对应错误码。</p>
</td>
</tr>
</tbody>
</table>

**使用示例**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

int main() {
    size_t dim = 128;  // 向量维度

    // 准备查询向量和底库向量
    float* query_vec = (float*)malloc(dim * sizeof(float));
    float* base_vec = (float*)malloc(dim * sizeof(float));

    // 填充示例数据
    float norm_q = 0.0f, norm_b = 0.0f;
    for (size_t i = 0; i < dim; i++) {
        query_vec[i] = (float)i;
        base_vec[i] = (float)(dim - i);
        norm_q += query_vec[i] * query_vec[i];
        norm_b += base_vec[i] * base_vec[i];
    }
    // 归一化
    norm_q = sqrtf(norm_q);
    norm_b = sqrtf(norm_b);
    for (size_t i = 0; i < dim; i++) {
        query_vec[i] /= norm_q;
        base_vec[i] /= norm_b;
    }

    // 存储距离结果
    float distance = 0.0f;

    // 计算内积距离
    int ret = krl_ipdis(query_vec, base_vec, dim, &distance, 1);

    if (ret != 0) {
        printf("内积距离计算失败，错误码: %d\n", ret);
        free(query_vec);
        free(base_vec);
        return -1;
    }

    printf("内积距离: %f\n", distance);
    // 对于归一化向量，内积距离范围为[-1, 1]

    free(query_vec);
    free(base_vec);

    return 0;
}
```

### krl\_negative\_ipdis\_f16f32

**接口定义<a name="section172317194488"></a>**

float krl\_negative\_ipdis\_f16f32\(const uint16\_t\* x, const uint16\_t\* \_\_restrict y, const size\_t d, float\* dis, size\_t dis\_size\);

**接口用途<a name="section1153124784912"></a>**

进行数据类型为fp16的一对一内积距离计算。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.601460146014599%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p953215815518"><a name="p953215815518"></a><a name="p953215815518"></a>const uint16_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p18661136253"><a name="p18661136253"></a><a name="p18661136253"></a>参与距离计算的查询向量。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>限制长度为d，其中<span class="parmname" id="parmname76117481457"><a name="parmname76117481457"></a><a name="parmname76117481457"></a>“d”</span>为向量维度。</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4982142445414"><a name="p4982142445414"></a><a name="p4982142445414"></a>y</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7532158856"><a name="p7532158856"></a><a name="p7532158856"></a>const uint16_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p36611261054"><a name="p36611261054"></a><a name="p36611261054"></a>参与距离计算的底库向量。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>限制长度为d，其中<span class="parmname" id="parmname551215813519"><a name="parmname551215813519"></a><a name="parmname551215813519"></a>“d”</span>为向量维度。</p>
</td>
</tr>
<tr id="row106882715416"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p46812710547"><a name="p46812710547"></a><a name="p46812710547"></a>d</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p45311183519"><a name="p45311183519"></a><a name="p45311183519"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p17661261256"><a name="p17661261256"></a><a name="p17661261256"></a>向量维度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p46952755416"><a name="p46952755416"></a><a name="p46952755416"></a>[1,65535]</p>
</td>
</tr>
<tr id="row172931135182017"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p8546192216"><a name="p8546192216"></a><a name="p8546192216"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p484916497520"><a name="p484916497520"></a><a name="p484916497520"></a>float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p184912496525"><a name="p184912496525"></a><a name="p184912496525"></a>存储计算所得的距离结果。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1984914498527"><a name="p1984914498527"></a><a name="p1984914498527"></a>限制长度为dis_size，其中<span class="parmname" id="parmname133743422533"><a name="parmname133743422533"></a><a name="parmname133743422533"></a>“dis_size”</span>为存储距离结果数组的长度。需要预先分配内存。</p>
</td>
</tr>
<tr id="row54317463111"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p271521115212"><a name="p271521115212"></a><a name="p271521115212"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p10722125214"><a name="p10722125214"></a><a name="p10722125214"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p1762116529"><a name="p1762116529"></a><a name="p1762116529"></a>存储距离结果数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p17182165214"><a name="p17182165214"></a><a name="p17182165214"></a>限制为1。</p>
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
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a>正常运行时返回0，异常退出返回对应错误码。</p>
</td>
</tr>
</tbody>
</table>

**使用示例**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

// 辅助函数：将float转换为fp16
uint16_t float_to_fp16(float value);

int main() {
    size_t dim = 128;  // 向量维度

    // 准备fp16格式的向量
    uint16_t* query_vec_fp16 = (uint16_t*)malloc(dim * sizeof(uint16_t));
    uint16_t* base_vec_fp16 = (uint16_t*)malloc(dim * sizeof(uint16_t));

    // 填充示例数据
    for (size_t i = 0; i < dim; i++) {
        query_vec_fp16[i] = float_to_fp16(0.1f);
        base_vec_fp16[i] = float_to_fp16(0.2f);
    }

    // 存储距离结果
    float distance = 0.0f;

    // 计算fp16向量的内积距离（返回负内积）
    int ret = krl_negative_ipdis_f16f32(query_vec_fp16, base_vec_fp16, dim, &distance, 1);

    if (ret != 0) {
        printf("fp16内积距离计算失败，错误码: %d\n", ret);
        free(query_vec_fp16);
        free(base_vec_fp16);
        return -1;
    }

    printf("fp16负内积距离: %f\n", distance);

    free(query_vec_fp16);
    free(base_vec_fp16);

    return 0;
}
```

### krl\_negative\_ipdis\_s8s32

**接口定义<a name="section172317194488"></a>**

int krl\_negative\_ipdis\_s8s32\(const int8\_t\* x, const int8\_t\* \_\_restrict y, const size\_t d, int32\_t\* dis, size\_t dis\_size\);

**接口用途<a name="section1153124784912"></a>**

进行数据类型为int8的一对一内积距离计算。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.601460146014599%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p953215815518"><a name="p953215815518"></a><a name="p953215815518"></a>const int8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p18661136253"><a name="p18661136253"></a><a name="p18661136253"></a>参与距离计算的查询向量。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>限制长度为d，其中<span class="parmname" id="parmname76117481457"><a name="parmname76117481457"></a><a name="parmname76117481457"></a>“d”</span>为向量维度。</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4982142445414"><a name="p4982142445414"></a><a name="p4982142445414"></a>y</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7532158856"><a name="p7532158856"></a><a name="p7532158856"></a>const int8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p36611261054"><a name="p36611261054"></a><a name="p36611261054"></a>参与距离计算的底库向量。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>限制长度为d，其中<span class="parmname" id="parmname551215813519"><a name="parmname551215813519"></a><a name="parmname551215813519"></a>“d”</span>为向量维度。</p>
</td>
</tr>
<tr id="row106882715416"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p46812710547"><a name="p46812710547"></a><a name="p46812710547"></a>d</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p45311183519"><a name="p45311183519"></a><a name="p45311183519"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p17661261256"><a name="p17661261256"></a><a name="p17661261256"></a>向量维度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p46952755416"><a name="p46952755416"></a><a name="p46952755416"></a>[1,65535]</p>
</td>
</tr>
<tr id="row78157718211"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4816127192115"><a name="p4816127192115"></a><a name="p4816127192115"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p28168718210"><a name="p28168718210"></a><a name="p28168718210"></a>int32_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p184912496525"><a name="p184912496525"></a><a name="p184912496525"></a>存储计算所得的距离结果。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1984914498527"><a name="p1984914498527"></a><a name="p1984914498527"></a>限制长度为dis_size，其中<span class="parmname" id="parmname133743422533"><a name="parmname133743422533"></a><a name="parmname133743422533"></a>“dis_size”</span>为存储距离结果数组的长度。需要预先分配内存。</p>
</td>
</tr>
<tr id="row162270523"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p271521115212"><a name="p271521115212"></a><a name="p271521115212"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p10722125214"><a name="p10722125214"></a><a name="p10722125214"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p1762116529"><a name="p1762116529"></a><a name="p1762116529"></a>存储距离结果数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p17182165214"><a name="p17182165214"></a><a name="p17182165214"></a>限制为1。</p>
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
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a>正常运行时返回0，异常退出返回对应错误码。</p>
</td>
</tr>
</tbody>
</table>

**使用示例**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

int main() {
    size_t dim = 128;  // 向量维度

    // 准备int8类型的向量
    int8_t* query_vec = (int8_t*)malloc(dim * sizeof(int8_t));
    int8_t* base_vec = (int8_t*)malloc(dim * sizeof(int8_t));

    // 填充示例数据（-128到127范围）
    for (size_t i = 0; i < dim; i++) {
        query_vec[i] = (int8_t)(i % 128);
        base_vec[i] = (int8_t)((dim - i) % 128);
    }

    // 存储距离结果（int32类型）
    int32_t distance = 0;

    // 计算int8向量的内积距离
    int ret = krl_negative_ipdis_s8s32(query_vec, base_vec, dim, &distance, 1);

    if (ret != 0) {
        printf("int8内积距离计算失败，错误码: %d\n", ret);
        free(query_vec);
        free(base_vec);
        return -1;
    }

    printf("int8负内积距离: %d\n", distance);

    free(query_vec);
    free(base_vec);

    return 0;
}
```

### krl\_L2sqr\_by\_idx

**接口定义<a name="section172317194488"></a>**

int krl\_L2sqr\_by\_idx\(float\* dis, const float\* x, const float\* y, const int64\_t\* ids, size\_t d, size\_t ny, size\_t dis\_size\);

**接口用途<a name="section1153124784912"></a>**

进行数据类型为float的一对多欧氏距离计算。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.601460146014599%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row92301478154"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p223015479158"><a name="p223015479158"></a><a name="p223015479158"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p11230154710156"><a name="p11230154710156"></a><a name="p11230154710156"></a>float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p82303471154"><a name="p82303471154"></a><a name="p82303471154"></a>存储计算所得的距离结果。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1984914498527"><a name="p1984914498527"></a><a name="p1984914498527"></a>限制长度为dis_size，其中<span class="parmname" id="parmname133743422533"><a name="parmname133743422533"></a><a name="parmname133743422533"></a>“dis_size”</span>为存储距离结果数组的长度。需要预先分配内存。</p>
</td>
</tr>
<tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p953215815518"><a name="p953215815518"></a><a name="p953215815518"></a>const float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p18661136253"><a name="p18661136253"></a><a name="p18661136253"></a>参与距离计算的查询向量。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>限制长度为d，其中<span class="parmname" id="parmname76117481457"><a name="parmname76117481457"></a><a name="parmname76117481457"></a>“d”</span>为向量维度。</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4982142445414"><a name="p4982142445414"></a><a name="p4982142445414"></a>y</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7532158856"><a name="p7532158856"></a><a name="p7532158856"></a>const float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p36611261054"><a name="p36611261054"></a><a name="p36611261054"></a>参与距离计算的底库向量。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>限制长度为d*ny，其中<span class="parmname" id="parmname551215813519"><a name="parmname551215813519"></a><a name="parmname551215813519"></a>“d”</span>为向量维度，<span class="parmname" id="parmname8646142120239"><a name="parmname8646142120239"></a><a name="parmname8646142120239"></a>“ny”</span>为参与距离计算的底库向量个数。</p>
</td>
</tr>
<tr id="row103951453161513"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p1395185361518"><a name="p1395185361518"></a><a name="p1395185361518"></a>ids</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p93958532154"><a name="p93958532154"></a><a name="p93958532154"></a>const int64_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p2039510531150"><a name="p2039510531150"></a><a name="p2039510531150"></a>参与距离计算的底库向量ID。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p6395135351511"><a name="p6395135351511"></a><a name="p6395135351511"></a>限制长度为ny，其中<span class="parmname" id="parmname0410141908"><a name="parmname0410141908"></a><a name="parmname0410141908"></a>“ny”</span>为参与距离计算的底库向量个数。ID大于等于0，小于底库向量的总数。</p>
</td>
</tr>
<tr id="row106882715416"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p46812710547"><a name="p46812710547"></a><a name="p46812710547"></a>d</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p45311183519"><a name="p45311183519"></a><a name="p45311183519"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p17661261256"><a name="p17661261256"></a><a name="p17661261256"></a>向量维度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p46952755416"><a name="p46952755416"></a><a name="p46952755416"></a>[1,65535]</p>
</td>
</tr>
<tr id="row37151957141516"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p171515741513"><a name="p171515741513"></a><a name="p171515741513"></a>ny</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p3715105741513"><a name="p3715105741513"></a><a name="p3715105741513"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p197153572157"><a name="p197153572157"></a><a name="p197153572157"></a>参与距离计算的底库向量个数。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1071517573156"><a name="p1071517573156"></a><a name="p1071517573156"></a>[1,2^30-1]</p>
</td>
</tr>
<tr id="row1396217381443"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p39628388417"><a name="p39628388417"></a><a name="p39628388417"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p10722125214"><a name="p10722125214"></a><a name="p10722125214"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p1762116529"><a name="p1762116529"></a><a name="p1762116529"></a>存储距离结果数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p154517391451"><a name="p154517391451"></a><a name="p154517391451"></a>ny，其中<span class="parmname" id="parmname44553910519"><a name="parmname44553910519"></a><a name="parmname44553910519"></a>“ny”</span>为参与距离计算的底库向量个数。</p>
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
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a>正常运行时返回0，异常退出返回对应错误码。</p>
</td>
</tr>
</tbody>
</table>

**使用示例**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

int main() {
    size_t dim = 128;                     // 向量维度
    size_t total_base_vectors = 10000;    // 底库总向量数
    size_t ny = 100;                      // 需要计算距离的向量个数

    // 准备查询向量
    float* query_vec = (float*)malloc(dim * sizeof(float));
    for (size_t i = 0; i < dim; i++) {
        query_vec[i] = (float)(rand() % 1000) / 1000.0f;
    }

    // 准备底库向量（实际场景中通常从文件或数据库加载）
    float* base_vectors = (float*)malloc(total_base_vectors * dim * sizeof(float));
    for (size_t i = 0; i < total_base_vectors * dim; i++) {
        base_vectors[i] = (float)(rand() % 1000) / 1000.0f;
    }

    // 指定需要计算距离的底库向量ID
    // 例如：计算ID为0, 10, 20, 30, ... 的向量
    int64_t* ids = (int64_t*)malloc(ny * sizeof(int64_t));
    for (size_t i = 0; i < ny; i++) {
        ids[i] = (int64_t)(i * 10);  // 每隔10个选一个
    }

    // 分配距离结果数组
    float* distances = (float*)malloc(ny * sizeof(float));

    // 执行一对多欧氏距离计算
    int ret = krl_L2sqr_by_idx(
        distances,      // 输出
        query_vec,      // 查询向量
        base_vectors,   // 底库向量
        ids,            // 指定的向量ID
        dim,            // 向量维度
        ny,             // 计算的向量个数
        ny              // 结果数组长度
    );

    if (ret != 0) {
        printf("一对多距离计算失败，错误码: %d\n", ret);
        goto cleanup;
    }

    // 输出前5个结果
    printf("一对多欧氏距离计算结果（前5个）:\n");
    for (size_t i = 0; i < 5 && i < ny; i++) {
        printf("  与向量ID[%ld]的距离: %f\n", ids[i], distances[i]);
    }

cleanup:
    free(query_vec);
    free(base_vectors);
    free(ids);
    free(distances);

    return ret;
}
```

### krl\_L2sqr\_by\_idx\_f16f32

**接口定义<a name="section172317194488"></a>**

int krl\_L2sqr\_by\_idx\_f16f32\(float\* dis, const uint16\_t\* x, const uint16\_t\* y, const int64\_t\* ids, size\_t d, size\_t ny, size\_t dis\_size\);

**接口用途<a name="section1153124784912"></a>**

进行数据类型为fp16的一对多欧氏距离计算。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.601460146014599%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row92301478154"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p223015479158"><a name="p223015479158"></a><a name="p223015479158"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p11230154710156"><a name="p11230154710156"></a><a name="p11230154710156"></a>float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p82303471154"><a name="p82303471154"></a><a name="p82303471154"></a>存储计算所得的距离结果。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p923018478155"><a name="p923018478155"></a><a name="p923018478155"></a>限制长度为dis_size，其中<span class="parmname" id="parmname133743422533"><a name="parmname133743422533"></a><a name="parmname133743422533"></a>“dis_size”</span>为存储距离结果数组的长度。需要预先分配内存。</p>
</td>
</tr>
<tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p953215815518"><a name="p953215815518"></a><a name="p953215815518"></a>const uint16_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p18661136253"><a name="p18661136253"></a><a name="p18661136253"></a>参与距离计算的查询向量。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>限制长度为d，其中<span class="parmname" id="parmname76117481457"><a name="parmname76117481457"></a><a name="parmname76117481457"></a>“d”</span>为向量维度。</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4982142445414"><a name="p4982142445414"></a><a name="p4982142445414"></a>y</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7532158856"><a name="p7532158856"></a><a name="p7532158856"></a>const uint16_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p36611261054"><a name="p36611261054"></a><a name="p36611261054"></a>参与距离计算的底库向量。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>限制长度为d*ny，其中<span class="parmname" id="parmname551215813519"><a name="parmname551215813519"></a><a name="parmname551215813519"></a>“d”</span>为向量维度，<span class="parmname" id="parmname8646142120239"><a name="parmname8646142120239"></a><a name="parmname8646142120239"></a>“ny”</span>为参与距离计算的底库向量个数。</p>
</td>
</tr>
<tr id="row103951453161513"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p1395185361518"><a name="p1395185361518"></a><a name="p1395185361518"></a>ids</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p93958532154"><a name="p93958532154"></a><a name="p93958532154"></a>const int64_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p2039510531150"><a name="p2039510531150"></a><a name="p2039510531150"></a>参与距离计算的底库向量ID。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p6395135351511"><a name="p6395135351511"></a><a name="p6395135351511"></a>限制长度为ny，其中<span class="parmname" id="parmname0410141908"><a name="parmname0410141908"></a><a name="parmname0410141908"></a>“ny”</span>为参与距离计算的底库向量个数。ID大于等于0，小于底库向量的总数。</p>
</td>
</tr>
<tr id="row106882715416"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p46812710547"><a name="p46812710547"></a><a name="p46812710547"></a>d</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p45311183519"><a name="p45311183519"></a><a name="p45311183519"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p17661261256"><a name="p17661261256"></a><a name="p17661261256"></a>向量维度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p46952755416"><a name="p46952755416"></a><a name="p46952755416"></a>[1,65535]</p>
</td>
</tr>
<tr id="row37151957141516"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p171515741513"><a name="p171515741513"></a><a name="p171515741513"></a>ny</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p3715105741513"><a name="p3715105741513"></a><a name="p3715105741513"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p197153572157"><a name="p197153572157"></a><a name="p197153572157"></a>参与距离计算的底库向量个数。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1071517573156"><a name="p1071517573156"></a><a name="p1071517573156"></a>[1,2^30-1]</p>
</td>
</tr>
<tr id="row106371540187"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p39628388417"><a name="p39628388417"></a><a name="p39628388417"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p10722125214"><a name="p10722125214"></a><a name="p10722125214"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p1762116529"><a name="p1762116529"></a><a name="p1762116529"></a>存储距离结果数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p154517391451"><a name="p154517391451"></a><a name="p154517391451"></a>ny，其中<span class="parmname" id="parmname44553910519"><a name="parmname44553910519"></a><a name="parmname44553910519"></a>“ny”</span>为参与距离计算的底库向量个数。</p>
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
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a>正常运行时返回0，异常退出返回对应错误码。</p>
</td>
</tr>
</tbody>
</table>

**使用示例**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

// 辅助函数：将float转换为fp16
uint16_t float_to_fp16(float value);

int main() {
    size_t dim = 128;
    size_t total_base_vectors = 10000;
    size_t ny = 50;  // 计算50个向量的距离

    // 准备fp16格式的查询向量
    uint16_t* query_vec_fp16 = (uint16_t*)malloc(dim * sizeof(uint16_t));
    for (size_t i = 0; i < dim; i++) {
        query_vec_fp16[i] = float_to_fp16((float)(rand() % 1000) / 1000.0f);
    }

    // 准备fp16格式的底库向量
    uint16_t* base_vectors_fp16 = (uint16_t*)malloc(total_base_vectors * dim * sizeof(uint16_t));
    for (size_t i = 0; i < total_base_vectors * dim; i++) {
        base_vectors_fp16[i] = float_to_fp16((float)(rand() % 1000) / 1000.0f);
    }

    // 指定需要计算的向量ID（随机选择）
    int64_t* ids = (int64_t*)malloc(ny * sizeof(int64_t));
    for (size_t i = 0; i < ny; i++) {
        ids[i] = rand() % total_base_vectors;
    }

    // 分配距离结果数组（输出仍为float类型）
    float* distances = (float*)malloc(ny * sizeof(float));

    // 执行fp16一对多欧氏距离计算
    int ret = krl_L2sqr_by_idx_f16f32(
        distances,
        query_vec_fp16,
        base_vectors_fp16,
        ids,
        dim,
        ny,
        ny
    );

    if (ret != 0) {
        printf("fp16一对多距离计算失败，错误码: %d\n", ret);
        goto cleanup;
    }

    printf("fp16一对多欧氏距离计算成功\n");
    printf("前3个结果:\n");
    for (size_t i = 0; i < 3 && i < ny; i++) {
        printf("  向量ID[%ld]: 距离 = %f\n", ids[i], distances[i]);
    }

cleanup:
    free(query_vec_fp16);
    free(base_vectors_fp16);
    free(ids);
    free(distances);

    return ret;
}
```

### krl\_L2sqr\_by\_idx\_u8f32

**接口定义<a name="section172317194488"></a>**

int krl\_L2sqr\_by\_idx\_u8f32\(float\* dis, const uint8\_t\* x, const uint8\_t\* y, const int64\_t\* ids, size\_t d, size\_t ny, size\_t dis\_size\);

**接口用途<a name="section1153124784912"></a>**

进行数据类型为uint8的一对多欧氏距离计算。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.601460146014599%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row92301478154"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p223015479158"><a name="p223015479158"></a><a name="p223015479158"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p11230154710156"><a name="p11230154710156"></a><a name="p11230154710156"></a>float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p82303471154"><a name="p82303471154"></a><a name="p82303471154"></a>存储计算所得的距离结果。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p923018478155"><a name="p923018478155"></a><a name="p923018478155"></a>限制长度为dis_size，其中<span class="parmname" id="parmname133743422533"><a name="parmname133743422533"></a><a name="parmname133743422533"></a>“dis_size”</span>为存储距离结果数组的长度。需要预先分配内存。</p>
</td>
</tr>
<tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p953215815518"><a name="p953215815518"></a><a name="p953215815518"></a>const uint8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p18661136253"><a name="p18661136253"></a><a name="p18661136253"></a>参与距离计算的查询向量。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>限制长度为d，其中<span class="parmname" id="parmname76117481457"><a name="parmname76117481457"></a><a name="parmname76117481457"></a>“d”</span>为向量维度。</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4982142445414"><a name="p4982142445414"></a><a name="p4982142445414"></a>y</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p154911116102813"><a name="p154911116102813"></a><a name="p154911116102813"></a>const uint8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p36611261054"><a name="p36611261054"></a><a name="p36611261054"></a>参与距离计算的底库向量。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>限制长度为d*ny，其中<span class="parmname" id="parmname551215813519"><a name="parmname551215813519"></a><a name="parmname551215813519"></a>“d”</span>为向量维度，<span class="parmname" id="parmname8646142120239"><a name="parmname8646142120239"></a><a name="parmname8646142120239"></a>“ny”</span>为参与距离计算的底库向量个数。</p>
</td>
</tr>
<tr id="row103951453161513"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p1395185361518"><a name="p1395185361518"></a><a name="p1395185361518"></a>ids</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p93958532154"><a name="p93958532154"></a><a name="p93958532154"></a>const int64_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p2039510531150"><a name="p2039510531150"></a><a name="p2039510531150"></a>参与距离计算的底库向量ID。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p19345103171215"><a name="p19345103171215"></a><a name="p19345103171215"></a>限制长度为ny，其中<span class="parmname" id="parmname0410141908"><a name="parmname0410141908"></a><a name="parmname0410141908"></a>“ny”</span>为参与距离计算的底库向量个数。ID大于等于0，小于底库向量的总数。</p>
</td>
</tr>
<tr id="row106882715416"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p46812710547"><a name="p46812710547"></a><a name="p46812710547"></a>d</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p45311183519"><a name="p45311183519"></a><a name="p45311183519"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p17661261256"><a name="p17661261256"></a><a name="p17661261256"></a>向量维度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p46952755416"><a name="p46952755416"></a><a name="p46952755416"></a>[1,65535]</p>
</td>
</tr>
<tr id="row37151957141516"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p171515741513"><a name="p171515741513"></a><a name="p171515741513"></a>ny</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p3715105741513"><a name="p3715105741513"></a><a name="p3715105741513"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p197153572157"><a name="p197153572157"></a><a name="p197153572157"></a>参与距离计算的底库向量个数。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1071517573156"><a name="p1071517573156"></a><a name="p1071517573156"></a>[1,2^30-1]</p>
</td>
</tr>
<tr id="row1689332720259"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p39628388417"><a name="p39628388417"></a><a name="p39628388417"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p10722125214"><a name="p10722125214"></a><a name="p10722125214"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p1762116529"><a name="p1762116529"></a><a name="p1762116529"></a>存储距离结果数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p154517391451"><a name="p154517391451"></a><a name="p154517391451"></a>ny，其中<span class="parmname" id="parmname44553910519"><a name="parmname44553910519"></a><a name="parmname44553910519"></a>“ny”</span>为参与距离计算的底库向量个数。</p>
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
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a>正常运行时返回0，异常退出返回对应错误码。</p>
</td>
</tr>
</tbody>
</table>

**使用示例**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

int main() {
    size_t dim = 128;
    size_t total_base_vectors = 5000;
    size_t ny = 200;  // 计算200个向量的距离

    // 准备uint8类型的查询向量
    uint8_t* query_vec = (uint8_t*)malloc(dim * sizeof(uint8_t));
    for (size_t i = 0; i < dim; i++) {
        query_vec[i] = (uint8_t)(rand() % 256);
    }

    // 准备uint8类型的底库向量
    uint8_t* base_vectors = (uint8_t*)malloc(total_base_vectors * dim * sizeof(uint8_t));
    for (size_t i = 0; i < total_base_vectors * dim; i++) {
        base_vectors[i] = (uint8_t)(rand() % 256);
    }

    // 指定需要计算的向量ID
    int64_t* ids = (int64_t*)malloc(ny * sizeof(int64_t));
    for (size_t i = 0; i < ny; i++) {
        ids[i] = (int64_t)(i * 25);  // 每隔25个选一个
    }

    // 分配距离结果数组（输出为float类型）
    float* distances = (float*)malloc(ny * sizeof(float));

    // 执行uint8一对多欧氏距离计算
    int ret = krl_L2sqr_by_idx_u8f32(
        distances,
        query_vec,
        base_vectors,
        ids,
        dim,
        ny,
        ny
    );

    if (ret != 0) {
        printf("uint8一对多距离计算失败，错误码: %d\n", ret);
        goto cleanup;
    }

    printf("uint8一对多欧氏距离计算成功\n");
    
    // 找出最小距离
    float min_dist = distances[0];
    int64_t min_id = ids[0];
    for (size_t i = 1; i < ny; i++) {
        if (distances[i] < min_dist) {
            min_dist = distances[i];
            min_id = ids[i];
        }
    }
    printf("最近邻向量ID: %ld, 距离: %f\n", min_id, min_dist);

cleanup:
    free(query_vec);
    free(base_vectors);
    free(ids);
    free(distances);

    return ret;
}
```

### krl\_inner\_product\_by\_idx

**接口定义<a name="section172317194488"></a>**

int krl\_inner\_product\_by\_idx\(float\* dis, const float\* x, const float\* y, const int64\_t\* ids, size\_t d, size\_t ny, size\_t dis\_size\);

**接口用途<a name="section1153124784912"></a>**

进行数据类型为float的一对多内积距离计算。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.601460146014599%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.97339733973397%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="35.873587358735875%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row92301478154"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p223015479158"><a name="p223015479158"></a><a name="p223015479158"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p11230154710156"><a name="p11230154710156"></a><a name="p11230154710156"></a>float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.97339733973397%" headers="mcps1.1.5.1.3 "><p id="p82303471154"><a name="p82303471154"></a><a name="p82303471154"></a>存储计算所得的距离结果。</p>
</td>
<td class="cellrowborder" valign="top" width="35.873587358735875%" headers="mcps1.1.5.1.4 "><p id="p923018478155"><a name="p923018478155"></a><a name="p923018478155"></a>限制长度为dis_size，其中<span class="parmname" id="parmname133743422533"><a name="parmname133743422533"></a><a name="parmname133743422533"></a>“dis_size”</span>为存储距离结果数组的长度。需要预先分配内存。</p>
</td>
</tr>
<tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p953215815518"><a name="p953215815518"></a><a name="p953215815518"></a>const float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.97339733973397%" headers="mcps1.1.5.1.3 "><p id="p18661136253"><a name="p18661136253"></a><a name="p18661136253"></a>参与距离计算的查询向量。</p>
</td>
<td class="cellrowborder" valign="top" width="35.873587358735875%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>限制长度为d，其中<span class="parmname" id="parmname76117481457"><a name="parmname76117481457"></a><a name="parmname76117481457"></a>“d”</span>为向量维度。</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4982142445414"><a name="p4982142445414"></a><a name="p4982142445414"></a>y</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7532158856"><a name="p7532158856"></a><a name="p7532158856"></a>const float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.97339733973397%" headers="mcps1.1.5.1.3 "><p id="p36611261054"><a name="p36611261054"></a><a name="p36611261054"></a>参与距离计算的底库向量。</p>
</td>
<td class="cellrowborder" valign="top" width="35.873587358735875%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>限制长度为d*ny，其中<span class="parmname" id="parmname551215813519"><a name="parmname551215813519"></a><a name="parmname551215813519"></a>“d”</span>为向量维度，<span class="parmname" id="parmname8646142120239"><a name="parmname8646142120239"></a><a name="parmname8646142120239"></a>“ny”</span>为参与距离计算的底库向量个数。</p>
</td>
</tr>
<tr id="row103951453161513"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p1395185361518"><a name="p1395185361518"></a><a name="p1395185361518"></a>ids</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p93958532154"><a name="p93958532154"></a><a name="p93958532154"></a>const int64_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.97339733973397%" headers="mcps1.1.5.1.3 "><p id="p2039510531150"><a name="p2039510531150"></a><a name="p2039510531150"></a>参与距离计算的底库向量ID。</p>
</td>
<td class="cellrowborder" valign="top" width="35.873587358735875%" headers="mcps1.1.5.1.4 "><p id="p6395135351511"><a name="p6395135351511"></a><a name="p6395135351511"></a>限制长度为ny，其中<span class="parmname" id="parmname0410141908"><a name="parmname0410141908"></a><a name="parmname0410141908"></a>“ny”</span>为参与距离计算的底库向量个数。ID大于等于0，小于底库向量的总数。</p>
</td>
</tr>
<tr id="row106882715416"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p46812710547"><a name="p46812710547"></a><a name="p46812710547"></a>d</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p45311183519"><a name="p45311183519"></a><a name="p45311183519"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.97339733973397%" headers="mcps1.1.5.1.3 "><p id="p17661261256"><a name="p17661261256"></a><a name="p17661261256"></a>向量维度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.873587358735875%" headers="mcps1.1.5.1.4 "><p id="p46952755416"><a name="p46952755416"></a><a name="p46952755416"></a>[1,65535]</p>
</td>
</tr>
<tr id="row37151957141516"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p171515741513"><a name="p171515741513"></a><a name="p171515741513"></a>ny</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p3715105741513"><a name="p3715105741513"></a><a name="p3715105741513"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.97339733973397%" headers="mcps1.1.5.1.3 "><p id="p197153572157"><a name="p197153572157"></a><a name="p197153572157"></a>参与距离计算的底库向量个数。</p>
</td>
<td class="cellrowborder" valign="top" width="35.873587358735875%" headers="mcps1.1.5.1.4 "><p id="p1071517573156"><a name="p1071517573156"></a><a name="p1071517573156"></a>[1,2^30-1]</p>
</td>
</tr>
<tr id="row195051882311"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p39628388417"><a name="p39628388417"></a><a name="p39628388417"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p10722125214"><a name="p10722125214"></a><a name="p10722125214"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.97339733973397%" headers="mcps1.1.5.1.3 "><p id="p1762116529"><a name="p1762116529"></a><a name="p1762116529"></a>存储距离结果数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.873587358735875%" headers="mcps1.1.5.1.4 "><p id="p154517391451"><a name="p154517391451"></a><a name="p154517391451"></a>ny，其中<span class="parmname" id="parmname44553910519"><a name="parmname44553910519"></a><a name="parmname44553910519"></a>“ny”</span>为参与距离计算的底库向量个数。</p>
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
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a>正常运行时返回0，异常退出返回对应错误码。</p>
</td>
</tr>
</tbody>
</table>

**使用示例**

```c
#include <stdio.h>
#include <stdlib.h>
#include <math.h>
#include "krl.h"

// 辅助函数：向量归一化
void normalize_vector(float* vec, size_t dim) {
    float norm = 0.0f;
    for (size_t i = 0; i < dim; i++) {
        norm += vec[i] * vec[i];
    }
    norm = sqrtf(norm);
    if (norm > 0) {
        for (size_t i = 0; i < dim; i++) {
            vec[i] /= norm;
        }
    }
}

int main() {
    size_t dim = 128;
    size_t total_base_vectors = 10000;
    size_t ny = 100;

    // 准备查询向量并归一化
    float* query_vec = (float*)malloc(dim * sizeof(float));
    for (size_t i = 0; i < dim; i++) {
        query_vec[i] = (float)(rand() % 1000) / 1000.0f;
    }
    normalize_vector(query_vec, dim);

    // 准备底库向量并归一化
    float* base_vectors = (float*)malloc(total_base_vectors * dim * sizeof(float));
    for (size_t j = 0; j < total_base_vectors; j++) {
        for (size_t i = 0; i < dim; i++) {
            base_vectors[j * dim + i] = (float)(rand() % 1000) / 1000.0f;
        }
        normalize_vector(&base_vectors[j * dim], dim);
    }

    // 指定需要计算的向量ID
    int64_t* ids = (int64_t*)malloc(ny * sizeof(int64_t));
    for (size_t i = 0; i < ny; i++) {
        ids[i] = rand() % total_base_vectors;
    }

    // 分配距离结果数组
    float* distances = (float*)malloc(ny * sizeof(float));

    // 执行一对多内积距离计算
    int ret = krl_inner_product_by_idx(
        distances,
        query_vec,
        base_vectors,
        ids,
        dim,
        ny,
        ny
    );

    if (ret != 0) {
        printf("一对多内积距离计算失败，错误码: %d\n", ret);
        goto cleanup;
    }

    printf("一对多内积距离计算成功\n");
    
    // 对于归一化向量，内积值越大表示越相似
    // 找出最大内积（最相似）
    float max_ip = distances[0];
    int64_t max_id = ids[0];
    for (size_t i = 1; i < ny; i++) {
        if (distances[i] > max_ip) {
            max_ip = distances[i];
            max_id = ids[i];
        }
    }
    printf("最相似向量ID: %ld, 内积值: %f\n", max_id, max_ip);

cleanup:
    free(query_vec);
    free(base_vectors);
    free(ids);
    free(distances);

    return ret;
}
```

### krl\_inner\_product\_by\_idx\_f16f32

**接口定义<a name="section172317194488"></a>**

int krl\_inner\_product\_by\_idx\_f16f32\(float\* dis, const uint16\_t\* x, const uint16\_t\* y, const int64\_t\* ids, size\_t d, size\_t ny, size\_t dis\_size\);

**接口用途<a name="section1153124784912"></a>**

进行数据类型为fp16的一对多内积距离计算。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.601460146014599%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.663366336633665%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="36.18361836183618%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row92301478154"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p223015479158"><a name="p223015479158"></a><a name="p223015479158"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p11230154710156"><a name="p11230154710156"></a><a name="p11230154710156"></a>float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.663366336633665%" headers="mcps1.1.5.1.3 "><p id="p82303471154"><a name="p82303471154"></a><a name="p82303471154"></a>存储计算所得的距离结果。</p>
</td>
<td class="cellrowborder" valign="top" width="36.18361836183618%" headers="mcps1.1.5.1.4 "><p id="p923018478155"><a name="p923018478155"></a><a name="p923018478155"></a>限制长度为dis_size，其中<span class="parmname" id="parmname133743422533"><a name="parmname133743422533"></a><a name="parmname133743422533"></a>“dis_size”</span>为存储距离结果数组的长度。需要预先分配内存。</p>
</td>
</tr>
<tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p953215815518"><a name="p953215815518"></a><a name="p953215815518"></a>const uint16_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.663366336633665%" headers="mcps1.1.5.1.3 "><p id="p18661136253"><a name="p18661136253"></a><a name="p18661136253"></a>参与距离计算的查询向量。</p>
</td>
<td class="cellrowborder" valign="top" width="36.18361836183618%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>限制长度为d，其中<span class="parmname" id="parmname76117481457"><a name="parmname76117481457"></a><a name="parmname76117481457"></a>“d”</span>为向量维度。</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4982142445414"><a name="p4982142445414"></a><a name="p4982142445414"></a>y</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7532158856"><a name="p7532158856"></a><a name="p7532158856"></a>const uint16_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.663366336633665%" headers="mcps1.1.5.1.3 "><p id="p36611261054"><a name="p36611261054"></a><a name="p36611261054"></a>参与距离计算的底库向量。</p>
</td>
<td class="cellrowborder" valign="top" width="36.18361836183618%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>限制长度为d*ny，其中<span class="parmname" id="parmname551215813519"><a name="parmname551215813519"></a><a name="parmname551215813519"></a>“d”</span>为向量维度，<span class="parmname" id="parmname8646142120239"><a name="parmname8646142120239"></a><a name="parmname8646142120239"></a>“ny”</span>为参与距离计算的底库向量个数。</p>
</td>
</tr>
<tr id="row103951453161513"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p1395185361518"><a name="p1395185361518"></a><a name="p1395185361518"></a>ids</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p93958532154"><a name="p93958532154"></a><a name="p93958532154"></a>const int64_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.663366336633665%" headers="mcps1.1.5.1.3 "><p id="p2039510531150"><a name="p2039510531150"></a><a name="p2039510531150"></a>参与距离计算的底库向量ID。</p>
</td>
<td class="cellrowborder" valign="top" width="36.18361836183618%" headers="mcps1.1.5.1.4 "><p id="p6395135351511"><a name="p6395135351511"></a><a name="p6395135351511"></a>限制长度为ny，其中<span class="parmname" id="parmname0410141908"><a name="parmname0410141908"></a><a name="parmname0410141908"></a>“ny”</span>为参与距离计算的底库向量个数。ID大于等于0，小于底库向量的总数。</p>
</td>
</tr>
<tr id="row106882715416"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p46812710547"><a name="p46812710547"></a><a name="p46812710547"></a>d</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p45311183519"><a name="p45311183519"></a><a name="p45311183519"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.663366336633665%" headers="mcps1.1.5.1.3 "><p id="p17661261256"><a name="p17661261256"></a><a name="p17661261256"></a>向量维度。</p>
</td>
<td class="cellrowborder" valign="top" width="36.18361836183618%" headers="mcps1.1.5.1.4 "><p id="p46952755416"><a name="p46952755416"></a><a name="p46952755416"></a>[1,65535]</p>
</td>
</tr>
<tr id="row37151957141516"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p171515741513"><a name="p171515741513"></a><a name="p171515741513"></a>ny</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p3715105741513"><a name="p3715105741513"></a><a name="p3715105741513"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.663366336633665%" headers="mcps1.1.5.1.3 "><p id="p197153572157"><a name="p197153572157"></a><a name="p197153572157"></a>参与距离计算的底库向量个数。</p>
</td>
<td class="cellrowborder" valign="top" width="36.18361836183618%" headers="mcps1.1.5.1.4 "><p id="p1071517573156"><a name="p1071517573156"></a><a name="p1071517573156"></a>[1,2^30-1]</p>
</td>
</tr>
<tr id="row36562453314"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p39628388417"><a name="p39628388417"></a><a name="p39628388417"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p10722125214"><a name="p10722125214"></a><a name="p10722125214"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.663366336633665%" headers="mcps1.1.5.1.3 "><p id="p1762116529"><a name="p1762116529"></a><a name="p1762116529"></a>存储距离结果数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="36.18361836183618%" headers="mcps1.1.5.1.4 "><p id="p154517391451"><a name="p154517391451"></a><a name="p154517391451"></a>ny，其中<span class="parmname" id="parmname44553910519"><a name="parmname44553910519"></a><a name="parmname44553910519"></a>“ny”</span>为参与距离计算的底库向量个数。</p>
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
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a>正常运行时返回0，异常退出返回对应错误码。</p>
</td>
</tr>
</tbody>
</table>

**使用示例**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

// 辅助函数：将float转换为fp16
uint16_t float_to_fp16(float value);

int main() {
    size_t dim = 256;
    size_t total_base_vectors = 8000;
    size_t ny = 64;

    // 准备fp16格式的查询向量
    uint16_t* query_vec_fp16 = (uint16_t*)malloc(dim * sizeof(uint16_t));
    for (size_t i = 0; i < dim; i++) {
        query_vec_fp16[i] = float_to_fp16(0.1f);
    }

    // 准备fp16格式的底库向量
    uint16_t* base_vectors_fp16 = (uint16_t*)malloc(total_base_vectors * dim * sizeof(uint16_t));
    for (size_t i = 0; i < total_base_vectors * dim; i++) {
        base_vectors_fp16[i] = float_to_fp16((float)(rand() % 100) / 100.0f);
    }

    // 指定需要计算的向量ID
    int64_t* ids = (int64_t*)malloc(ny * sizeof(int64_t));
    for (size_t i = 0; i < ny; i++) {
        ids[i] = (int64_t)(i * 100);
    }

    // 分配距离结果数组
    float* distances = (float*)malloc(ny * sizeof(float));

    // 执行fp16一对多内积距离计算
    int ret = krl_inner_product_by_idx_f16f32(
        distances,
        query_vec_fp16,
        base_vectors_fp16,
        ids,
        dim,
        ny,
        ny
    );

    if (ret != 0) {
        printf("fp16一对多内积距离计算失败，错误码: %d\n", ret);
        goto cleanup;
    }

    printf("fp16一对多内积距离计算成功\n");
    printf("前5个结果:\n");
    for (size_t i = 0; i < 5 && i < ny; i++) {
        printf("  向量ID[%ld]: 内积 = %f\n", ids[i], distances[i]);
    }

cleanup:
    free(query_vec_fp16);
    free(base_vectors_fp16);
    free(ids);
    free(distances);

    return ret;
}
```

### krl\_negative\_inner\_product\_by\_idx\_f16f32

**接口定义<a name="section172317194488"></a>**

int krl\_negative\_inner\_product\_by\_idx\_f16f32\(float\* dis, const uint16\_t\* x, const uint16\_t\* y, const int64\_t\* ids, size\_t d, size\_t ny, size\_t dis\_size\);

**接口用途<a name="section1153124784912"></a>**

进行数据类型为fp16的一对多内积距离计算，对结果取反。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.661466146614663%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.93339333933393%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row92301478154"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p223015479158"><a name="p223015479158"></a><a name="p223015479158"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.661466146614663%" headers="mcps1.1.5.1.2 "><p id="p11230154710156"><a name="p11230154710156"></a><a name="p11230154710156"></a>float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.93339333933393%" headers="mcps1.1.5.1.3 "><p id="p82303471154"><a name="p82303471154"></a><a name="p82303471154"></a>存储计算所得的距离结果。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p923018478155"><a name="p923018478155"></a><a name="p923018478155"></a>限制长度为dis_size，其中<span class="parmname" id="parmname133743422533"><a name="parmname133743422533"></a><a name="parmname133743422533"></a>“dis_size”</span>为存储距离结果数组的长度。需要预先分配内存。</p>
</td>
</tr>
<tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="14.661466146614663%" headers="mcps1.1.5.1.2 "><p id="p953215815518"><a name="p953215815518"></a><a name="p953215815518"></a>const uint16_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.93339333933393%" headers="mcps1.1.5.1.3 "><p id="p18661136253"><a name="p18661136253"></a><a name="p18661136253"></a>参与距离计算的查询向量。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>限制长度为d，其中<span class="parmname" id="parmname76117481457"><a name="parmname76117481457"></a><a name="parmname76117481457"></a>“d”</span>为向量维度。</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4982142445414"><a name="p4982142445414"></a><a name="p4982142445414"></a>y</p>
</td>
<td class="cellrowborder" valign="top" width="14.661466146614663%" headers="mcps1.1.5.1.2 "><p id="p7532158856"><a name="p7532158856"></a><a name="p7532158856"></a>const uint16_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.93339333933393%" headers="mcps1.1.5.1.3 "><p id="p36611261054"><a name="p36611261054"></a><a name="p36611261054"></a>参与距离计算的底库向量。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>限制长度为d*ny，其中<span class="parmname" id="parmname551215813519"><a name="parmname551215813519"></a><a name="parmname551215813519"></a>“d”</span>为向量维度，<span class="parmname" id="parmname8646142120239"><a name="parmname8646142120239"></a><a name="parmname8646142120239"></a>“ny”</span>为参与距离计算的底库向量个数。</p>
</td>
</tr>
<tr id="row103951453161513"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p1395185361518"><a name="p1395185361518"></a><a name="p1395185361518"></a>ids</p>
</td>
<td class="cellrowborder" valign="top" width="14.661466146614663%" headers="mcps1.1.5.1.2 "><p id="p93958532154"><a name="p93958532154"></a><a name="p93958532154"></a>const int64_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.93339333933393%" headers="mcps1.1.5.1.3 "><p id="p2039510531150"><a name="p2039510531150"></a><a name="p2039510531150"></a>参与距离计算的底库向量ID。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p6395135351511"><a name="p6395135351511"></a><a name="p6395135351511"></a>限制长度为ny，其中<span class="parmname" id="parmname0410141908"><a name="parmname0410141908"></a><a name="parmname0410141908"></a>“ny”</span>为参与距离计算的底库向量个数。ID大于等于0，小于底库向量的总数。</p>
</td>
</tr>
<tr id="row106882715416"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p46812710547"><a name="p46812710547"></a><a name="p46812710547"></a>d</p>
</td>
<td class="cellrowborder" valign="top" width="14.661466146614663%" headers="mcps1.1.5.1.2 "><p id="p45311183519"><a name="p45311183519"></a><a name="p45311183519"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.93339333933393%" headers="mcps1.1.5.1.3 "><p id="p17661261256"><a name="p17661261256"></a><a name="p17661261256"></a>向量维度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p46952755416"><a name="p46952755416"></a><a name="p46952755416"></a>[1,65535]</p>
</td>
</tr>
<tr id="row37151957141516"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p171515741513"><a name="p171515741513"></a><a name="p171515741513"></a>ny</p>
</td>
<td class="cellrowborder" valign="top" width="14.661466146614663%" headers="mcps1.1.5.1.2 "><p id="p3715105741513"><a name="p3715105741513"></a><a name="p3715105741513"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.93339333933393%" headers="mcps1.1.5.1.3 "><p id="p197153572157"><a name="p197153572157"></a><a name="p197153572157"></a>参与距离计算的底库向量个数。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1071517573156"><a name="p1071517573156"></a><a name="p1071517573156"></a>[1,2^30-1]</p>
</td>
</tr>
<tr id="row17278128173918"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p39628388417"><a name="p39628388417"></a><a name="p39628388417"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.661466146614663%" headers="mcps1.1.5.1.2 "><p id="p10722125214"><a name="p10722125214"></a><a name="p10722125214"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.93339333933393%" headers="mcps1.1.5.1.3 "><p id="p1762116529"><a name="p1762116529"></a><a name="p1762116529"></a>存储距离结果数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p154517391451"><a name="p154517391451"></a><a name="p154517391451"></a>ny，其中<span class="parmname" id="parmname44553910519"><a name="parmname44553910519"></a><a name="parmname44553910519"></a>“ny”</span>为参与距离计算的底库向量个数。</p>
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
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a>正常运行时返回0，异常退出返回对应错误码。</p>
</td>
</tr>
</tbody>
</table>

**使用示例**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

// 辅助函数：将float转换为fp16
uint16_t float_to_fp16(float value);

int main() {
    size_t dim = 128;
    size_t total_base_vectors = 5000;
    size_t ny = 100;

    // 准备fp16格式的查询向量
    uint16_t* query_vec_fp16 = (uint16_t*)malloc(dim * sizeof(uint16_t));
    for (size_t i = 0; i < dim; i++) {
        query_vec_fp16[i] = float_to_fp16(0.5f);
    }

    // 准备fp16格式的底库向量
    uint16_t* base_vectors_fp16 = (uint16_t*)malloc(total_base_vectors * dim * sizeof(uint16_t));
    for (size_t i = 0; i < total_base_vectors * dim; i++) {
        base_vectors_fp16[i] = float_to_fp16((float)(rand() % 100) / 100.0f);
    }

    // 指定需要计算的向量ID
    int64_t* ids = (int64_t*)malloc(ny * sizeof(int64_t));
    for (size_t i = 0; i < ny; i++) {
        ids[i] = rand() % total_base_vectors;
    }

    // 分配距离结果数组
    float* distances = (float*)malloc(ny * sizeof(float));

    // 执行fp16一对多负内积距离计算
    // 注意：结果是内积的负值，可直接用于最小堆排序找最相似向量
    int ret = krl_negative_inner_product_by_idx_f16f32(
        distances,
        query_vec_fp16,
        base_vectors_fp16,
        ids,
        dim,
        ny,
        ny
    );

    if (ret != 0) {
        printf("fp16一对多负内积距离计算失败，错误码: %d\n", ret);
        goto cleanup;
    }

    printf("fp16一对多负内积距离计算成功\n");
    
    // 使用负内积时，值越小表示原始内积越大（越相似）
    // 因此可以直接使用最小值找最相似向量
    float min_neg_ip = distances[0];
    int64_t most_similar_id = ids[0];
    for (size_t i = 1; i < ny; i++) {
        if (distances[i] < min_neg_ip) {
            min_neg_ip = distances[i];
            most_similar_id = ids[i];
        }
    }
    
    printf("最相似向量ID: %ld\n", most_similar_id);
    printf("负内积值: %f (原始内积: %f)\n", min_neg_ip, -min_neg_ip);

cleanup:
    free(query_vec_fp16);
    free(base_vectors_fp16);
    free(ids);
    free(distances);

    return ret;
}
```

### krl\_inner\_product\_by\_idx\_s8f32

**接口定义<a name="section172317194488"></a>**

int krl\_inner\_product\_by\_idx\_s8f32\(float\* dis, const int8\_t\* x, const int8\_t\* y, const int64\_t\* ids, size\_t d, size\_t ny, size\_t dis\_size\);

**接口用途<a name="section1153124784912"></a>**

进行数据类型为int8的一对多内积距离计算。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.601460146014599%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row92301478154"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p223015479158"><a name="p223015479158"></a><a name="p223015479158"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p11230154710156"><a name="p11230154710156"></a><a name="p11230154710156"></a>float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p82303471154"><a name="p82303471154"></a><a name="p82303471154"></a>存储计算所得的距离结果。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p923018478155"><a name="p923018478155"></a><a name="p923018478155"></a>限制长度为dis_size，其中<span class="parmname" id="parmname133743422533"><a name="parmname133743422533"></a><a name="parmname133743422533"></a>“dis_size”</span>为存储距离结果数组的长度。需要预先分配内存。</p>
</td>
</tr>
<tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p953215815518"><a name="p953215815518"></a><a name="p953215815518"></a>const int8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p18661136253"><a name="p18661136253"></a><a name="p18661136253"></a>参与距离计算的查询向量。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>限制长度为d，其中<span class="parmname" id="parmname76117481457"><a name="parmname76117481457"></a><a name="parmname76117481457"></a>“d”</span>为向量维度。</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4982142445414"><a name="p4982142445414"></a><a name="p4982142445414"></a>y</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p154911116102813"><a name="p154911116102813"></a><a name="p154911116102813"></a>const int8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p36611261054"><a name="p36611261054"></a><a name="p36611261054"></a>参与距离计算的底库向量。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>限制长度为d*ny，其中<span class="parmname" id="parmname551215813519"><a name="parmname551215813519"></a><a name="parmname551215813519"></a>“d”</span>为向量维度，<span class="parmname" id="parmname8646142120239"><a name="parmname8646142120239"></a><a name="parmname8646142120239"></a>“ny”</span>为参与距离计算的底库向量个数。</p>
</td>
</tr>
<tr id="row103951453161513"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p1395185361518"><a name="p1395185361518"></a><a name="p1395185361518"></a>ids</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p93958532154"><a name="p93958532154"></a><a name="p93958532154"></a>const int64_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p2039510531150"><a name="p2039510531150"></a><a name="p2039510531150"></a>参与距离计算的底库向量ID。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p6395135351511"><a name="p6395135351511"></a><a name="p6395135351511"></a>限制长度为ny，其中<span class="parmname" id="parmname0410141908"><a name="parmname0410141908"></a><a name="parmname0410141908"></a>“ny”</span>为参与距离计算的底库向量个数。ID大于等于0，小于底库向量的总数。</p>
</td>
</tr>
<tr id="row106882715416"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p46812710547"><a name="p46812710547"></a><a name="p46812710547"></a>d</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p45311183519"><a name="p45311183519"></a><a name="p45311183519"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p17661261256"><a name="p17661261256"></a><a name="p17661261256"></a>向量维度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p46952755416"><a name="p46952755416"></a><a name="p46952755416"></a>[1,65535]</p>
</td>
</tr>
<tr id="row37151957141516"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p171515741513"><a name="p171515741513"></a><a name="p171515741513"></a>ny</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p3715105741513"><a name="p3715105741513"></a><a name="p3715105741513"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p197153572157"><a name="p197153572157"></a><a name="p197153572157"></a>参与距离计算的底库向量个数。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1071517573156"><a name="p1071517573156"></a><a name="p1071517573156"></a>[1,2^30-1]</p>
</td>
</tr>
<tr id="row5987191044118"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p39628388417"><a name="p39628388417"></a><a name="p39628388417"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p10722125214"><a name="p10722125214"></a><a name="p10722125214"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p1762116529"><a name="p1762116529"></a><a name="p1762116529"></a>存储距离结果数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p154517391451"><a name="p154517391451"></a><a name="p154517391451"></a>ny，其中<span class="parmname" id="parmname44553910519"><a name="parmname44553910519"></a><a name="parmname44553910519"></a>“ny”</span>为参与距离计算的底库向量个数。</p>
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
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a>正常运行时返回0，异常退出返回对应错误码。</p>
</td>
</tr>
</tbody>
</table>

**使用示例**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

int main() {
    size_t dim = 128;
    size_t total_base_vectors = 10000;
    size_t ny = 100;

    // 准备int8类型的查询向量
    int8_t* query_vec = (int8_t*)malloc(dim * sizeof(int8_t));
    for (size_t i = 0; i < dim; i++) {
        query_vec[i] = (int8_t)(rand() % 256 - 128);
    }

    // 准备int8类型的底库向量
    int8_t* base_vectors = (int8_t*)malloc(total_base_vectors * dim * sizeof(int8_t));
    for (size_t i = 0; i < total_base_vectors * dim; i++) {
        base_vectors[i] = (int8_t)(rand() % 256 - 128);
    }

    // 指定需要计算的向量ID
    int64_t* ids = (int64_t*)malloc(ny * sizeof(int64_t));
    for (size_t i = 0; i < ny; i++) {
        ids[i] = rand() % total_base_vectors;
    }

    // 分配距离结果数组（输出为float类型）
    float* distances = (float*)malloc(ny * sizeof(float));

    // 执行int8一对多内积距离计算
    int ret = krl_inner_product_by_idx_s8f32(
        distances,
        query_vec,
        base_vectors,
        ids,
        dim,
        ny,
        ny
    );

    if (ret != 0) {
        printf("int8一对多内积距离计算失败，错误码: %d\n", ret);
        goto cleanup;
    }

    printf("int8一对多内积距离计算成功\n");
    printf("前5个结果:\n");
    for (size_t i = 0; i < 5 && i < ny; i++) {
        printf("  向量ID[%ld]: 内积 = %f\n", ids[i], distances[i]);
    }

cleanup:
    free(query_vec);
    free(base_vectors);
    free(ids);
    free(distances);

    return ret;
}
```

### krl\_L2sqr\_ny

**接口定义<a name="section172317194488"></a>**

int krl\_L2sqr\_ny\(float\* dis, const float\* x, const float\* y, size\_t ny, size\_t d, size\_t dis\_size\);

**接口用途<a name="section1153124784912"></a>**

进行数据类型为float的一对多欧氏距离计算。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.601460146014599%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row92301478154"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p223015479158"><a name="p223015479158"></a><a name="p223015479158"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p11230154710156"><a name="p11230154710156"></a><a name="p11230154710156"></a>float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p82303471154"><a name="p82303471154"></a><a name="p82303471154"></a>存储计算所得的距离结果。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p923018478155"><a name="p923018478155"></a><a name="p923018478155"></a>限制长度为dis_size，其中<span class="parmname" id="parmname133743422533"><a name="parmname133743422533"></a><a name="parmname133743422533"></a>“dis_size”</span>为存储距离结果数组的长度。需要预先分配内存。</p>
</td>
</tr>
<tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p953215815518"><a name="p953215815518"></a><a name="p953215815518"></a>const float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p18661136253"><a name="p18661136253"></a><a name="p18661136253"></a>参与距离计算的查询向量。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>限制长度为d，其中<span class="parmname" id="parmname76117481457"><a name="parmname76117481457"></a><a name="parmname76117481457"></a>“d”</span>为向量维度。</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4982142445414"><a name="p4982142445414"></a><a name="p4982142445414"></a>y</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7532158856"><a name="p7532158856"></a><a name="p7532158856"></a>const float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p36611261054"><a name="p36611261054"></a><a name="p36611261054"></a>参与距离计算的底库向量。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>限制长度为d*ny，其中<span class="parmname" id="parmname551215813519"><a name="parmname551215813519"></a><a name="parmname551215813519"></a>“d”</span>为向量维度，<span class="parmname" id="parmname8646142120239"><a name="parmname8646142120239"></a><a name="parmname8646142120239"></a>“ny”</span>为参与距离计算的底库向量个数。</p>
</td>
</tr>
<tr id="row103951453161513"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p14723141215409"><a name="p14723141215409"></a><a name="p14723141215409"></a>ny</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p4723181210404"><a name="p4723181210404"></a><a name="p4723181210404"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p672341218403"><a name="p672341218403"></a><a name="p672341218403"></a>参与距离计算的底库向量个数。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p6723181274010"><a name="p6723181274010"></a><a name="p6723181274010"></a>[1,2^30-1]</p>
</td>
</tr>
<tr id="row106882715416"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p46812710547"><a name="p46812710547"></a><a name="p46812710547"></a>d</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p45311183519"><a name="p45311183519"></a><a name="p45311183519"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p17661261256"><a name="p17661261256"></a><a name="p17661261256"></a>向量维度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p46952755416"><a name="p46952755416"></a><a name="p46952755416"></a>[1,65535]</p>
</td>
</tr>
<tr id="row161414323423"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p39628388417"><a name="p39628388417"></a><a name="p39628388417"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p10722125214"><a name="p10722125214"></a><a name="p10722125214"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p1762116529"><a name="p1762116529"></a><a name="p1762116529"></a>存储距离结果数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p154517391451"><a name="p154517391451"></a><a name="p154517391451"></a>ny，其中<span class="parmname" id="parmname44553910519"><a name="parmname44553910519"></a><a name="parmname44553910519"></a>“ny”</span>为参与距离计算的底库向量个数。</p>
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
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a>正常运行时返回0，异常退出返回对应错误码。</p>
</td>
</tr>
</tbody>
</table>

**使用示例**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

int main() {
    size_t dim = 128;
    size_t ny = 1000;  // 底库向量数量

    // 准备查询向量
    float* query_vec = (float*)malloc(dim * sizeof(float));
    for (size_t i = 0; i < dim; i++) {
        query_vec[i] = (float)(rand() % 1000) / 1000.0f;
    }

    // 准备底库向量（连续存储）
    float* base_vectors = (float*)malloc(ny * dim * sizeof(float));
    for (size_t i = 0; i < ny * dim; i++) {
        base_vectors[i] = (float)(rand() % 1000) / 1000.0f;
    }

    // 分配距离结果数组
    float* distances = (float*)malloc(ny * sizeof(float));

    // 执行一对多欧氏距离计算（计算与所有ny个向量的距离）
    int ret = krl_L2sqr_ny(
        distances,      // 输出
        query_vec,      // 查询向量
        base_vectors,   // 底库向量（连续存储）
        ny,             // 底库向量数量
        dim,            // 维度
        ny              // 结果数组长度
    );

    if (ret != 0) {
        printf("一对多欧氏距离计算失败，错误码: %d\n", ret);
        goto cleanup;
    }

    // 找出最近邻
    float min_dist = distances[0];
    size_t min_idx = 0;
    for (size_t i = 1; i < ny; i++) {
        if (distances[i] < min_dist) {
            min_dist = distances[i];
            min_idx = i;
        }
    }

    printf("最近邻: 向量索引=%zu, 距离=%f\n", min_idx, min_dist);

cleanup:
    free(query_vec);
    free(base_vectors);
    free(distances);

    return ret;
}
```

### krl\_L2sqr\_ny\_f16f32

**接口定义<a name="section172317194488"></a>**

in krl\_L2sqr\_ny\_f16f32\(float\* dis, const uint16\_t\* x, const uint16\_t\* y, size\_t ny, size\_t d, size\_t dis\_size\);

**接口用途<a name="section1153124784912"></a>**

进行数据类型为fp16的一对多欧氏距离计算。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.601460146014599%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row92301478154"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p223015479158"><a name="p223015479158"></a><a name="p223015479158"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p11230154710156"><a name="p11230154710156"></a><a name="p11230154710156"></a>float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p82303471154"><a name="p82303471154"></a><a name="p82303471154"></a>存储计算所得的距离结果。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p923018478155"><a name="p923018478155"></a><a name="p923018478155"></a>限制长度为dis_size，其中<span class="parmname" id="parmname133743422533"><a name="parmname133743422533"></a><a name="parmname133743422533"></a>“dis_size”</span>为存储距离结果数组的长度。需要预先分配内存。</p>
</td>
</tr>
<tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p953215815518"><a name="p953215815518"></a><a name="p953215815518"></a>const uint16_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p18661136253"><a name="p18661136253"></a><a name="p18661136253"></a>参与距离计算的查询向量。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>限制长度为d，其中<span class="parmname" id="parmname76117481457"><a name="parmname76117481457"></a><a name="parmname76117481457"></a>“d”</span>为向量维度。</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4982142445414"><a name="p4982142445414"></a><a name="p4982142445414"></a>y</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7532158856"><a name="p7532158856"></a><a name="p7532158856"></a>const uint16_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p36611261054"><a name="p36611261054"></a><a name="p36611261054"></a>参与距离计算的底库向量。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>限制长度为d*ny，其中<span class="parmname" id="parmname551215813519"><a name="parmname551215813519"></a><a name="parmname551215813519"></a>“d”</span>为向量维度，<span class="parmname" id="parmname8646142120239"><a name="parmname8646142120239"></a><a name="parmname8646142120239"></a>“ny”</span>为参与距离计算的底库向量个数。</p>
</td>
</tr>
<tr id="row103951453161513"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p14723141215409"><a name="p14723141215409"></a><a name="p14723141215409"></a>ny</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p4723181210404"><a name="p4723181210404"></a><a name="p4723181210404"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p672341218403"><a name="p672341218403"></a><a name="p672341218403"></a>参与距离计算的底库向量个数。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p6723181274010"><a name="p6723181274010"></a><a name="p6723181274010"></a>[1,2^30-1]</p>
</td>
</tr>
<tr id="row106882715416"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p46812710547"><a name="p46812710547"></a><a name="p46812710547"></a>d</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p45311183519"><a name="p45311183519"></a><a name="p45311183519"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p17661261256"><a name="p17661261256"></a><a name="p17661261256"></a>向量维度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p46952755416"><a name="p46952755416"></a><a name="p46952755416"></a>[1,65535]</p>
</td>
</tr>
<tr id="row1922192114518"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p39628388417"><a name="p39628388417"></a><a name="p39628388417"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p10722125214"><a name="p10722125214"></a><a name="p10722125214"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p1762116529"><a name="p1762116529"></a><a name="p1762116529"></a>存储距离结果数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p154517391451"><a name="p154517391451"></a><a name="p154517391451"></a>ny，其中<span class="parmname" id="parmname44553910519"><a name="parmname44553910519"></a><a name="parmname44553910519"></a>“ny”</span>为参与距离计算的底库向量个数。</p>
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
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a>正常运行时返回0，异常退出返回对应错误码。</p>
</td>
</tr>
</tbody>
</table>

**使用示例**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

// 辅助函数：将float转换为fp16
uint16_t float_to_fp16(float value);

int main() {
    size_t dim = 128;
    size_t ny = 500;

    // 准备fp16格式的查询向量
    uint16_t* query_vec_fp16 = (uint16_t*)malloc(dim * sizeof(uint16_t));
    for (size_t i = 0; i < dim; i++) {
        query_vec_fp16[i] = float_to_fp16((float)(rand() % 100) / 100.0f);
    }

    // 准备fp16格式的底库向量
    uint16_t* base_vectors_fp16 = (uint16_t*)malloc(ny * dim * sizeof(uint16_t));
    for (size_t i = 0; i < ny * dim; i++) {
        base_vectors_fp16[i] = float_to_fp16((float)(rand() % 100) / 100.0f);
    }

    // 分配距离结果数组
    float* distances = (float*)malloc(ny * sizeof(float));

    // 执行fp16一对多欧氏距离计算
    int ret = krl_L2sqr_ny_f16f32(
        distances,
        query_vec_fp16,
        base_vectors_fp16,
        ny,
        dim,
        ny
    );

    if (ret != 0) {
        printf("fp16一对多欧氏距离计算失败，错误码: %d\n", ret);
        goto cleanup;
    }

    printf("fp16一对多欧氏距离计算成功，共计算%zu个向量\n", ny);

cleanup:
    free(query_vec_fp16);
    free(base_vectors_fp16);
    free(distances);

    return ret;
}
```

### krl\_L2sqr\_ny\_u8f32

**接口定义<a name="section172317194488"></a>**

void krl\_L2sqr\_ny\_u8f32\(float\* dis, const uint8\_t\* x, const uint8\_t\* y, size\_t ny, size\_t d, size\_t dis\_size\);

**接口用途<a name="section1153124784912"></a>**

进行数据类型为uint8的一对多欧氏距离计算。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.601460146014599%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row92301478154"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p223015479158"><a name="p223015479158"></a><a name="p223015479158"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p11230154710156"><a name="p11230154710156"></a><a name="p11230154710156"></a>float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p82303471154"><a name="p82303471154"></a><a name="p82303471154"></a>存储计算所得的距离结果。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p923018478155"><a name="p923018478155"></a><a name="p923018478155"></a>限制长度为dis_size，其中<span class="parmname" id="parmname133743422533"><a name="parmname133743422533"></a><a name="parmname133743422533"></a>“dis_size”</span>为存储距离结果数组的长度。需要预先分配内存。</p>
</td>
</tr>
<tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p953215815518"><a name="p953215815518"></a><a name="p953215815518"></a>const uint8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p18661136253"><a name="p18661136253"></a><a name="p18661136253"></a>参与距离计算的查询向量。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>限制长度为d，其中<span class="parmname" id="parmname76117481457"><a name="parmname76117481457"></a><a name="parmname76117481457"></a>“d”</span>为向量维度。</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4982142445414"><a name="p4982142445414"></a><a name="p4982142445414"></a>y</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7532158856"><a name="p7532158856"></a><a name="p7532158856"></a>const uint8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p36611261054"><a name="p36611261054"></a><a name="p36611261054"></a>参与距离计算的底库向量。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>限制长度为d*ny，其中<span class="parmname" id="parmname551215813519"><a name="parmname551215813519"></a><a name="parmname551215813519"></a>“d”</span>为向量维度，<span class="parmname" id="parmname8646142120239"><a name="parmname8646142120239"></a><a name="parmname8646142120239"></a>“ny”</span>为参与距离计算的底库向量个数。</p>
</td>
</tr>
<tr id="row103951453161513"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p14723141215409"><a name="p14723141215409"></a><a name="p14723141215409"></a>ny</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p4723181210404"><a name="p4723181210404"></a><a name="p4723181210404"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p672341218403"><a name="p672341218403"></a><a name="p672341218403"></a>参与距离计算的底库向量个数。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p6723181274010"><a name="p6723181274010"></a><a name="p6723181274010"></a>[1,2^30-1]</p>
</td>
</tr>
<tr id="row106882715416"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p46812710547"><a name="p46812710547"></a><a name="p46812710547"></a>d</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p45311183519"><a name="p45311183519"></a><a name="p45311183519"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p17661261256"><a name="p17661261256"></a><a name="p17661261256"></a>向量维度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p46952755416"><a name="p46952755416"></a><a name="p46952755416"></a>[1,65535]</p>
</td>
</tr>
<tr id="row882011193585"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p39628388417"><a name="p39628388417"></a><a name="p39628388417"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p10722125214"><a name="p10722125214"></a><a name="p10722125214"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p1762116529"><a name="p1762116529"></a><a name="p1762116529"></a>存储距离结果数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p154517391451"><a name="p154517391451"></a><a name="p154517391451"></a>ny，其中<span class="parmname" id="parmname44553910519"><a name="parmname44553910519"></a><a name="parmname44553910519"></a>“ny”</span>为参与距离计算的底库向量个数。</p>
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
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a>正常运行时返回0，异常退出返回对应错误码。</p>
</td>
</tr>
</tbody>
</table>

**使用示例**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

int main() {
    size_t dim = 128;
    size_t ny = 1000;

    // 准备uint8类型的查询向量
    uint8_t* query_vec = (uint8_t*)malloc(dim * sizeof(uint8_t));
    for (size_t i = 0; i < dim; i++) {
        query_vec[i] = (uint8_t)(rand() % 256);
    }

    // 准备uint8类型的底库向量
    uint8_t* base_vectors = (uint8_t*)malloc(ny * dim * sizeof(uint8_t));
    for (size_t i = 0; i < ny * dim; i++) {
        base_vectors[i] = (uint8_t)(rand() % 256);
    }

    // 分配距离结果数组
    float* distances = (float*)malloc(ny * sizeof(float));

    // 执行uint8一对多欧氏距离计算
    krl_L2sqr_ny_u8f32(
        distances,
        query_vec,
        base_vectors,
        ny,
        dim,
        ny
    );

    printf("uint8一对多欧氏距离计算完成\n");

    // 统计结果
    float sum = 0.0f;
    for (size_t i = 0; i < ny; i++) {
        sum += distances[i];
    }
    printf("平均距离: %f\n", sum / ny);

    free(query_vec);
    free(base_vectors);
    free(distances);

    return 0;
}
```

### krl\_L2sqr\_ny\_with\_handle

**接口定义<a name="section172317194488"></a>**

int krl\_L2sqr\_ny\_with\_handle\(const KRLDistanceHandle\* kdh, float\* dis, const float\* x, size\_t dis\_size, size\_t x\_size\);

**接口用途<a name="section1153124784912"></a>**

进行数据类型为float的一对多欧氏距离计算，底库向量与维度存储于Handle中。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.601460146014599%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row92301478154"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p223015479158"><a name="p223015479158"></a><a name="p223015479158"></a>kdh</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p11230154710156"><a name="p11230154710156"></a><a name="p11230154710156"></a>const KRLDistanceHandle*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p82303471154"><a name="p82303471154"></a><a name="p82303471154"></a>KRLDistanceHandle指针。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p923018478155"><a name="p923018478155"></a><a name="p923018478155"></a>限制非空，需要使用krl_create_distance_handle初始化。</p>
</td>
</tr>
<tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p953215815518"><a name="p953215815518"></a><a name="p953215815518"></a>float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p23437551435"><a name="p23437551435"></a><a name="p23437551435"></a>存储计算所得的距离结果。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1334317552314"><a name="p1334317552314"></a><a name="p1334317552314"></a>限制长度为dis_size，其中<span class="parmname" id="parmname13438551312"><a name="parmname13438551312"></a><a name="parmname13438551312"></a>“dis_size”</span>为存储距离结果数组的长度。需要预先分配内存。</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p1089412431931"><a name="p1089412431931"></a><a name="p1089412431931"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p1389417431933"><a name="p1389417431933"></a><a name="p1389417431933"></a>const uint8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p28941943039"><a name="p28941943039"></a><a name="p28941943039"></a>参与距离计算的查询向量。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p389414311314"><a name="p389414311314"></a><a name="p389414311314"></a>限制长度为x_size，其中<span class="parmname" id="parmname58941043930"><a name="parmname58941043930"></a><a name="parmname58941043930"></a>“x_size”</span>为参与距离计算的查询向量数组的长度。</p>
</td>
</tr>
<tr id="row204111454114013"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p741115416407"><a name="p741115416407"></a><a name="p741115416407"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p11411185494014"><a name="p11411185494014"></a><a name="p11411185494014"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p54111354134020"><a name="p54111354134020"></a><a name="p54111354134020"></a>存储距离结果数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p64114540409"><a name="p64114540409"></a><a name="p64114540409"></a>num_base*codes_num，其中<span class="parmname" id="parmname1683723319432"><a name="parmname1683723319432"></a><a name="parmname1683723319432"></a>“num_base”</span>为单次处理的查询向量个数，<span class="parmname" id="parmname68371933174315"><a name="parmname68371933174315"></a><a name="parmname68371933174315"></a>“codes_num”</span>为每个查询向量计算的底库向量数量。</p>
</td>
</tr>
<tr id="row203061171413"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p63061672410"><a name="p63061672410"></a><a name="p63061672410"></a>x_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p1306147134110"><a name="p1306147134110"></a><a name="p1306147134110"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p330613718414"><a name="p330613718414"></a><a name="p330613718414"></a>参与距离计算的查询向量数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1730614764116"><a name="p1730614764116"></a><a name="p1730614764116"></a>d*num_base，其中<span class="parmname" id="parmname1753503824315"><a name="parmname1753503824315"></a><a name="parmname1753503824315"></a>“d”</span>为向量维度，<span class="parmname" id="parmname1353503811435"><a name="parmname1353503811435"></a><a name="parmname1353503811435"></a>“num_base”</span>为单次处理的查询向量个数。</p>
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
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a>正常运行时返回0，异常退出返回对应错误码。</p>
</td>
</tr>
</tbody>
</table>

**使用示例**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

int main() {
    // 参数配置
    size_t dim = 128;
    size_t num_base = 1;        // 单次处理的查询向量个数
    size_t codes_num = 1000;    // 每个查询向量计算的底库向量数量
    size_t accu_level = 3;      // fp32精度
    size_t blocksize = 32;
    int metric_type = 1;        // 欧氏距离

    // 准备底库向量
    size_t codes_size = num_base * codes_num * dim * sizeof(float);
    float* base_vectors = (float*)malloc(codes_size);
    for (size_t i = 0; i < num_base * codes_num * dim; i++) {
        base_vectors[i] = (float)(rand() % 1000) / 1000.0f;
    }

    // 创建Handle
    KRLDistanceHandle* kdh = NULL;
    int ret = krl_create_distance_handle(
        &kdh,
        accu_level,
        blocksize,
        codes_num,
        dim,
        num_base,
        metric_type,
        (const uint8_t*)base_vectors,
        codes_size
    );

    if (ret != 0) {
        printf("创建Handle失败: %d\n", ret);
        free(base_vectors);
        return -1;
    }

    // 准备查询向量
    size_t x_size = dim * num_base * sizeof(float);
    float* query_vec = (float*)malloc(x_size);
    for (size_t i = 0; i < dim * num_base; i++) {
        query_vec[i] = (float)(rand() % 1000) / 1000.0f;
    }

    // 分配结果数组
    size_t dis_size = num_base * codes_num;
    float* distances = (float*)malloc(dis_size * sizeof(float));

    // 使用Handle进行距离计算
    ret = krl_L2sqr_ny_with_handle(
        kdh,
        distances,
        query_vec,
        dis_size,
        x_size / sizeof(float)
    );

    if (ret != 0) {
        printf("距离计算失败: %d\n", ret);
        goto cleanup;
    }

    printf("使用Handle的一对多欧氏距离计算成功\n");
    printf("前5个距离结果:\n");
    for (size_t i = 0; i < 5 && i < dis_size; i++) {
        printf("  距离[%zu] = %f\n", i, distances[i]);
    }

cleanup:
    krl_clean_distance_handle(&kdh);
    free(base_vectors);
    free(query_vec);
    free(distances);

    return ret;
}
```

### krl\_inner\_product\_ny

**接口定义<a name="section172317194488"></a>**

int krl\_inner\_product\_ny\(float\* dis, const float\* x, const float\* y, size\_t ny, size\_t d, size\_t dis\_size\);

**接口用途<a name="section1153124784912"></a>**

进行数据类型为float的一对多内积距离计算。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515553%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.601460146014603%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="34.043404340434044%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="35.80358035803581%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row92301478154"><td class="cellrowborder" valign="top" width="15.551555155515553%" headers="mcps1.1.5.1.1 "><p id="p223015479158"><a name="p223015479158"></a><a name="p223015479158"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014603%" headers="mcps1.1.5.1.2 "><p id="p11230154710156"><a name="p11230154710156"></a><a name="p11230154710156"></a>float*</p>
</td>
<td class="cellrowborder" valign="top" width="34.043404340434044%" headers="mcps1.1.5.1.3 "><p id="p82303471154"><a name="p82303471154"></a><a name="p82303471154"></a>存储计算所得的距离结果。</p>
</td>
<td class="cellrowborder" valign="top" width="35.80358035803581%" headers="mcps1.1.5.1.4 "><p id="p923018478155"><a name="p923018478155"></a><a name="p923018478155"></a>限制长度为dis_size，其中<span class="parmname" id="parmname133743422533"><a name="parmname133743422533"></a><a name="parmname133743422533"></a>“dis_size”</span>为存储距离结果数组的长度。需要预先分配内存。</p>
</td>
</tr>
<tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515553%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014603%" headers="mcps1.1.5.1.2 "><p id="p953215815518"><a name="p953215815518"></a><a name="p953215815518"></a>const float*</p>
</td>
<td class="cellrowborder" valign="top" width="34.043404340434044%" headers="mcps1.1.5.1.3 "><p id="p18661136253"><a name="p18661136253"></a><a name="p18661136253"></a>参与距离计算的查询向量。</p>
</td>
<td class="cellrowborder" valign="top" width="35.80358035803581%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>限制长度为d，其中<span class="parmname" id="parmname76117481457"><a name="parmname76117481457"></a><a name="parmname76117481457"></a>“d”</span>为向量维度。</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515553%" headers="mcps1.1.5.1.1 "><p id="p4982142445414"><a name="p4982142445414"></a><a name="p4982142445414"></a>y</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014603%" headers="mcps1.1.5.1.2 "><p id="p7532158856"><a name="p7532158856"></a><a name="p7532158856"></a>const float*</p>
</td>
<td class="cellrowborder" valign="top" width="34.043404340434044%" headers="mcps1.1.5.1.3 "><p id="p36611261054"><a name="p36611261054"></a><a name="p36611261054"></a>参与距离计算的底库向量。</p>
</td>
<td class="cellrowborder" valign="top" width="35.80358035803581%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>限制长度为d*ny，其中<span class="parmname" id="parmname551215813519"><a name="parmname551215813519"></a><a name="parmname551215813519"></a>“d”</span>为向量维度，<span class="parmname" id="parmname8646142120239"><a name="parmname8646142120239"></a><a name="parmname8646142120239"></a>“ny”</span>为参与距离计算的底库向量个数。</p>
</td>
</tr>
<tr id="row103951453161513"><td class="cellrowborder" valign="top" width="15.551555155515553%" headers="mcps1.1.5.1.1 "><p id="p14723141215409"><a name="p14723141215409"></a><a name="p14723141215409"></a>ny</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014603%" headers="mcps1.1.5.1.2 "><p id="p4723181210404"><a name="p4723181210404"></a><a name="p4723181210404"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="34.043404340434044%" headers="mcps1.1.5.1.3 "><p id="p672341218403"><a name="p672341218403"></a><a name="p672341218403"></a>参与距离计算的底库向量个数。</p>
</td>
<td class="cellrowborder" valign="top" width="35.80358035803581%" headers="mcps1.1.5.1.4 "><p id="p6723181274010"><a name="p6723181274010"></a><a name="p6723181274010"></a>[1,2^30-1]</p>
</td>
</tr>
<tr id="row106882715416"><td class="cellrowborder" valign="top" width="15.551555155515553%" headers="mcps1.1.5.1.1 "><p id="p46812710547"><a name="p46812710547"></a><a name="p46812710547"></a>d</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014603%" headers="mcps1.1.5.1.2 "><p id="p45311183519"><a name="p45311183519"></a><a name="p45311183519"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="34.043404340434044%" headers="mcps1.1.5.1.3 "><p id="p17661261256"><a name="p17661261256"></a><a name="p17661261256"></a>向量维度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.80358035803581%" headers="mcps1.1.5.1.4 "><p id="p46952755416"><a name="p46952755416"></a><a name="p46952755416"></a>[1,65535]</p>
</td>
</tr>
<tr id="row1069011157013"><td class="cellrowborder" valign="top" width="15.551555155515553%" headers="mcps1.1.5.1.1 "><p id="p39628388417"><a name="p39628388417"></a><a name="p39628388417"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014603%" headers="mcps1.1.5.1.2 "><p id="p10722125214"><a name="p10722125214"></a><a name="p10722125214"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="34.043404340434044%" headers="mcps1.1.5.1.3 "><p id="p1762116529"><a name="p1762116529"></a><a name="p1762116529"></a>存储距离结果数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.80358035803581%" headers="mcps1.1.5.1.4 "><p id="p154517391451"><a name="p154517391451"></a><a name="p154517391451"></a>ny，其中<span class="parmname" id="parmname44553910519"><a name="parmname44553910519"></a><a name="parmname44553910519"></a>“ny”</span>为参与距离计算的底库向量个数。</p>
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
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a>正常运行时返回0，异常退出返回对应错误码。</p>
</td>
</tr>
</tbody>
</table>

**使用示例**

```c
#include <stdio.h>
#include <stdlib.h>
#include <math.h>
#include "krl.h"

int main() {
    size_t dim = 128;
    size_t ny = 1000;

    // 准备查询向量
    float* query_vec = (float*)malloc(dim * sizeof(float));
    for (size_t i = 0; i < dim; i++) {
        query_vec[i] = (float)(rand() % 100) / 100.0f;
    }

    // 准备底库向量
    float* base_vectors = (float*)malloc(ny * dim * sizeof(float));
    for (size_t i = 0; i < ny * dim; i++) {
        base_vectors[i] = (float)(rand() % 100) / 100.0f;
    }

    // 分配距离结果数组
    float* distances = (float*)malloc(ny * sizeof(float));

    // 执行一对多内积距离计算
    int ret = krl_inner_product_ny(
        distances,
        query_vec,
        base_vectors,
        ny,
        dim,
        ny
    );

    if (ret != 0) {
        printf("一对多内积距离计算失败，错误码: %d\n", ret);
        goto cleanup;
    }

    // 找出最大内积（最相似）
    float max_ip = distances[0];
    size_t max_idx = 0;
    for (size_t i = 1; i < ny; i++) {
        if (distances[i] > max_ip) {
            max_ip = distances[i];
            max_idx = i;
        }
    }

    printf("最相似向量: 索引=%zu, 内积=%f\n", max_idx, max_ip);

cleanup:
    free(query_vec);
    free(base_vectors);
    free(distances);

    return ret;
}
```

### krl\_inner\_product\_ny\_f16f32

**接口定义<a name="section172317194488"></a>**

int krl\_inner\_product\_ny\_f16f32\(float\* dis, const uint16\_t\* x, const uint16\_t\* y, size\_t ny, size\_t d, size\_t dis\_size\);

**接口用途<a name="section1153124784912"></a>**

进行数据类型为fp16的一对多内积距离计算。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.601460146014599%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.97339733973397%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="35.873587358735875%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row92301478154"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p223015479158"><a name="p223015479158"></a><a name="p223015479158"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p11230154710156"><a name="p11230154710156"></a><a name="p11230154710156"></a>float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.97339733973397%" headers="mcps1.1.5.1.3 "><p id="p82303471154"><a name="p82303471154"></a><a name="p82303471154"></a>存储计算所得的距离结果。</p>
</td>
<td class="cellrowborder" valign="top" width="35.873587358735875%" headers="mcps1.1.5.1.4 "><p id="p923018478155"><a name="p923018478155"></a><a name="p923018478155"></a>限制长度为dis_size，其中<span class="parmname" id="parmname133743422533"><a name="parmname133743422533"></a><a name="parmname133743422533"></a>“dis_size”</span>为存储距离结果数组的长度。需要预先分配内存。</p>
</td>
</tr>
<tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p953215815518"><a name="p953215815518"></a><a name="p953215815518"></a>const uint16_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.97339733973397%" headers="mcps1.1.5.1.3 "><p id="p18661136253"><a name="p18661136253"></a><a name="p18661136253"></a>参与距离计算的查询向量。</p>
</td>
<td class="cellrowborder" valign="top" width="35.873587358735875%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>限制长度为d，其中<span class="parmname" id="parmname76117481457"><a name="parmname76117481457"></a><a name="parmname76117481457"></a>“d”</span>为向量维度。</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4982142445414"><a name="p4982142445414"></a><a name="p4982142445414"></a>y</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7532158856"><a name="p7532158856"></a><a name="p7532158856"></a>const uint16_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.97339733973397%" headers="mcps1.1.5.1.3 "><p id="p36611261054"><a name="p36611261054"></a><a name="p36611261054"></a>参与距离计算的底库向量。</p>
</td>
<td class="cellrowborder" valign="top" width="35.873587358735875%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>限制长度为d*ny，其中<span class="parmname" id="parmname551215813519"><a name="parmname551215813519"></a><a name="parmname551215813519"></a>“d”</span>为向量维度，<span class="parmname" id="parmname8646142120239"><a name="parmname8646142120239"></a><a name="parmname8646142120239"></a>“ny”</span>为参与距离计算的底库向量个数。</p>
</td>
</tr>
<tr id="row103951453161513"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p14723141215409"><a name="p14723141215409"></a><a name="p14723141215409"></a>ny</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p4723181210404"><a name="p4723181210404"></a><a name="p4723181210404"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.97339733973397%" headers="mcps1.1.5.1.3 "><p id="p672341218403"><a name="p672341218403"></a><a name="p672341218403"></a>参与距离计算的底库向量个数。</p>
</td>
<td class="cellrowborder" valign="top" width="35.873587358735875%" headers="mcps1.1.5.1.4 "><p id="p6723181274010"><a name="p6723181274010"></a><a name="p6723181274010"></a>[1,2^30-1]</p>
</td>
</tr>
<tr id="row106882715416"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p46812710547"><a name="p46812710547"></a><a name="p46812710547"></a>d</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p45311183519"><a name="p45311183519"></a><a name="p45311183519"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.97339733973397%" headers="mcps1.1.5.1.3 "><p id="p17661261256"><a name="p17661261256"></a><a name="p17661261256"></a>向量维度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.873587358735875%" headers="mcps1.1.5.1.4 "><p id="p46952755416"><a name="p46952755416"></a><a name="p46952755416"></a>[1,65535]</p>
</td>
</tr>
<tr id="row536922710219"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p39628388417"><a name="p39628388417"></a><a name="p39628388417"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p10722125214"><a name="p10722125214"></a><a name="p10722125214"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.97339733973397%" headers="mcps1.1.5.1.3 "><p id="p1762116529"><a name="p1762116529"></a><a name="p1762116529"></a>存储距离结果数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.873587358735875%" headers="mcps1.1.5.1.4 "><p id="p154517391451"><a name="p154517391451"></a><a name="p154517391451"></a>ny，其中<span class="parmname" id="parmname44553910519"><a name="parmname44553910519"></a><a name="parmname44553910519"></a>“ny”</span>为参与距离计算的底库向量个数。</p>
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
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a>正常运行时返回0，异常退出返回对应错误码。</p>
</td>
</tr>
</tbody>
</table>

**使用示例**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

// 辅助函数：将float转换为fp16
uint16_t float_to_fp16(float value);

int main() {
    size_t dim = 256;
    size_t ny = 500;

    // 准备fp16格式的查询向量
    uint16_t* query_vec_fp16 = (uint16_t*)malloc(dim * sizeof(uint16_t));
    for (size_t i = 0; i < dim; i++) {
        query_vec_fp16[i] = float_to_fp16(0.5f);
    }

    // 准备fp16格式的底库向量
    uint16_t* base_vectors_fp16 = (uint16_t*)malloc(ny * dim * sizeof(uint16_t));
    for (size_t i = 0; i < ny * dim; i++) {
        base_vectors_fp16[i] = float_to_fp16((float)(rand() % 100) / 100.0f);
    }

    // 分配距离结果数组
    float* distances = (float*)malloc(ny * sizeof(float));

    // 执行fp16一对多内积距离计算
    int ret = krl_inner_product_ny_f16f32(
        distances,
        query_vec_fp16,
        base_vectors_fp16,
        ny,
        dim,
        ny
    );

    if (ret != 0) {
        printf("fp16一对多内积距离计算失败，错误码: %d\n", ret);
        goto cleanup;
    }

    printf("fp16一对多内积距离计算成功\n");

cleanup:
    free(query_vec_fp16);
    free(base_vectors_fp16);
    free(distances);

    return ret;
}
```

### krl\_inner\_product\_ny\_s8f32

**接口定义<a name="section172317194488"></a>**

int krl\_inner\_product\_ny\_s8f32\(float\* dis, const int8\_t\* x, const int8\_t\* y, size\_t ny, size\_t d, size\_t dis\_size\);

**接口用途<a name="section1153124784912"></a>**

进行数据类型为int8的一对多内积距离计算。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.601460146014599%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row92301478154"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p223015479158"><a name="p223015479158"></a><a name="p223015479158"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p11230154710156"><a name="p11230154710156"></a><a name="p11230154710156"></a>float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p82303471154"><a name="p82303471154"></a><a name="p82303471154"></a>存储计算所得的距离结果。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p923018478155"><a name="p923018478155"></a><a name="p923018478155"></a>限制长度为dis_size，其中<span class="parmname" id="parmname133743422533"><a name="parmname133743422533"></a><a name="parmname133743422533"></a>“dis_size”</span>为存储距离结果数组的长度。需要预先分配内存。</p>
</td>
</tr>
<tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p953215815518"><a name="p953215815518"></a><a name="p953215815518"></a>const int8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p18661136253"><a name="p18661136253"></a><a name="p18661136253"></a>参与距离计算的查询向量。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>限制长度为d，其中<span class="parmname" id="parmname76117481457"><a name="parmname76117481457"></a><a name="parmname76117481457"></a>“d”</span>为向量维度。</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4982142445414"><a name="p4982142445414"></a><a name="p4982142445414"></a>y</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7532158856"><a name="p7532158856"></a><a name="p7532158856"></a>const int8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p36611261054"><a name="p36611261054"></a><a name="p36611261054"></a>参与距离计算的底库向量。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>限制长度为d*ny，其中<span class="parmname" id="parmname551215813519"><a name="parmname551215813519"></a><a name="parmname551215813519"></a>“d”</span>为向量维度，<span class="parmname" id="parmname8646142120239"><a name="parmname8646142120239"></a><a name="parmname8646142120239"></a>“ny”</span>为参与距离计算的底库向量个数。</p>
</td>
</tr>
<tr id="row103951453161513"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p14723141215409"><a name="p14723141215409"></a><a name="p14723141215409"></a>ny</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p4723181210404"><a name="p4723181210404"></a><a name="p4723181210404"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p672341218403"><a name="p672341218403"></a><a name="p672341218403"></a>参与距离计算的底库向量个数。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p6723181274010"><a name="p6723181274010"></a><a name="p6723181274010"></a>[1,2^30-1]</p>
</td>
</tr>
<tr id="row106882715416"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p46812710547"><a name="p46812710547"></a><a name="p46812710547"></a>d</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p45311183519"><a name="p45311183519"></a><a name="p45311183519"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p17661261256"><a name="p17661261256"></a><a name="p17661261256"></a>向量维度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p46952755416"><a name="p46952755416"></a><a name="p46952755416"></a>[1,65535]</p>
</td>
</tr>
<tr id="row1491157243"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p39628388417"><a name="p39628388417"></a><a name="p39628388417"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p10722125214"><a name="p10722125214"></a><a name="p10722125214"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p1762116529"><a name="p1762116529"></a><a name="p1762116529"></a>存储距离结果数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p154517391451"><a name="p154517391451"></a><a name="p154517391451"></a>ny，其中<span class="parmname" id="parmname44553910519"><a name="parmname44553910519"></a><a name="parmname44553910519"></a>“ny”</span>为参与距离计算的底库向量个数。</p>
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
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a>正常运行时返回0，异常退出返回对应错误码。</p>
</td>
</tr>
</tbody>
</table>

**使用示例**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

int main() {
    size_t dim = 128;
    size_t ny = 1000;

    // 准备int8类型的查询向量
    int8_t* query_vec = (int8_t*)malloc(dim * sizeof(int8_t));
    for (size_t i = 0; i < dim; i++) {
        query_vec[i] = (int8_t)(rand() % 256 - 128);
    }

    // 准备int8类型的底库向量
    int8_t* base_vectors = (int8_t*)malloc(ny * dim * sizeof(int8_t));
    for (size_t i = 0; i < ny * dim; i++) {
        base_vectors[i] = (int8_t)(rand() % 256 - 128);
    }

    // 分配距离结果数组
    float* distances = (float*)malloc(ny * sizeof(float));

    // 执行int8一对多内积距离计算
    int ret = krl_inner_product_ny_s8f32(
        distances,
        query_vec,
        base_vectors,
        ny,
        dim,
        ny
    );

    if (ret != 0) {
        printf("int8一对多内积距离计算失败，错误码: %d\n", ret);
        goto cleanup;
    }

    printf("int8一对多内积距离计算成功\n");

    // 找出Top-3
    printf("Top-3 最大内积:\n");
    for (int k = 0; k < 3; k++) {
        float max_val = -1e30f;
        size_t max_idx = 0;
        for (size_t i = 0; i < ny; i++) {
            if (distances[i] > max_val) {
                max_val = distances[i];
                max_idx = i;
            }
        }
        printf("  第%d名: 索引=%zu, 内积=%f\n", k + 1, max_idx, max_val);
        distances[max_idx] = -1e30f;  // 标记已选
    }

cleanup:
    free(query_vec);
    free(base_vectors);
    free(distances);

    return ret;
}
```

### krl\_inner\_product\_ny\_with\_handle

**接口定义<a name="section172317194488"></a>**

int krl\_inner\_product\_ny\_with\_handle\(const KRLDistanceHandle\* krl\_distance\_handle, float\* dis, const float\* x, size\_t dis\_size, size\_t x\_size\);

**接口用途<a name="section1153124784912"></a>**

进行数据类型为float的一对多内积距离计算，底库向量与维度存储于Handle中。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.601460146014599%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row92301478154"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p223015479158"><a name="p223015479158"></a><a name="p223015479158"></a>kdh</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p11230154710156"><a name="p11230154710156"></a><a name="p11230154710156"></a>const KRLDistanceHandle*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p82303471154"><a name="p82303471154"></a><a name="p82303471154"></a>KRLDistanceHandle指针。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p923018478155"><a name="p923018478155"></a><a name="p923018478155"></a>限制非空，需要使用krl_create_distance_handle初始化。</p>
</td>
</tr>
<tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p953215815518"><a name="p953215815518"></a><a name="p953215815518"></a>float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p23437551435"><a name="p23437551435"></a><a name="p23437551435"></a>存储计算所得的距离结果。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1334317552314"><a name="p1334317552314"></a><a name="p1334317552314"></a>限制长度为dis_size，其中<span class="parmname" id="parmname13438551312"><a name="parmname13438551312"></a><a name="parmname13438551312"></a>“dis_size”</span>为存储距离结果数组的长度。需要预先分配内存。</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p1089412431931"><a name="p1089412431931"></a><a name="p1089412431931"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p1389417431933"><a name="p1389417431933"></a><a name="p1389417431933"></a>const uint8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p28941943039"><a name="p28941943039"></a><a name="p28941943039"></a>参与距离计算的查询向量。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p389414311314"><a name="p389414311314"></a><a name="p389414311314"></a>限制长度为x_size，其中<span class="parmname" id="parmname58941043930"><a name="parmname58941043930"></a><a name="parmname58941043930"></a>“x_size”</span>为参与距离计算的查询向量数组的长度。</p>
</td>
</tr>
<tr id="row416975034615"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p741115416407"><a name="p741115416407"></a><a name="p741115416407"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p11411185494014"><a name="p11411185494014"></a><a name="p11411185494014"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p54111354134020"><a name="p54111354134020"></a><a name="p54111354134020"></a>存储距离结果数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p116975012466"><a name="p116975012466"></a><a name="p116975012466"></a>num_base*codes_num，其中<span class="parmname" id="parmname206011465474"><a name="parmname206011465474"></a><a name="parmname206011465474"></a>“num_base”</span>为单次处理的查询向量个数，<span class="parmname" id="parmname1660186134712"><a name="parmname1660186134712"></a><a name="parmname1660186134712"></a>“codes_num”</span>为每个查询向量计算的底库向量数量。</p>
</td>
</tr>
<tr id="row17378115284614"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p63061672410"><a name="p63061672410"></a><a name="p63061672410"></a>x_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p1306147134110"><a name="p1306147134110"></a><a name="p1306147134110"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p330613718414"><a name="p330613718414"></a><a name="p330613718414"></a>参与距离计算的查询向量数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p10378252194615"><a name="p10378252194615"></a><a name="p10378252194615"></a>d*num_base，其中<span class="parmname" id="parmname5313131244714"><a name="parmname5313131244714"></a><a name="parmname5313131244714"></a>“d”</span>为向量维度，<span class="parmname" id="parmname231381224715"><a name="parmname231381224715"></a><a name="parmname231381224715"></a>“num_base”</span>为单次处理的查询向量个数。</p>
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
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a>正常运行时返回0，异常退出返回对应错误码。</p>
</td>
</tr>
</tbody>
</table>

**使用示例**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

int main() {
    // 参数配置
    size_t dim = 128;
    size_t num_base = 1;
    size_t codes_num = 1000;
    size_t accu_level = 3;
    size_t blocksize = 32;
    int metric_type = 0;  // 内积距离

    // 准备底库向量
    size_t codes_size = num_base * codes_num * dim * sizeof(float);
    float* base_vectors = (float*)malloc(codes_size);
    for (size_t i = 0; i < num_base * codes_num * dim; i++) {
        base_vectors[i] = (float)(rand() % 100) / 100.0f;
    }

    // 创建Handle（使用内积距离度量）
    KRLDistanceHandle* kdh = NULL;
    int ret = krl_create_distance_handle(
        &kdh,
        accu_level,
        blocksize,
        codes_num,
        dim,
        num_base,
        metric_type,  // 0表示内积距离
        (const uint8_t*)base_vectors,
        codes_size
    );

    if (ret != 0) {
        printf("创建Handle失败: %d\n", ret);
        free(base_vectors);
        return -1;
    }

    // 准备查询向量
    size_t x_size = dim * num_base;
    float* query_vec = (float*)malloc(x_size * sizeof(float));
    for (size_t i = 0; i < x_size; i++) {
        query_vec[i] = (float)(rand() % 100) / 100.0f;
    }

    // 分配结果数组
    size_t dis_size = num_base * codes_num;
    float* distances = (float*)malloc(dis_size * sizeof(float));

    // 使用Handle进行内积距离计算
    ret = krl_inner_product_ny_with_handle(
        kdh,
        distances,
        query_vec,
        dis_size,
        x_size
    );

    if (ret != 0) {
        printf("内积距离计算失败: %d\n", ret);
        goto cleanup;
    }

    printf("使用Handle的一对多内积距离计算成功\n");

    // 找出最大内积
    float max_ip = distances[0];
    size_t max_idx = 0;
    for (size_t i = 1; i < dis_size; i++) {
        if (distances[i] > max_ip) {
            max_ip = distances[i];
            max_idx = i;
        }
    }
    printf("最相似向量: 索引=%zu, 内积=%f\n", max_idx, max_ip);

cleanup:
    krl_clean_distance_handle(&kdh);
    free(base_vectors);
    free(query_vec);
    free(distances);

    return ret;
}
```

## 8bit查表累和接口

### krl\_table\_lookup\_8b\_f32

**接口定义<a name="section172317194488"></a>**

int krl\_table\_lookup\_8b\_f32\(size\_t nsq, size\_t ncode, const uint8\_t\* codes, const float\* sim\_table, float\* distance, float dis0, size\_t codes\_size, size\_t sim\_table\_size, size\_t dis\_size\);

**接口用途<a name="section1153124784912"></a>**

使用8bit索引在float类型表项中查询距离并累和，将累和结果加上dis0后存入distance。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.601460146014599%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row92301478154"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p223015479158"><a name="p223015479158"></a><a name="p223015479158"></a>nsq</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p11230154710156"><a name="p11230154710156"></a><a name="p11230154710156"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p82303471154"><a name="p82303471154"></a><a name="p82303471154"></a>子空间数量。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p923018478155"><a name="p923018478155"></a><a name="p923018478155"></a>[1,65535]</p>
</td>
</tr>
<tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>ncode</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p953215815518"><a name="p953215815518"></a><a name="p953215815518"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p18661136253"><a name="p18661136253"></a><a name="p18661136253"></a>底库向量总数。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>[1,2^30-1]</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4982142445414"><a name="p4982142445414"></a><a name="p4982142445414"></a>codes</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7532158856"><a name="p7532158856"></a><a name="p7532158856"></a>const uint8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p36611261054"><a name="p36611261054"></a><a name="p36611261054"></a>码本，底库向量对应的索引。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>限制长度为codes_size，其中<span class="parmname" id="parmname551215813519"><a name="parmname551215813519"></a><a name="parmname551215813519"></a>“codes_size”</span>为码本数组的长度。</p>
</td>
</tr>
<tr id="row103951453161513"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p14723141215409"><a name="p14723141215409"></a><a name="p14723141215409"></a>sim_table</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p4723181210404"><a name="p4723181210404"></a><a name="p4723181210404"></a>const float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p718413012396"><a name="p718413012396"></a><a name="p718413012396"></a>码表，存储每维度查询向量与所有质心的距离。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p6723181274010"><a name="p6723181274010"></a><a name="p6723181274010"></a>限制长度为sim_table_size，其中<span class="parmname" id="parmname23951728194513"><a name="parmname23951728194513"></a><a name="parmname23951728194513"></a>“sim_table_size”</span>为码表数组的长度。</p>
</td>
</tr>
<tr id="row106882715416"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p46812710547"><a name="p46812710547"></a><a name="p46812710547"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p45311183519"><a name="p45311183519"></a><a name="p45311183519"></a>float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p17661261256"><a name="p17661261256"></a><a name="p17661261256"></a>存储计算所得的距离结果。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p57801052141013"><a name="p57801052141013"></a><a name="p57801052141013"></a>限制长度为dis_size，其中<span class="parmname" id="parmname1048505120457"><a name="parmname1048505120457"></a><a name="parmname1048505120457"></a>“dis_size”</span>为存储距离结果数组的长度。需预先分配内存。</p>
</td>
</tr>
<tr id="row1875218456372"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p275311453374"><a name="p275311453374"></a><a name="p275311453374"></a>dis0</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7753045173714"><a name="p7753045173714"></a><a name="p7753045173714"></a>float</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p17531445103716"><a name="p17531445103716"></a><a name="p17531445103716"></a>初始距离。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p69179904614"><a name="p69179904614"></a><a name="p69179904614"></a>浮点数。</p>
</td>
</tr>
<tr id="row9742043764"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p137414311617"><a name="p137414311617"></a><a name="p137414311617"></a>codes_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p06662231878"><a name="p06662231878"></a><a name="p06662231878"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p16744431269"><a name="p16744431269"></a><a name="p16744431269"></a>码本数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p127494317611"><a name="p127494317611"></a><a name="p127494317611"></a>nsq*ncode，其中<span class="parmname" id="parmname137711421694"><a name="parmname137711421694"></a><a name="parmname137711421694"></a>“nsq”</span>为子空间数量，<span class="parmname" id="parmname83779421995"><a name="parmname83779421995"></a><a name="parmname83779421995"></a>“ncode”</span>为底库向量总数。</p>
</td>
</tr>
<tr id="row411920559612"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p7119655861"><a name="p7119655861"></a><a name="p7119655861"></a>sim_table_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p6403112617719"><a name="p6403112617719"></a><a name="p6403112617719"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p311925516613"><a name="p311925516613"></a><a name="p311925516613"></a>码表数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p81191255064"><a name="p81191255064"></a><a name="p81191255064"></a>nsq*256，其中<span class="parmname" id="parmname6479105617916"><a name="parmname6479105617916"></a><a name="parmname6479105617916"></a>“nsq”</span>为子空间数量。</p>
</td>
</tr>
<tr id="row2533196472"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p1753316619720"><a name="p1753316619720"></a><a name="p1753316619720"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p64039264714"><a name="p64039264714"></a><a name="p64039264714"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p54111354134020"><a name="p54111354134020"></a><a name="p54111354134020"></a>存储距离结果数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p175331661478"><a name="p175331661478"></a><a name="p175331661478"></a>ncode，其中<span class="parmname" id="parmname89954141011"><a name="parmname89954141011"></a><a name="parmname89954141011"></a>“ncode”</span>为底库向量总数。</p>
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
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a>正常运行时返回0，异常退出返回对应错误码。</p>
</td>
</tr>
</tbody>
</table>

**使用示例**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

int main() {
    // PQ参数配置
    size_t nsq = 32;        // 子空间数量（向量被分成32个子空间）
    size_t ncode = 10000;   // 底库向量总数
    size_t ksub = 256;      // 每个子空间的质心数量（8bit索引，最多256个）

    // 准备码本（codes）
    // 每个底库向量有nsq个索引，每个索引指向对应子空间的质心
    size_t codes_size = nsq * ncode;
    uint8_t* codes = (uint8_t*)malloc(codes_size * sizeof(uint8_t));
    
    // 模拟码本数据（实际使用中由PQ训练得到）
    for (size_t i = 0; i < codes_size; i++) {
        codes[i] = (uint8_t)(rand() % ksub);
    }

    // 准备码表（sim_table）
    // 存储查询向量与每个子空间所有质心的距离
    // 维度：nsq * ksub
    size_t sim_table_size = nsq * ksub;
    float* sim_table = (float*)malloc(sim_table_size * sizeof(float));
    
    // 模拟码表数据（实际使用中需要计算查询向量与质心的距离）
    for (size_t i = 0; i < sim_table_size; i++) {
        sim_table[i] = (float)(rand() % 1000) / 100.0f;
    }

    // 分配距离结果数组
    float* distances = (float*)malloc(ncode * sizeof(float));

    // 执行8bit查表累和
    float dis0 = 0.0f;  // 初始距离
    int ret = krl_table_lookup_8b_f32(
        nsq,
        ncode,
        codes,
        sim_table,
        distances,
        dis0,
        codes_size,
        sim_table_size,
        ncode
    );

    if (ret != 0) {
        printf("8bit查表累和失败，错误码: %d\n", ret);
        goto cleanup;
    }

    printf("8bit查表累和计算成功\n");

    // 找出最近邻
    float min_dist = distances[0];
    size_t min_idx = 0;
    for (size_t i = 1; i < ncode; i++) {
        if (distances[i] < min_dist) {
            min_dist = distances[i];
            min_idx = i;
        }
    }
    printf("最近邻: 索引=%zu, PQ距离=%f\n", min_idx, min_dist);

cleanup:
    free(codes);
    free(sim_table);
    free(distances);

    return ret;
}
```

### krl\_table\_lookup\_8b\_f32\_by\_idx

**接口定义<a name="section172317194488"></a>**

int krl\_table\_lookup\_8b\_f32\_by\_idx\(size\_t nsq, size\_t ncode, const uint8\_t\* codes, const float\* sim\_table, float\* dis, float dis0, const size\_t\* idx, size\_t codes\_size, size\_t sim\_table\_size, size\_t dis\_size\);

**接口用途<a name="section1153124784912"></a>**

使用8bit索引在float类型表项中查询距离并累和，将累和结果加上dis0后存入distance。ID在idx数组中出现的底库向量结果才会参与计算。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.601460146014599%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row92301478154"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p223015479158"><a name="p223015479158"></a><a name="p223015479158"></a>nsq</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p11230154710156"><a name="p11230154710156"></a><a name="p11230154710156"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p82303471154"><a name="p82303471154"></a><a name="p82303471154"></a>子空间数量。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p923018478155"><a name="p923018478155"></a><a name="p923018478155"></a>[1,65535]</p>
</td>
</tr>
<tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>ncode</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p953215815518"><a name="p953215815518"></a><a name="p953215815518"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p18661136253"><a name="p18661136253"></a><a name="p18661136253"></a>底库向量总数。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>[1,2^30-1]</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4982142445414"><a name="p4982142445414"></a><a name="p4982142445414"></a>codes</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7532158856"><a name="p7532158856"></a><a name="p7532158856"></a>const uint8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p992551816390"><a name="p992551816390"></a><a name="p992551816390"></a>码本，底库向量对应的索引。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>限制长度为codes_size，其中<span class="parmname" id="parmname551215813519"><a name="parmname551215813519"></a><a name="parmname551215813519"></a>“codes_size”</span>为码本数组的长度。</p>
</td>
</tr>
<tr id="row103951453161513"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p14723141215409"><a name="p14723141215409"></a><a name="p14723141215409"></a>sim_table</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p4723181210404"><a name="p4723181210404"></a><a name="p4723181210404"></a>const float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p710155233915"><a name="p710155233915"></a><a name="p710155233915"></a>码表，存储每维度查询向量与所有质心的距离。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p6723181274010"><a name="p6723181274010"></a><a name="p6723181274010"></a>限制长度为sim_table_size，其中<span class="parmname" id="parmname23951728194513"><a name="parmname23951728194513"></a><a name="parmname23951728194513"></a>“sim_table_size”</span>为码表数组的长度。</p>
</td>
</tr>
<tr id="row106882715416"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p46812710547"><a name="p46812710547"></a><a name="p46812710547"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p45311183519"><a name="p45311183519"></a><a name="p45311183519"></a>float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p17661261256"><a name="p17661261256"></a><a name="p17661261256"></a>存储计算所得的距离结果。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p57801052141013"><a name="p57801052141013"></a><a name="p57801052141013"></a>限制长度为dis_size，其中<span class="parmname" id="parmname1048505120457"><a name="parmname1048505120457"></a><a name="parmname1048505120457"></a>“dis_size”</span>为存储距离结果数组的长度。需预先分配内存。</p>
</td>
</tr>
<tr id="row1875218456372"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p275311453374"><a name="p275311453374"></a><a name="p275311453374"></a>dis0</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7753045173714"><a name="p7753045173714"></a><a name="p7753045173714"></a>float</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p17531445103716"><a name="p17531445103716"></a><a name="p17531445103716"></a>初始距离。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p69179904614"><a name="p69179904614"></a><a name="p69179904614"></a>浮点数。</p>
</td>
</tr>
<tr id="row575095414710"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p075085444712"><a name="p075085444712"></a><a name="p075085444712"></a>idx</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p19750155420479"><a name="p19750155420479"></a><a name="p19750155420479"></a>const size_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p875015418477"><a name="p875015418477"></a><a name="p875015418477"></a>参与计算的底库向量ID数组。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p375065415472"><a name="p375065415472"></a><a name="p375065415472"></a>限制长度为ncode，其中<span class="parmname" id="parmname3464124964815"><a name="parmname3464124964815"></a><a name="parmname3464124964815"></a>“ncode”</span>为底库向量总数。ID需要递增。</p>
</td>
</tr>
<tr id="row14701171851717"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p137414311617"><a name="p137414311617"></a><a name="p137414311617"></a>codes_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p06662231878"><a name="p06662231878"></a><a name="p06662231878"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p16744431269"><a name="p16744431269"></a><a name="p16744431269"></a>码本数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p127494317611"><a name="p127494317611"></a><a name="p127494317611"></a>nsq*ncode，其中<span class="parmname" id="parmname137711421694"><a name="parmname137711421694"></a><a name="parmname137711421694"></a>“nsq”</span>为子空间数量，<span class="parmname" id="parmname83779421995"><a name="parmname83779421995"></a><a name="parmname83779421995"></a>“ncode”</span>为底库向量总数。</p>
</td>
</tr>
<tr id="row37001918161712"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p7119655861"><a name="p7119655861"></a><a name="p7119655861"></a>sim_table_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p6403112617719"><a name="p6403112617719"></a><a name="p6403112617719"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p311925516613"><a name="p311925516613"></a><a name="p311925516613"></a>码表数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p81191255064"><a name="p81191255064"></a><a name="p81191255064"></a>nsq*256，其中<span class="parmname" id="parmname6479105617916"><a name="parmname6479105617916"></a><a name="parmname6479105617916"></a>“nsq”</span>为子空间数量。</p>
</td>
</tr>
<tr id="row370081812173"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p1753316619720"><a name="p1753316619720"></a><a name="p1753316619720"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p64039264714"><a name="p64039264714"></a><a name="p64039264714"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p54111354134020"><a name="p54111354134020"></a><a name="p54111354134020"></a>存储距离结果数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p175331661478"><a name="p175331661478"></a><a name="p175331661478"></a>ncode，其中<span class="parmname" id="parmname89954141011"><a name="parmname89954141011"></a><a name="parmname89954141011"></a>“ncode”</span>为底库向量总数。</p>
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
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a>正常运行时返回0，异常退出返回对应错误码。</p>
</td>
</tr>
</tbody>
</table>

**使用示例**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

int main() {
    // PQ参数配置
    size_t nsq = 32;
    size_t total_vectors = 100000;  // 底库总向量数
    size_t ncode = 1000;            // 需要计算的向量数（筛选后）
    size_t ksub = 256;

    // 准备码本
    size_t full_codes_size = nsq * total_vectors;
    uint8_t* codes = (uint8_t*)malloc(full_codes_size * sizeof(uint8_t));
    for (size_t i = 0; i < full_codes_size; i++) {
        codes[i] = (uint8_t)(rand() % ksub);
    }

    // 准备码表
    size_t sim_table_size = nsq * ksub;
    float* sim_table = (float*)malloc(sim_table_size * sizeof(float));
    for (size_t i = 0; i < sim_table_size; i++) {
        sim_table[i] = (float)(rand() % 1000) / 100.0f;
    }

    // 准备筛选后的ID数组（必须递增）
    size_t* idx = (size_t*)malloc(ncode * sizeof(size_t));
    for (size_t i = 0; i < ncode; i++) {
        idx[i] = i * 100;  // 选择ID: 0, 100, 200, ...（递增）
    }

    // 分配距离结果数组
    float* distances = (float*)malloc(ncode * sizeof(float));

    // 执行带索引的8bit查表累和
    float dis0 = 0.0f;
    int ret = krl_table_lookup_8b_f32_by_idx(
        nsq,
        ncode,
        codes,
        sim_table,
        distances,
        dis0,
        idx,
        nsq * ncode,  // 只计算选中的向量
        sim_table_size,
        ncode
    );

    if (ret != 0) {
        printf("带索引的8bit查表累和失败，错误码: %d\n", ret);
        goto cleanup;
    }

    printf("带索引的8bit查表累和计算成功\n");
    printf("计算了%zu个向量的PQ距离\n", ncode);

    // 输出前5个结果
    printf("前5个结果:\n");
    for (size_t i = 0; i < 5 && i < ncode; i++) {
        printf("  向量ID[%zu]: PQ距离 = %f\n", idx[i], distances[i]);
    }

cleanup:
    free(codes);
    free(sim_table);
    free(idx);
    free(distances);

    return ret;
}
```

### krl\_table\_lookup\_8b\_f32\_with\_handle

**接口定义<a name="section172317194488"></a>**

int krl\_table\_lookup\_8b\_f32\_with\_handle\(KRLLUT8bHandle\* klh, size\_t dim, size\_t ncode, const uint8\_t\* codes, const float\* sim\_table, float dis0, size\_t codes\_size, size\_t sim\_table\_size\);

**接口用途<a name="section1153124784912"></a>**

使用8bit索引在float类型表项中查询距离并累和，将累和结果加上dis0后存入distance。idx数组与distance数组被包含在KRLLUT8bHandle实例中，ID在idx数组中出现的底库向量结果才会参与计算。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.601460146014599%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.953395339533955%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="35.8935893589359%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row92301478154"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p223015479158"><a name="p223015479158"></a><a name="p223015479158"></a>klh</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p11230154710156"><a name="p11230154710156"></a><a name="p11230154710156"></a>KRLLUT8bHandle*</p>
</td>
<td class="cellrowborder" valign="top" width="33.953395339533955%" headers="mcps1.1.5.1.3 "><p id="p82303471154"><a name="p82303471154"></a><a name="p82303471154"></a>KRLLUT8bHandle指针。</p>
</td>
<td class="cellrowborder" valign="top" width="35.8935893589359%" headers="mcps1.1.5.1.4 "><p id="p923018478155"><a name="p923018478155"></a><a name="p923018478155"></a>限制非空，需要使用krl_create_LUT8b_handle初始化。</p>
</td>
</tr>
<tr id="row166241441532"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p262494414531"><a name="p262494414531"></a><a name="p262494414531"></a>dim</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p126241544125310"><a name="p126241544125310"></a><a name="p126241544125310"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.953395339533955%" headers="mcps1.1.5.1.3 "><p id="p1562414447536"><a name="p1562414447536"></a><a name="p1562414447536"></a>向量维度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.8935893589359%" headers="mcps1.1.5.1.4 "><p id="p19624744195313"><a name="p19624744195313"></a><a name="p19624744195313"></a>[1,65535]</p>
</td>
</tr>
<tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>ncode</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p953215815518"><a name="p953215815518"></a><a name="p953215815518"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.953395339533955%" headers="mcps1.1.5.1.3 "><p id="p18661136253"><a name="p18661136253"></a><a name="p18661136253"></a>底库向量总数。</p>
</td>
<td class="cellrowborder" valign="top" width="35.8935893589359%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>[1,2^30-1]</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4982142445414"><a name="p4982142445414"></a><a name="p4982142445414"></a>codes</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7532158856"><a name="p7532158856"></a><a name="p7532158856"></a>const uint8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.953395339533955%" headers="mcps1.1.5.1.3 "><p id="p992551816390"><a name="p992551816390"></a><a name="p992551816390"></a>码本，底库向量对应的索引。</p>
</td>
<td class="cellrowborder" valign="top" width="35.8935893589359%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>限制长度为codes_size，其中<span class="parmname" id="parmname551215813519"><a name="parmname551215813519"></a><a name="parmname551215813519"></a>“codes_size”</span>为码本数组的长度。</p>
</td>
</tr>
<tr id="row103951453161513"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p14723141215409"><a name="p14723141215409"></a><a name="p14723141215409"></a>sim_table</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p4723181210404"><a name="p4723181210404"></a><a name="p4723181210404"></a>const float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.953395339533955%" headers="mcps1.1.5.1.3 "><p id="p710155233915"><a name="p710155233915"></a><a name="p710155233915"></a>码表，存储每维度查询向量与所有质心的距离。</p>
</td>
<td class="cellrowborder" valign="top" width="35.8935893589359%" headers="mcps1.1.5.1.4 "><p id="p6723181274010"><a name="p6723181274010"></a><a name="p6723181274010"></a>限制长度为sim_table_size，其中<span class="parmname" id="parmname23951728194513"><a name="parmname23951728194513"></a><a name="parmname23951728194513"></a>“sim_table_size”</span>为码表数组的长度。</p>
</td>
</tr>
<tr id="row1875218456372"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p275311453374"><a name="p275311453374"></a><a name="p275311453374"></a>dis0</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7753045173714"><a name="p7753045173714"></a><a name="p7753045173714"></a>float</p>
</td>
<td class="cellrowborder" valign="top" width="33.953395339533955%" headers="mcps1.1.5.1.3 "><p id="p17531445103716"><a name="p17531445103716"></a><a name="p17531445103716"></a>初始距离。</p>
</td>
<td class="cellrowborder" valign="top" width="35.8935893589359%" headers="mcps1.1.5.1.4 "><p id="p69179904614"><a name="p69179904614"></a><a name="p69179904614"></a>浮点数。</p>
</td>
</tr>
<tr id="row10770205351915"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p137414311617"><a name="p137414311617"></a><a name="p137414311617"></a>codes_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p06662231878"><a name="p06662231878"></a><a name="p06662231878"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.953395339533955%" headers="mcps1.1.5.1.3 "><p id="p16744431269"><a name="p16744431269"></a><a name="p16744431269"></a>码本数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.8935893589359%" headers="mcps1.1.5.1.4 "><p id="p127494317611"><a name="p127494317611"></a><a name="p127494317611"></a>dim*ncode，其中<span class="parmname" id="parmname1015643162220"><a name="parmname1015643162220"></a><a name="parmname1015643162220"></a>“dim”</span>为向量维度，<span class="parmname" id="parmname19156153115224"><a name="parmname19156153115224"></a><a name="parmname19156153115224"></a>“ncode”</span>为底库向量总数。</p>
</td>
</tr>
<tr id="row15300105641919"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p7119655861"><a name="p7119655861"></a><a name="p7119655861"></a>sim_table_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p6403112617719"><a name="p6403112617719"></a><a name="p6403112617719"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.953395339533955%" headers="mcps1.1.5.1.3 "><p id="p311925516613"><a name="p311925516613"></a><a name="p311925516613"></a>码表数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.8935893589359%" headers="mcps1.1.5.1.4 "><p id="p1350143882216"><a name="p1350143882216"></a><a name="p1350143882216"></a>dim*256，其中<span class="parmname" id="parmname450118384223"><a name="parmname450118384223"></a><a name="parmname450118384223"></a>“dim”</span>为向量维度。</p>
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
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a>正常运行时返回0，异常退出返回对应错误码。</p>
</td>
</tr>
</tbody>
</table>

**使用示例**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

int main() {
    // 参数配置
    size_t dim = 128;       // 向量维度（也是子空间数量）
    size_t ncode = 10000;   // 底库向量总数
    size_t ksub = 256;
    int use_idx = 1;        // 启用索引筛选
    size_t capacity = ncode;

    // 创建LUT8b Handle
    KRLLUT8bHandle* klh = NULL;
    int ret = krl_create_LUT8b_handle(&klh, use_idx, capacity);
    if (ret != 0) {
        printf("创建LUT8b Handle失败: %d\n", ret);
        return -1;
    }

    // 设置需要计算的向量ID
    size_t* idx_ptr = krl_get_idx_pointer(klh);
    size_t selected_count = 500;  // 只计算500个向量
    for (size_t i = 0; i < selected_count; i++) {
        idx_ptr[i] = i * 20;  // 选择ID: 0, 20, 40, ...
    }

    // 准备码本
    size_t codes_size = dim * ncode;
    uint8_t* codes = (uint8_t*)malloc(codes_size * sizeof(uint8_t));
    for (size_t i = 0; i < codes_size; i++) {
        codes[i] = (uint8_t)(rand() % ksub);
    }

    // 准备码表
    size_t sim_table_size = dim * ksub;
    float* sim_table = (float*)malloc(sim_table_size * sizeof(float));
    for (size_t i = 0; i < sim_table_size; i++) {
        sim_table[i] = (float)(rand() % 1000) / 100.0f;
    }

    // 执行使用Handle的8bit查表累和
    float dis0 = 0.0f;
    ret = krl_table_lookup_8b_f32_with_handle(
        klh,
        dim,
        selected_count,  // 实际计算的向量数
        codes,
        sim_table,
        dis0,
        codes_size,
        sim_table_size
    );

    if (ret != 0) {
        printf("使用Handle的8bit查表累和失败: %d\n", ret);
        goto cleanup;
    }

    // 获取距离结果
    float* dist_ptr = krl_get_dist_pointer(klh);

    printf("使用Handle的8bit查表累和计算成功\n");
    printf("前5个结果:\n");
    for (size_t i = 0; i < 5 && i < selected_count; i++) {
        printf("  向量ID[%zu]: PQ距离 = %f\n", idx_ptr[i], dist_ptr[i]);
    }

cleanup:
    krl_clean_LUT8b_handle(&klh);
    free(codes);
    free(sim_table);

    return ret;
}
```

## 4bit查表累和接口

### krl\_fast\_table\_lookup\_step

**接口定义<a name="section172317194488"></a>**

int krl\_fast\_table\_lookup\_step\(int nq, int nsq, const uint8\_t\* codes, const uint8\_t\* LUT, uint16\_t\* dis, const uint16\_t\* threshold, uint32\_t\* lt\_mask, int keep\_min, size\_t codes\_size, size\_t LUT\_size, size\_t dis\_size, size\_t threshold\_size, size\_t lt\_mask\_size\);

**接口用途<a name="section1153124784912"></a>**

批量处理数据类型为float的查询向量的4bit查表累和过滤压缩算子。算子支持计算至多16个查询向量与32个底库向量间的距离。在距离计算完成后，将其与阈值进行比较，满足比较条件的底库向量的lt\_mask对应位置将会设置为1，反之为0。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.601460146014599%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row92301478154"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p223015479158"><a name="p223015479158"></a><a name="p223015479158"></a>nq</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p11230154710156"><a name="p11230154710156"></a><a name="p11230154710156"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p82303471154"><a name="p82303471154"></a><a name="p82303471154"></a>查询向量总数。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p923018478155"><a name="p923018478155"></a><a name="p923018478155"></a>[1,16]</p>
</td>
</tr>
<tr id="row166241441532"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p262494414531"><a name="p262494414531"></a><a name="p262494414531"></a>nsq</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p126241544125310"><a name="p126241544125310"></a><a name="p126241544125310"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p1562414447536"><a name="p1562414447536"></a><a name="p1562414447536"></a>子空间数量。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p19624744195313"><a name="p19624744195313"></a><a name="p19624744195313"></a>[1,256]且为偶数。</p>
</td>
</tr>
<tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p14381721205612"><a name="p14381721205612"></a><a name="p14381721205612"></a>codes</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7438122115569"><a name="p7438122115569"></a><a name="p7438122115569"></a>const uint8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p570319812427"><a name="p570319812427"></a><a name="p570319812427"></a>码本，使用krl_pack_codes_4b（blocksize=32）处理后底库向量对应的索引。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p51251625162911"><a name="p51251625162911"></a><a name="p51251625162911"></a>限制长度为codes_size，其中<span class="parmname" id="parmname18125825132915"><a name="parmname18125825132915"></a><a name="parmname18125825132915"></a>“codes_size”</span>为码本数组的长度。</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4982142445414"><a name="p4982142445414"></a><a name="p4982142445414"></a>LUT</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7532158856"><a name="p7532158856"></a><a name="p7532158856"></a>const uint8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p36611261054"><a name="p36611261054"></a><a name="p36611261054"></a>各子空间中PQ质心与查询向量的uint8距离表。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>限制长度为LUT_size，其中<span class="parmname" id="parmname551215813519"><a name="parmname551215813519"></a><a name="parmname551215813519"></a>“LUT_size”</span>为距离表数组的长度。</p>
</td>
</tr>
<tr id="row103951453161513"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p14723141215409"><a name="p14723141215409"></a><a name="p14723141215409"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p4723181210404"><a name="p4723181210404"></a><a name="p4723181210404"></a>uint16_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p672341218403"><a name="p672341218403"></a><a name="p672341218403"></a>存储计算所得的距离结果。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p57801052141013"><a name="p57801052141013"></a><a name="p57801052141013"></a>限制长度为dis_size，其中<span class="parmname" id="parmname1048505120457"><a name="parmname1048505120457"></a><a name="parmname1048505120457"></a>“dis_size”</span>为存储距离结果数组的长度。需预先分配内存。</p>
</td>
</tr>
<tr id="row1875218456372"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p275311453374"><a name="p275311453374"></a><a name="p275311453374"></a>threshold</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7753045173714"><a name="p7753045173714"></a><a name="p7753045173714"></a>const uint16_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p17531445103716"><a name="p17531445103716"></a><a name="p17531445103716"></a>距离阈值。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p748810273302"><a name="p748810273302"></a><a name="p748810273302"></a>限制长度为threshold_size，其中<span class="parmname" id="parmname18488627123013"><a name="parmname18488627123013"></a><a name="parmname18488627123013"></a>“threshold_size”</span>为距离阈值数组的长度。阈值限制为65535。</p>
</td>
</tr>
<tr id="row143744955610"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p34370492563"><a name="p34370492563"></a><a name="p34370492563"></a>lt_mask</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p3437549145616"><a name="p3437549145616"></a><a name="p3437549145616"></a>uint32_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p143715495569"><a name="p143715495569"></a><a name="p143715495569"></a>过滤压缩结果。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p77615321231"><a name="p77615321231"></a><a name="p77615321231"></a>限制长度为lt_mask_size，其中<span class="parmname" id="parmname10988163762914"><a name="parmname10988163762914"></a><a name="parmname10988163762914"></a>“lt_mask_size”</span>为过滤压缩结果数组的长度。需预先分配内存。</p>
</td>
</tr>
<tr id="row12299105712"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p22931165713"><a name="p22931165713"></a><a name="p22931165713"></a>keep_min</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p192916117571"><a name="p192916117571"></a><a name="p192916117571"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p8731759124214"><a name="p8731759124214"></a><a name="p8731759124214"></a>是否保留小于阈值的距离结果。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p329412578"><a name="p329412578"></a><a name="p329412578"></a>[0,1]，取值表示是否保留小于阈值的距离结果：</p>
<a name="ul164886121012"></a><a name="ul164886121012"></a><ul id="ul164886121012"><li>0：保留大于阈值的距离结果。</li><li>1：保留小于阈值的距离结果。</li></ul>
</td>
</tr>
<tr id="row1167140172619"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p11681640172619"><a name="p11681640172619"></a><a name="p11681640172619"></a>codes_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p06662231878"><a name="p06662231878"></a><a name="p06662231878"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p16681940142616"><a name="p16681940142616"></a><a name="p16681940142616"></a>码本数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p568184012612"><a name="p568184012612"></a><a name="p568184012612"></a>nsq/2*32，其中<span class="parmname" id="parmname1170114418287"><a name="parmname1170114418287"></a><a name="parmname1170114418287"></a>“nsq”</span>为子空间数量。</p>
</td>
</tr>
<tr id="row1758312172712"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p1258316232715"><a name="p1258316232715"></a><a name="p1258316232715"></a>LUT_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p6403112617719"><a name="p6403112617719"></a><a name="p6403112617719"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p1258316212714"><a name="p1258316212714"></a><a name="p1258316212714"></a>距离表数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1658311212279"><a name="p1658311212279"></a><a name="p1658311212279"></a>nq*nsq*16，其中<span class="parmname" id="parmname299054918285"><a name="parmname299054918285"></a><a name="parmname299054918285"></a>“nq”</span>为查询向量总数，<span class="parmname" id="parmname9990249152811"><a name="parmname9990249152811"></a><a name="parmname9990249152811"></a>“nsq”</span>为子空间数量。</p>
</td>
</tr>
<tr id="row613215113273"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p1613312110277"><a name="p1613312110277"></a><a name="p1613312110277"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p1699263912712"><a name="p1699263912712"></a><a name="p1699263912712"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p21335117279"><a name="p21335117279"></a><a name="p21335117279"></a>存储距离结果数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p41335118277"><a name="p41335118277"></a><a name="p41335118277"></a>nq*32，其中<span class="parmname" id="parmname2640145611280"><a name="parmname2640145611280"></a><a name="parmname2640145611280"></a>“nq”</span>为查询向量总数。</p>
</td>
</tr>
<tr id="row9243174820292"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4243154811296"><a name="p4243154811296"></a><a name="p4243154811296"></a>threshold_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p1524318483294"><a name="p1524318483294"></a><a name="p1524318483294"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p8243184812293"><a name="p8243184812293"></a><a name="p8243184812293"></a>距离阈值数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1824374814291"><a name="p1824374814291"></a><a name="p1824374814291"></a>nq，其中<span class="parmname" id="parmname1180318211305"><a name="parmname1180318211305"></a><a name="parmname1180318211305"></a>“nq”</span>为查询向量总数。</p>
</td>
</tr>
<tr id="row721827152717"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p172182719273"><a name="p172182719273"></a><a name="p172182719273"></a>lt_mask_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p119923399274"><a name="p119923399274"></a><a name="p119923399274"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p92127202712"><a name="p92127202712"></a><a name="p92127202712"></a>过滤压缩结果数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1421327132714"><a name="p1421327132714"></a><a name="p1421327132714"></a>nq/32，其中<span class="parmname" id="parmname5124423292"><a name="parmname5124423292"></a><a name="parmname5124423292"></a>“nq”</span>为查询向量总数。</p>
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
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a>正常运行时返回0，异常退出返回对应错误码。</p>
</td>
</tr>
</tbody>
</table>

**使用示例**

```c
#include <stdio.h>
#include <stdlib.h>
#include <string.h>
#include "krl.h"

int main() {
    // 4bit PQ参数配置
    int nq = 8;             // 查询向量数量（最多16个）
    int nsq = 64;           // 子空间数量（必须为偶数）
    int ncode = 32;         // 底库向量数量（固定为32）
    int ksub = 16;          // 4bit索引，每个子空间16个质心

    // 准备码本（4bit打包后）
    // 4bit打包：每2个4bit索引合并为1个uint8
    size_t codes_size = (nsq / 2) * ncode;
    uint8_t* codes = (uint8_t*)malloc(codes_size * sizeof(uint8_t));
    
    // 模拟4bit打包的码本数据
    for (size_t i = 0; i < codes_size; i++) {
        uint8_t low = rand() % ksub;   // 低4位
        uint8_t high = rand() % ksub;  // 高4位
        codes[i] = (high << 4) | low;
    }

    // 准备距离表（LUT）
    // 维度：nq * nsq * ksub
    size_t LUT_size = nq * nsq * ksub;
    uint8_t* LUT = (uint8_t*)malloc(LUT_size * sizeof(uint8_t));
    for (size_t i = 0; i < LUT_size; i++) {
        LUT[i] = (uint8_t)(rand() % 256);
    }

    // 准备距离结果数组
    size_t dis_size = nq * ncode;
    uint16_t* distances = (uint16_t*)malloc(dis_size * sizeof(uint16_t));

    // 准备阈值数组（每个查询向量一个阈值）
    uint16_t* threshold = (uint16_t*)malloc(nq * sizeof(uint16_t));
    for (int i = 0; i < nq; i++) {
        threshold[i] = 5000;  // 设置距离阈值
    }

    // 准备过滤掩码数组
    size_t lt_mask_size = (nq + 31) / 32;  // 向上取整
    uint32_t* lt_mask = (uint32_t*)malloc(lt_mask_size * sizeof(uint32_t));
    memset(lt_mask, 0, lt_mask_size * sizeof(uint32_t));

    // 执行4bit查表累和过滤
    int keep_min = 1;  // 保留小于阈值的结果
    int ret = krl_fast_table_lookup_step(
        nq,
        nsq,
        codes,
        LUT,
        distances,
        threshold,
        lt_mask,
        keep_min,
        codes_size,
        LUT_size,
        dis_size,
        nq,
        lt_mask_size
    );

    if (ret != 0) {
        printf("4bit查表累和过滤失败，错误码: %d\n", ret);
        goto cleanup;
    }

    printf("4bit查表累和过滤计算成功\n");

    // 统计满足条件的向量数量
    int passed_count = 0;
    for (size_t i = 0; i < lt_mask_size; i++) {
        for (int bit = 0; bit < 32; bit++) {
            if (lt_mask[i] & (1u << bit)) {
                passed_count++;
            }
        }
    }
    printf("满足阈值条件的向量数量: %d\n", passed_count);

cleanup:
    free(codes);
    free(LUT);
    free(distances);
    free(threshold);
    free(lt_mask);

    return ret;
}
```

### krl\_L2\_table\_lookup\_fast\_scan\_bs64

**接口定义<a name="section172317194488"></a>**

int krl\_L2\_table\_lookup\_fast\_scan\_bs64\(int nsq, const uint8\_t\* codes, const uint8\_t\* LUT, uint16\_t\* dis, uint16\_t threshold, uint32\_t\* lt\_mask, size\_t codes\_size, size\_t LUT\_size, size\_t dis\_size, size\_t lt\_mask\_size\);

**接口用途<a name="section1153124784912"></a>**

单独处理数据类型为float的查询向量的4比特查表累和过滤压缩算子。计算1个查询向量与64个底库向量间的欧氏距离。根据距离类型决定比较规则，将距离值满足比较规则的底库向量的lt\_mask设置为1，反之为0。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.601460146014599%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.97339733973397%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="35.873587358735875%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row166241441532"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p262494414531"><a name="p262494414531"></a><a name="p262494414531"></a>nsq</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p126241544125310"><a name="p126241544125310"></a><a name="p126241544125310"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="33.97339733973397%" headers="mcps1.1.5.1.3 "><p id="p1562414447536"><a name="p1562414447536"></a><a name="p1562414447536"></a>子空间数量。</p>
</td>
<td class="cellrowborder" valign="top" width="35.873587358735875%" headers="mcps1.1.5.1.4 "><p id="p19624744195313"><a name="p19624744195313"></a><a name="p19624744195313"></a>[1,256]且为偶数。</p>
</td>
</tr>
<tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p14381721205612"><a name="p14381721205612"></a><a name="p14381721205612"></a>codes</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7438122115569"><a name="p7438122115569"></a><a name="p7438122115569"></a>const uint8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.97339733973397%" headers="mcps1.1.5.1.3 "><p id="p18618921124518"><a name="p18618921124518"></a><a name="p18618921124518"></a>码本，使用krl_pack_codes_4b（blocksize=64）处理后底库向量对应的索引。</p>
</td>
<td class="cellrowborder" valign="top" width="35.873587358735875%" headers="mcps1.1.5.1.4 "><p id="p51251625162911"><a name="p51251625162911"></a><a name="p51251625162911"></a>限制长度为codes_size，其中<span class="parmname" id="parmname18125825132915"><a name="parmname18125825132915"></a><a name="parmname18125825132915"></a>“codes_size”</span>为码本数组的长度。</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4982142445414"><a name="p4982142445414"></a><a name="p4982142445414"></a>LUT</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7532158856"><a name="p7532158856"></a><a name="p7532158856"></a>const uint8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.97339733973397%" headers="mcps1.1.5.1.3 "><p id="p36611261054"><a name="p36611261054"></a><a name="p36611261054"></a>各子空间中PQ质心与查询向量的uint8距离表。</p>
</td>
<td class="cellrowborder" valign="top" width="35.873587358735875%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>限制长度为LUT_size，其中<span class="parmname" id="parmname551215813519"><a name="parmname551215813519"></a><a name="parmname551215813519"></a>“LUT_size”</span>为距离表数组的长度。</p>
</td>
</tr>
<tr id="row103951453161513"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p14723141215409"><a name="p14723141215409"></a><a name="p14723141215409"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p4723181210404"><a name="p4723181210404"></a><a name="p4723181210404"></a>uint16_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.97339733973397%" headers="mcps1.1.5.1.3 "><p id="p672341218403"><a name="p672341218403"></a><a name="p672341218403"></a>存储计算所得的距离结果。</p>
</td>
<td class="cellrowborder" valign="top" width="35.873587358735875%" headers="mcps1.1.5.1.4 "><p id="p57801052141013"><a name="p57801052141013"></a><a name="p57801052141013"></a>限制长度为dis_size，其中<span class="parmname" id="parmname1048505120457"><a name="parmname1048505120457"></a><a name="parmname1048505120457"></a>“dis_size”</span>为存储距离结果数组的长度。需预先分配内存。</p>
</td>
</tr>
<tr id="row1875218456372"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p275311453374"><a name="p275311453374"></a><a name="p275311453374"></a>threshold</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7753045173714"><a name="p7753045173714"></a><a name="p7753045173714"></a>const uint16_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.97339733973397%" headers="mcps1.1.5.1.3 "><p id="p17531445103716"><a name="p17531445103716"></a><a name="p17531445103716"></a>距离阈值。</p>
</td>
<td class="cellrowborder" valign="top" width="35.873587358735875%" headers="mcps1.1.5.1.4 "><p id="p748810273302"><a name="p748810273302"></a><a name="p748810273302"></a>限制为65535。</p>
</td>
</tr>
<tr id="row143744955610"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p34370492563"><a name="p34370492563"></a><a name="p34370492563"></a>lt_mask</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p3437549145616"><a name="p3437549145616"></a><a name="p3437549145616"></a>uint32_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.97339733973397%" headers="mcps1.1.5.1.3 "><p id="p143715495569"><a name="p143715495569"></a><a name="p143715495569"></a>过滤压缩结果。</p>
</td>
<td class="cellrowborder" valign="top" width="35.873587358735875%" headers="mcps1.1.5.1.4 "><p id="p77615321231"><a name="p77615321231"></a><a name="p77615321231"></a>限制长度为lt_mask_size，其中<span class="parmname" id="parmname10988163762914"><a name="parmname10988163762914"></a><a name="parmname10988163762914"></a>“lt_mask_size”</span>为过滤压缩结果数组的长度。需预先分配内存。</p>
</td>
</tr>
<tr id="row1695419558379"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p11681640172619"><a name="p11681640172619"></a><a name="p11681640172619"></a>codes_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p06662231878"><a name="p06662231878"></a><a name="p06662231878"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.97339733973397%" headers="mcps1.1.5.1.3 "><p id="p16681940142616"><a name="p16681940142616"></a><a name="p16681940142616"></a>码本数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.873587358735875%" headers="mcps1.1.5.1.4 "><p id="p568184012612"><a name="p568184012612"></a><a name="p568184012612"></a>nsq/2*64，其中<span class="parmname" id="parmname1170114418287"><a name="parmname1170114418287"></a><a name="parmname1170114418287"></a>“nsq”</span>为子空间数量。</p>
</td>
</tr>
<tr id="row15954175511376"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p1258316232715"><a name="p1258316232715"></a><a name="p1258316232715"></a>LUT_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p6403112617719"><a name="p6403112617719"></a><a name="p6403112617719"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.97339733973397%" headers="mcps1.1.5.1.3 "><p id="p1258316212714"><a name="p1258316212714"></a><a name="p1258316212714"></a>距离表数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.873587358735875%" headers="mcps1.1.5.1.4 "><p id="p1658311212279"><a name="p1658311212279"></a><a name="p1658311212279"></a>nsq*16，其中<span class="parmname" id="parmname584361843817"><a name="parmname584361843817"></a><a name="parmname584361843817"></a>“nsq”</span>为子空间数量。</p>
</td>
</tr>
<tr id="row109541655133713"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p1613312110277"><a name="p1613312110277"></a><a name="p1613312110277"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p1699263912712"><a name="p1699263912712"></a><a name="p1699263912712"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.97339733973397%" headers="mcps1.1.5.1.3 "><p id="p21335117279"><a name="p21335117279"></a><a name="p21335117279"></a>存储距离结果数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.873587358735875%" headers="mcps1.1.5.1.4 "><p id="p41335118277"><a name="p41335118277"></a><a name="p41335118277"></a>限制为64。</p>
</td>
</tr>
<tr id="row4954455153717"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p172182719273"><a name="p172182719273"></a><a name="p172182719273"></a>lt_mask_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p119923399274"><a name="p119923399274"></a><a name="p119923399274"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.97339733973397%" headers="mcps1.1.5.1.3 "><p id="p92127202712"><a name="p92127202712"></a><a name="p92127202712"></a>过滤压缩结果数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.873587358735875%" headers="mcps1.1.5.1.4 "><p id="p1421327132714"><a name="p1421327132714"></a><a name="p1421327132714"></a>限制为2。</p>
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
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a>正常运行时返回0，异常退出返回对应错误码。</p>
</td>
</tr>
</tbody>
</table>

**使用示例**

```c
#include <stdio.h>
#include <stdlib.h>
#include <string.h>
#include "krl.h"

int main() {
    // 4bit PQ参数配置（blocksize=64）
    int nsq = 64;           // 子空间数量（必须为偶数）
    int ncode = 64;         // 底库向量数量（固定为64）
    int ksub = 16;          // 4bit索引

    // 准备码本（4bit打包，blocksize=64）
    size_t codes_size = (nsq / 2) * ncode;
    uint8_t* codes = (uint8_t*)malloc(codes_size * sizeof(uint8_t));
    
    for (size_t i = 0; i < codes_size; i++) {
        uint8_t low = rand() % ksub;
        uint8_t high = rand() % ksub;
        codes[i] = (high << 4) | low;
    }

    // 准备距离表（LUT）
    size_t LUT_size = nsq * ksub;
    uint8_t* LUT = (uint8_t*)malloc(LUT_size * sizeof(uint8_t));
    for (size_t i = 0; i < LUT_size; i++) {
        LUT[i] = (uint8_t)(rand() % 256);
    }

    // 准备距离结果数组
    uint16_t* distances = (uint16_t*)malloc(ncode * sizeof(uint16_t));

    // 准备过滤掩码数组
    size_t lt_mask_size = 2;  // 64个向量需要2个uint32
    uint32_t* lt_mask = (uint32_t*)malloc(lt_mask_size * sizeof(uint32_t));
    memset(lt_mask, 0, lt_mask_size * sizeof(uint32_t));

    // 执行L2距离的4bit查表累和过滤（blocksize=64）
    uint16_t threshold = 8000;  // 距离阈值
    int ret = krl_L2_table_lookup_fast_scan_bs64(
        nsq,
        codes,
        LUT,
        distances,
        threshold,
        lt_mask,
        codes_size,
        LUT_size,
        ncode,       // dis_size固定为64
        lt_mask_size
    );

    if (ret != 0) {
        printf("L2 4bit查表累和过滤失败，错误码: %d\n", ret);
        goto cleanup;
    }

    printf("L2 4bit查表累和过滤（bs64）计算成功\n");

    // 统计满足条件的向量
    printf("满足条件的向量（距离 < %u）:\n", threshold);
    int count = 0;
    for (int i = 0; i < ncode; i++) {
        int mask_idx = i / 32;
        int bit_idx = i % 32;
        if (lt_mask[mask_idx] & (1u << bit_idx)) {
            if (count < 10) {  // 只显示前10个
                printf("  向量[%d]: 距离 = %u\n", i, distances[i]);
            }
            count++;
        }
    }
    printf("共%d个向量满足条件\n", count);

cleanup:
    free(codes);
    free(LUT);
    free(distances);
    free(lt_mask);

    return ret;
}
```

### krl\_IP\_table\_lookup\_fast\_scan\_bs64

**接口定义<a name="section172317194488"></a>**

int krl\_IP\_table\_lookup\_fast\_scan\_bs64\(int nsq, const uint8\_t\* codes, const uint8\_t\* LUT, uint16\_t\* dis, uint16\_t threshold, uint32\_t\* lt\_mask, size\_t codes\_size, size\_t LUT\_size, size\_t dis\_size, size\_t lt\_mask\_size\);

**接口用途<a name="section1153124784912"></a>**

单独处理数据类型为float的查询向量的4比特查表累和过滤压缩算子。计算1个查询向量与64个底库向量间的内积距离。根据距离类型决定比较规则，将距离值满足比较规则的底库向量的lt\_mask设置为1，反之为0。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.601460146014599%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row166241441532"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p262494414531"><a name="p262494414531"></a><a name="p262494414531"></a>nsq</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p126241544125310"><a name="p126241544125310"></a><a name="p126241544125310"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p1562414447536"><a name="p1562414447536"></a><a name="p1562414447536"></a>子空间数量。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p19624744195313"><a name="p19624744195313"></a><a name="p19624744195313"></a>[1,256]且为偶数。</p>
</td>
</tr>
<tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p14381721205612"><a name="p14381721205612"></a><a name="p14381721205612"></a>codes</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7438122115569"><a name="p7438122115569"></a><a name="p7438122115569"></a>const uint8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p18618921124518"><a name="p18618921124518"></a><a name="p18618921124518"></a>码本，使用krl_pack_codes_4b（blocksize=64）处理后底库向量对应的索引。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p51251625162911"><a name="p51251625162911"></a><a name="p51251625162911"></a>限制长度为codes_size，其中<span class="parmname" id="parmname18125825132915"><a name="parmname18125825132915"></a><a name="parmname18125825132915"></a>“codes_size”</span>为码本数组的长度。</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4982142445414"><a name="p4982142445414"></a><a name="p4982142445414"></a>LUT</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7532158856"><a name="p7532158856"></a><a name="p7532158856"></a>const uint8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p36611261054"><a name="p36611261054"></a><a name="p36611261054"></a>各子空间中PQ质心与查询向量的uint8距离表。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>限制长度为LUT_size，其中<span class="parmname" id="parmname551215813519"><a name="parmname551215813519"></a><a name="parmname551215813519"></a>“LUT_size”</span>为距离表数组的长度。</p>
</td>
</tr>
<tr id="row103951453161513"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p14723141215409"><a name="p14723141215409"></a><a name="p14723141215409"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p4723181210404"><a name="p4723181210404"></a><a name="p4723181210404"></a>uint16_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p672341218403"><a name="p672341218403"></a><a name="p672341218403"></a>存储计算所得的距离结果。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p57801052141013"><a name="p57801052141013"></a><a name="p57801052141013"></a>限制长度为dis_size，其中<span class="parmname" id="parmname1048505120457"><a name="parmname1048505120457"></a><a name="parmname1048505120457"></a>“dis_size”</span>为存储距离结果数组的长度。需预先分配内存。</p>
</td>
</tr>
<tr id="row1875218456372"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p275311453374"><a name="p275311453374"></a><a name="p275311453374"></a>threshold</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7753045173714"><a name="p7753045173714"></a><a name="p7753045173714"></a>const uint16_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p17531445103716"><a name="p17531445103716"></a><a name="p17531445103716"></a>距离阈值。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p748810273302"><a name="p748810273302"></a><a name="p748810273302"></a>限制为65535。</p>
</td>
</tr>
<tr id="row143744955610"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p34370492563"><a name="p34370492563"></a><a name="p34370492563"></a>lt_mask</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p3437549145616"><a name="p3437549145616"></a><a name="p3437549145616"></a>uint32_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p143715495569"><a name="p143715495569"></a><a name="p143715495569"></a>过滤压缩结果。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p77615321231"><a name="p77615321231"></a><a name="p77615321231"></a>限制长度为lt_mask_size，其中<span class="parmname" id="parmname10988163762914"><a name="parmname10988163762914"></a><a name="parmname10988163762914"></a>“lt_mask_size”</span>为过滤压缩结果数组的长度。需预先分配内存。</p>
</td>
</tr>
<tr id="row177615011429"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p11681640172619"><a name="p11681640172619"></a><a name="p11681640172619"></a>codes_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p06662231878"><a name="p06662231878"></a><a name="p06662231878"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p16681940142616"><a name="p16681940142616"></a><a name="p16681940142616"></a>码本数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p568184012612"><a name="p568184012612"></a><a name="p568184012612"></a>nsq/2*64，其中<span class="parmname" id="parmname1170114418287"><a name="parmname1170114418287"></a><a name="parmname1170114418287"></a>“nsq”</span>为子空间数量。</p>
</td>
</tr>
<tr id="row9760006427"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p1258316232715"><a name="p1258316232715"></a><a name="p1258316232715"></a>LUT_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p6403112617719"><a name="p6403112617719"></a><a name="p6403112617719"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p1258316212714"><a name="p1258316212714"></a><a name="p1258316212714"></a>距离表数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1658311212279"><a name="p1658311212279"></a><a name="p1658311212279"></a>nsq*16，其中<span class="parmname" id="parmname584361843817"><a name="parmname584361843817"></a><a name="parmname584361843817"></a>“nsq”</span>为子空间数量。</p>
</td>
</tr>
<tr id="row1276017012420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p1613312110277"><a name="p1613312110277"></a><a name="p1613312110277"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p1699263912712"><a name="p1699263912712"></a><a name="p1699263912712"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p21335117279"><a name="p21335117279"></a><a name="p21335117279"></a>存储距离结果数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p41335118277"><a name="p41335118277"></a><a name="p41335118277"></a>限制为64。</p>
</td>
</tr>
<tr id="row157604034212"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p172182719273"><a name="p172182719273"></a><a name="p172182719273"></a>lt_mask_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p119923399274"><a name="p119923399274"></a><a name="p119923399274"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p92127202712"><a name="p92127202712"></a><a name="p92127202712"></a>过滤压缩结果数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1421327132714"><a name="p1421327132714"></a><a name="p1421327132714"></a>限制为2。</p>
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
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a>正常运行时返回0，异常退出返回对应错误码。</p>
</td>
</tr>
</tbody>
</table>

**使用示例**

```c
#include <stdio.h>
#include <stdlib.h>
#include <string.h>
#include "krl.h"

int main() {
    // 4bit PQ参数配置（内积距离，blocksize=64）
    int nsq = 64;           // 子空间数量（必须为偶数）
    int ncode = 64;         // 底库向量数量（固定为64）
    int ksub = 16;          // 4bit索引，每个子空间16个质心

    // 准备码本（4bit打包，blocksize=64）
    size_t codes_size = (nsq / 2) * ncode;
    uint8_t* codes = (uint8_t*)malloc(codes_size * sizeof(uint8_t));
    
    for (size_t i = 0; i < codes_size; i++) {
        uint8_t low = rand() % ksub;
        uint8_t high = rand() % ksub;
        codes[i] = (high << 4) | low;
    }

    // 准备内积距离表（LUT）
    // 注意：内积距离通常需要取反或特殊处理以便于比较
    size_t LUT_size = nsq * ksub;
    uint8_t* LUT = (uint8_t*)malloc(LUT_size * sizeof(uint8_t));
    for (size_t i = 0; i < LUT_size; i++) {
        LUT[i] = (uint8_t)(rand() % 256);
    }

    // 准备距离结果数组
    uint16_t* distances = (uint16_t*)malloc(ncode * sizeof(uint16_t));

    // 准备过滤掩码数组
    size_t lt_mask_size = 2;  // 64个向量需要2个uint32
    uint32_t* lt_mask = (uint32_t*)malloc(lt_mask_size * sizeof(uint32_t));
    memset(lt_mask, 0, lt_mask_size * sizeof(uint32_t));

    // 执行内积距离的4bit查表累和过滤
    // 注意：对于内积距离，阈值比较规则与L2距离不同
    // 内积越大越相似，因此通常保留大于阈值的结果
    uint16_t threshold = 3000;
    int ret = krl_IP_table_lookup_fast_scan_bs64(
        nsq,
        codes,
        LUT,
        distances,
        threshold,
        lt_mask,
        codes_size,
        LUT_size,
        ncode,
        lt_mask_size
    );

    if (ret != 0) {
        printf("IP 4bit查表累和过滤失败，错误码: %d\n", ret);
        goto cleanup;
    }

    printf("IP 4bit查表累和过滤（bs64）计算成功\n");

    // 统计满足条件的向量（内积 > 阈值）
    int count = 0;
    printf("满足条件的向量（内积 > %u）:\n", threshold);
    for (int i = 0; i < ncode; i++) {
        int mask_idx = i / 32;
        int bit_idx = i % 32;
        if (lt_mask[mask_idx] & (1u << bit_idx)) {
            if (count < 5) {
                printf("  向量[%d]: 内积 = %u\n", i, distances[i]);
            }
            count++;
        }
    }
    printf("共%d个向量满足条件\n", count);

cleanup:
    free(codes);
    free(LUT);
    free(distances);
    free(lt_mask);

    return ret;
}
```

### krl\_L2\_table\_lookup\_fast\_scan\_bs96

**接口定义<a name="section172317194488"></a>**

int krl\_L2\_table\_lookup\_fast\_scan\_bs96\(int nsq, const uint8\_t\* codes, const uint8\_t\* LUT, uint16\_t\* dis, uint16\_t threshold, uint32\_t\* lt\_mask, size\_t codes\_size, size\_t LUT\_size, size\_t dis\_size, size\_t lt\_mask\_size\);

**接口用途<a name="section1153124784912"></a>**

单独处理数据类型为float的查询向量的4比特查表累和过滤压缩算子。计算1个查询向量与96个底库向量间的欧氏距离。根据距离类型决定比较规则，将距离值满足比较规则的底库向量的lt\_mask设置为1，反之为0。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.601460146014599%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row166241441532"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p262494414531"><a name="p262494414531"></a><a name="p262494414531"></a>nsq</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p126241544125310"><a name="p126241544125310"></a><a name="p126241544125310"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p1562414447536"><a name="p1562414447536"></a><a name="p1562414447536"></a>子空间数量。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p19624744195313"><a name="p19624744195313"></a><a name="p19624744195313"></a>[1,256]且为偶数。</p>
</td>
</tr>
<tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p14381721205612"><a name="p14381721205612"></a><a name="p14381721205612"></a>codes</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7438122115569"><a name="p7438122115569"></a><a name="p7438122115569"></a>const uint8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p18438121155616"><a name="p18438121155616"></a><a name="p18438121155616"></a>码本，使用krl_pack_codes_4b（blocksize=96）处理后底库向量对应的索引。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p51251625162911"><a name="p51251625162911"></a><a name="p51251625162911"></a>限制长度为codes_size，其中<span class="parmname" id="parmname18125825132915"><a name="parmname18125825132915"></a><a name="parmname18125825132915"></a>“codes_size”</span>为码本数组的长度。</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4982142445414"><a name="p4982142445414"></a><a name="p4982142445414"></a>LUT</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7532158856"><a name="p7532158856"></a><a name="p7532158856"></a>const uint8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p36611261054"><a name="p36611261054"></a><a name="p36611261054"></a>各子空间中PQ质心与查询向量的uint8距离表。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>限制长度为LUT_size，其中<span class="parmname" id="parmname551215813519"><a name="parmname551215813519"></a><a name="parmname551215813519"></a>“LUT_size”</span>为距离表数组的长度。</p>
</td>
</tr>
<tr id="row103951453161513"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p14723141215409"><a name="p14723141215409"></a><a name="p14723141215409"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p4723181210404"><a name="p4723181210404"></a><a name="p4723181210404"></a>uint16_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p672341218403"><a name="p672341218403"></a><a name="p672341218403"></a>存储计算所得的距离结果。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p57801052141013"><a name="p57801052141013"></a><a name="p57801052141013"></a>限制长度为dis_size，其中<span class="parmname" id="parmname1048505120457"><a name="parmname1048505120457"></a><a name="parmname1048505120457"></a>“dis_size”</span>为存储距离结果数组的长度。需预先分配内存。</p>
</td>
</tr>
<tr id="row1875218456372"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p275311453374"><a name="p275311453374"></a><a name="p275311453374"></a>threshold</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7753045173714"><a name="p7753045173714"></a><a name="p7753045173714"></a>const uint16_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p17531445103716"><a name="p17531445103716"></a><a name="p17531445103716"></a>距离阈值。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p748810273302"><a name="p748810273302"></a><a name="p748810273302"></a>限制为65535。</p>
</td>
</tr>
<tr id="row143744955610"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p34370492563"><a name="p34370492563"></a><a name="p34370492563"></a>lt_mask</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p3437549145616"><a name="p3437549145616"></a><a name="p3437549145616"></a>uint32_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p143715495569"><a name="p143715495569"></a><a name="p143715495569"></a>过滤压缩结果。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p77615321231"><a name="p77615321231"></a><a name="p77615321231"></a>限制长度为lt_mask_size，其中<span class="parmname" id="parmname10988163762914"><a name="parmname10988163762914"></a><a name="parmname10988163762914"></a>“lt_mask_size”</span>为过滤压缩结果数组的长度。需预先分配内存。</p>
</td>
</tr>
<tr id="row02162634718"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p11681640172619"><a name="p11681640172619"></a><a name="p11681640172619"></a>codes_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p06662231878"><a name="p06662231878"></a><a name="p06662231878"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p16681940142616"><a name="p16681940142616"></a><a name="p16681940142616"></a>码本数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p568184012612"><a name="p568184012612"></a><a name="p568184012612"></a>nsq/2*96，其中<span class="parmname" id="parmname1170114418287"><a name="parmname1170114418287"></a><a name="parmname1170114418287"></a>“nsq”</span>为子空间数量。</p>
</td>
</tr>
<tr id="row11211726184714"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p1258316232715"><a name="p1258316232715"></a><a name="p1258316232715"></a>LUT_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p6403112617719"><a name="p6403112617719"></a><a name="p6403112617719"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p1258316212714"><a name="p1258316212714"></a><a name="p1258316212714"></a>距离表数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1658311212279"><a name="p1658311212279"></a><a name="p1658311212279"></a>nsq*16，其中<span class="parmname" id="parmname584361843817"><a name="parmname584361843817"></a><a name="parmname584361843817"></a>“nsq”</span>为子空间数量。</p>
</td>
</tr>
<tr id="row172114262476"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p1613312110277"><a name="p1613312110277"></a><a name="p1613312110277"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p1699263912712"><a name="p1699263912712"></a><a name="p1699263912712"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p21335117279"><a name="p21335117279"></a><a name="p21335117279"></a>存储距离结果数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p41335118277"><a name="p41335118277"></a><a name="p41335118277"></a>限制为96。</p>
</td>
</tr>
<tr id="row11201326164720"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p172182719273"><a name="p172182719273"></a><a name="p172182719273"></a>lt_mask_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p119923399274"><a name="p119923399274"></a><a name="p119923399274"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p92127202712"><a name="p92127202712"></a><a name="p92127202712"></a>过滤压缩结果数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1421327132714"><a name="p1421327132714"></a><a name="p1421327132714"></a>限制为3。</p>
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
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a>正常运行时返回0，异常退出返回对应错误码。</p>
</td>
</tr>
</tbody>
</table>

**使用示例**

```c
#include <stdio.h>
#include <stdlib.h>
#include <string.h>
#include "krl.h"

int main() {
    // 4bit PQ参数配置（L2距离，blocksize=96）
    int nsq = 64;           // 子空间数量（必须为偶数）
    int ncode = 96;         // 底库向量数量（固定为96）
    int ksub = 16;          // 4bit索引

    // 准备码本（4bit打包，blocksize=96）
    size_t codes_size = (nsq / 2) * ncode;
    uint8_t* codes = (uint8_t*)malloc(codes_size * sizeof(uint8_t));
    
    for (size_t i = 0; i < codes_size; i++) {
        uint8_t low = rand() % ksub;
        uint8_t high = rand() % ksub;
        codes[i] = (high << 4) | low;
    }

    // 准备L2距离表（LUT）
    size_t LUT_size = nsq * ksub;
    uint8_t* LUT = (uint8_t*)malloc(LUT_size * sizeof(uint8_t));
    for (size_t i = 0; i < LUT_size; i++) {
        LUT[i] = (uint8_t)(rand() % 256);
    }

    // 准备距离结果数组
    uint16_t* distances = (uint16_t*)malloc(ncode * sizeof(uint16_t));

    // 准备过滤掩码数组
    // 96个向量需要3个uint32（96 / 32 = 3）
    size_t lt_mask_size = 3;
    uint32_t* lt_mask = (uint32_t*)malloc(lt_mask_size * sizeof(uint32_t));
    memset(lt_mask, 0, lt_mask_size * sizeof(uint32_t));

    // 执行L2距离的4bit查表累和过滤（blocksize=96）
    uint16_t threshold = 10000;
    int ret = krl_L2_table_lookup_fast_scan_bs96(
        nsq,
        codes,
        LUT,
        distances,
        threshold,
        lt_mask,
        codes_size,
        LUT_size,
        ncode,       // dis_size固定为96
        lt_mask_size
    );

    if (ret != 0) {
        printf("L2 4bit查表累和过滤（bs96）失败，错误码: %d\n", ret);
        goto cleanup;
    }

    printf("L2 4bit查表累和过滤（bs96）计算成功\n");

    // 统计满足条件的向量
    int count = 0;
    for (int i = 0; i < ncode; i++) {
        int mask_idx = i / 32;
        int bit_idx = i % 32;
        if (lt_mask[mask_idx] & (1u << bit_idx)) {
            count++;
        }
    }
    printf("共%d个向量满足L2距离 < %u\n", count, threshold);

cleanup:
    free(codes);
    free(LUT);
    free(distances);
    free(lt_mask);

    return ret;
}
```

### krl\_IP\_table\_lookup\_fast\_scan\_bs96

**接口定义<a name="section172317194488"></a>**

int krl\_IP\_table\_lookup\_fast\_scan\_bs96\(int nsq, const uint8\_t\* codes, const uint8\_t\* LUT, uint16\_t\* dis, uint16\_t threshold, uint32\_t\* lt\_mask, size\_t codes\_size, size\_t LUT\_size, size\_t dis\_size, size\_t lt\_mask\_size\);

**接口用途<a name="section1153124784912"></a>**

单独处理数据类型为float的查询向量的4比特查表累和过滤压缩算子。计算1个查询向量与96个底库向量间的内积距离。根据距离类型决定比较规则，将距离值满足比较规则的底库向量的lt\_mask设置为1，反之为0。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.601460146014599%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.903390339033905%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="35.94359435943594%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row166241441532"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p262494414531"><a name="p262494414531"></a><a name="p262494414531"></a>nsq</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p126241544125310"><a name="p126241544125310"></a><a name="p126241544125310"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="33.903390339033905%" headers="mcps1.1.5.1.3 "><p id="p1562414447536"><a name="p1562414447536"></a><a name="p1562414447536"></a>子空间数量。</p>
</td>
<td class="cellrowborder" valign="top" width="35.94359435943594%" headers="mcps1.1.5.1.4 "><p id="p19624744195313"><a name="p19624744195313"></a><a name="p19624744195313"></a>[1,256]且为偶数。</p>
</td>
</tr>
<tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p14381721205612"><a name="p14381721205612"></a><a name="p14381721205612"></a>codes</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7438122115569"><a name="p7438122115569"></a><a name="p7438122115569"></a>const uint8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.903390339033905%" headers="mcps1.1.5.1.3 "><p id="p18438121155616"><a name="p18438121155616"></a><a name="p18438121155616"></a>码本，使用krl_pack_codes_4b（blocksize=96）处理后底库向量对应的索引。</p>
</td>
<td class="cellrowborder" valign="top" width="35.94359435943594%" headers="mcps1.1.5.1.4 "><p id="p51251625162911"><a name="p51251625162911"></a><a name="p51251625162911"></a>限制长度为codes_size，其中<span class="parmname" id="parmname18125825132915"><a name="parmname18125825132915"></a><a name="parmname18125825132915"></a>“codes_size”</span>为码本数组的长度。</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4982142445414"><a name="p4982142445414"></a><a name="p4982142445414"></a>LUT</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7532158856"><a name="p7532158856"></a><a name="p7532158856"></a>const uint8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.903390339033905%" headers="mcps1.1.5.1.3 "><p id="p36611261054"><a name="p36611261054"></a><a name="p36611261054"></a>各子空间中PQ质心与查询向量的uint8距离表。</p>
</td>
<td class="cellrowborder" valign="top" width="35.94359435943594%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>限制长度为LUT_size，其中<span class="parmname" id="parmname551215813519"><a name="parmname551215813519"></a><a name="parmname551215813519"></a>“LUT_size”</span>为距离表数组的长度。</p>
</td>
</tr>
<tr id="row103951453161513"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p14723141215409"><a name="p14723141215409"></a><a name="p14723141215409"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p4723181210404"><a name="p4723181210404"></a><a name="p4723181210404"></a>uint16_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.903390339033905%" headers="mcps1.1.5.1.3 "><p id="p672341218403"><a name="p672341218403"></a><a name="p672341218403"></a>存储计算所得的距离结果。</p>
</td>
<td class="cellrowborder" valign="top" width="35.94359435943594%" headers="mcps1.1.5.1.4 "><p id="p57801052141013"><a name="p57801052141013"></a><a name="p57801052141013"></a>限制长度为dis_size，其中<span class="parmname" id="parmname1048505120457"><a name="parmname1048505120457"></a><a name="parmname1048505120457"></a>“dis_size”</span>为存储距离结果数组的长度。需预先分配内存。</p>
</td>
</tr>
<tr id="row1875218456372"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p275311453374"><a name="p275311453374"></a><a name="p275311453374"></a>threshold</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7753045173714"><a name="p7753045173714"></a><a name="p7753045173714"></a>const uint16_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.903390339033905%" headers="mcps1.1.5.1.3 "><p id="p17531445103716"><a name="p17531445103716"></a><a name="p17531445103716"></a>距离阈值。</p>
</td>
<td class="cellrowborder" valign="top" width="35.94359435943594%" headers="mcps1.1.5.1.4 "><p id="p748810273302"><a name="p748810273302"></a><a name="p748810273302"></a>限制为65535。</p>
</td>
</tr>
<tr id="row143744955610"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p34370492563"><a name="p34370492563"></a><a name="p34370492563"></a>lt_mask</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p3437549145616"><a name="p3437549145616"></a><a name="p3437549145616"></a>uint32_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.903390339033905%" headers="mcps1.1.5.1.3 "><p id="p143715495569"><a name="p143715495569"></a><a name="p143715495569"></a>过滤压缩结果。</p>
</td>
<td class="cellrowborder" valign="top" width="35.94359435943594%" headers="mcps1.1.5.1.4 "><p id="p77615321231"><a name="p77615321231"></a><a name="p77615321231"></a>限制长度为lt_mask_size，其中<span class="parmname" id="parmname10988163762914"><a name="parmname10988163762914"></a><a name="parmname10988163762914"></a>“lt_mask_size”</span>为过滤压缩结果数组的长度。需预先分配内存。</p>
</td>
</tr>
<tr id="row3115131755217"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p11681640172619"><a name="p11681640172619"></a><a name="p11681640172619"></a>codes_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p06662231878"><a name="p06662231878"></a><a name="p06662231878"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.903390339033905%" headers="mcps1.1.5.1.3 "><p id="p16681940142616"><a name="p16681940142616"></a><a name="p16681940142616"></a>码本数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.94359435943594%" headers="mcps1.1.5.1.4 "><p id="p568184012612"><a name="p568184012612"></a><a name="p568184012612"></a>nsq/2*96，其中<span class="parmname" id="parmname1170114418287"><a name="parmname1170114418287"></a><a name="parmname1170114418287"></a>“nsq”</span>为子空间数量。</p>
</td>
</tr>
<tr id="row511551717527"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p1258316232715"><a name="p1258316232715"></a><a name="p1258316232715"></a>LUT_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p6403112617719"><a name="p6403112617719"></a><a name="p6403112617719"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.903390339033905%" headers="mcps1.1.5.1.3 "><p id="p1258316212714"><a name="p1258316212714"></a><a name="p1258316212714"></a>距离表数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.94359435943594%" headers="mcps1.1.5.1.4 "><p id="p1658311212279"><a name="p1658311212279"></a><a name="p1658311212279"></a>nsq*16，其中<span class="parmname" id="parmname584361843817"><a name="parmname584361843817"></a><a name="parmname584361843817"></a>“nsq”</span>为子空间数量。</p>
</td>
</tr>
<tr id="row11115201711529"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p1613312110277"><a name="p1613312110277"></a><a name="p1613312110277"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p1699263912712"><a name="p1699263912712"></a><a name="p1699263912712"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.903390339033905%" headers="mcps1.1.5.1.3 "><p id="p21335117279"><a name="p21335117279"></a><a name="p21335117279"></a>存储距离结果数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.94359435943594%" headers="mcps1.1.5.1.4 "><p id="p41335118277"><a name="p41335118277"></a><a name="p41335118277"></a>限制为96。</p>
</td>
</tr>
<tr id="row111141217155212"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p172182719273"><a name="p172182719273"></a><a name="p172182719273"></a>lt_mask_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p119923399274"><a name="p119923399274"></a><a name="p119923399274"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.903390339033905%" headers="mcps1.1.5.1.3 "><p id="p92127202712"><a name="p92127202712"></a><a name="p92127202712"></a>过滤压缩结果数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.94359435943594%" headers="mcps1.1.5.1.4 "><p id="p1421327132714"><a name="p1421327132714"></a><a name="p1421327132714"></a>限制为3。</p>
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
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a>正常运行时返回0，异常退出返回对应错误码。</p>
</td>
</tr>
</tbody>
</table>

**使用示例**

```c
#include <stdio.h>
#include <stdlib.h>
#include <string.h>
#include "krl.h"

int main() {
    // 4bit PQ参数配置（内积距离，blocksize=96）
    int nsq = 64;
    int ncode = 96;
    int ksub = 16;

    // 准备码本
    size_t codes_size = (nsq / 2) * ncode;
    uint8_t* codes = (uint8_t*)malloc(codes_size * sizeof(uint8_t));
    for (size_t i = 0; i < codes_size; i++) {
        uint8_t low = rand() % ksub;
        uint8_t high = rand() % ksub;
        codes[i] = (high << 4) | low;
    }

    // 准备内积距离表
    size_t LUT_size = nsq * ksub;
    uint8_t* LUT = (uint8_t*)malloc(LUT_size * sizeof(uint8_t));
    for (size_t i = 0; i < LUT_size; i++) {
        LUT[i] = (uint8_t)(rand() % 256);
    }

    // 准备结果数组
    uint16_t* distances = (uint16_t*)malloc(ncode * sizeof(uint16_t));
    size_t lt_mask_size = 3;
    uint32_t* lt_mask = (uint32_t*)malloc(lt_mask_size * sizeof(uint32_t));
    memset(lt_mask, 0, lt_mask_size * sizeof(uint32_t));

    // 执行内积距离的4bit查表累和过滤（bs96）
    uint16_t threshold = 5000;
    int ret = krl_IP_table_lookup_fast_scan_bs96(
        nsq,
        codes,
        LUT,
        distances,
        threshold,
        lt_mask,
        codes_size,
        LUT_size,
        ncode,
        lt_mask_size
    );

    if (ret != 0) {
        printf("IP 4bit查表累和过滤（bs96）失败，错误码: %d\n", ret);
        goto cleanup;
    }

    printf("IP 4bit查表累和过滤（bs96）计算成功\n");

    // 输出Top-5最大内积
    printf("Top-5 最大内积:\n");
    for (int k = 0; k < 5; k++) {
        uint16_t max_val = 0;
        int max_idx = -1;
        for (int i = 0; i < ncode; i++) {
            if (distances[i] > max_val) {
                max_val = distances[i];
                max_idx = i;
            }
        }
        if (max_idx >= 0) {
            printf("  第%d名: 向量[%d], 内积 = %u\n", k + 1, max_idx, max_val);
            distances[max_idx] = 0;  // 标记已选
        }
    }

cleanup:
    free(codes);
    free(LUT);
    free(distances);
    free(lt_mask);

    return ret;
}
```

### krl\_table\_lookup\_4b\_f16

**接口定义<a name="section172317194488"></a>**

int krl\_table\_lookup\_4b\_f16\(size\_t nsq, size\_t ncode, const uint8\_t\* codes, const uint16\_t\* LUT, float\* dis, uint16\_t dis0, size\_t codes\_size, size\_t LUT\_size, size\_t dis\_size\);

**接口用途<a name="section1153124784912"></a>**

单独处理数据类型为fp16的查询向量的4比特查表累和过滤压缩算子。计算1个查询向量与多个底库向量间的内积距离，距离的初始值为dis0。此接口不会进行过滤压缩（与阈值进行比较）。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.601460146014599%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row166241441532"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p262494414531"><a name="p262494414531"></a><a name="p262494414531"></a>nsq</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p126241544125310"><a name="p126241544125310"></a><a name="p126241544125310"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p1562414447536"><a name="p1562414447536"></a><a name="p1562414447536"></a>子空间数量。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p19624744195313"><a name="p19624744195313"></a><a name="p19624744195313"></a>[1,65535]且为偶数。</p>
</td>
</tr>
<tr id="row8437621111217"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p943722161218"><a name="p943722161218"></a><a name="p943722161218"></a>ncode</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p19437152117123"><a name="p19437152117123"></a><a name="p19437152117123"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p543720213125"><a name="p543720213125"></a><a name="p543720213125"></a>底库向量总数。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p743792191219"><a name="p743792191219"></a><a name="p743792191219"></a>[1,2^30-1]</p>
</td>
</tr>
<tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p14381721205612"><a name="p14381721205612"></a><a name="p14381721205612"></a>codes</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7438122115569"><a name="p7438122115569"></a><a name="p7438122115569"></a>const uint8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p18438121155616"><a name="p18438121155616"></a><a name="p18438121155616"></a>码本，使用krl_pack_codes_4b（blocksize=64）处理后底库向量对应的索引。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p51251625162911"><a name="p51251625162911"></a><a name="p51251625162911"></a>限制长度为codes_size，其中<span class="parmname" id="parmname18125825132915"><a name="parmname18125825132915"></a><a name="parmname18125825132915"></a>“codes_size”</span>为码本数组的长度。</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p734604031220"><a name="p734604031220"></a><a name="p734604031220"></a>LUT</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7532158856"><a name="p7532158856"></a><a name="p7532158856"></a>const uint16_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p36611261054"><a name="p36611261054"></a><a name="p36611261054"></a>各子空间中PQ质心与查询向量的fp16距离表。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>限制长度为LUT_size，其中<span class="parmname" id="parmname551215813519"><a name="parmname551215813519"></a><a name="parmname551215813519"></a>“LUT_size”</span>为距离表数组的长度。</p>
</td>
</tr>
<tr id="row103951453161513"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p14723141215409"><a name="p14723141215409"></a><a name="p14723141215409"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p4723181210404"><a name="p4723181210404"></a><a name="p4723181210404"></a>float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p672341218403"><a name="p672341218403"></a><a name="p672341218403"></a>存储计算所得的距离结果。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p57801052141013"><a name="p57801052141013"></a><a name="p57801052141013"></a>限制长度为dis_size，其中<span class="parmname" id="parmname1048505120457"><a name="parmname1048505120457"></a><a name="parmname1048505120457"></a>“dis_size”</span>为存储距离结果数组的长度。需预先分配内存。</p>
</td>
</tr>
<tr id="row1875218456372"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p564545281211"><a name="p564545281211"></a><a name="p564545281211"></a>dis0</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7753045173714"><a name="p7753045173714"></a><a name="p7753045173714"></a>uint16_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p17531445103716"><a name="p17531445103716"></a><a name="p17531445103716"></a>初始距离。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p69179904614"><a name="p69179904614"></a><a name="p69179904614"></a>浮点数。</p>
</td>
</tr>
<tr id="row5701164775910"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p137414311617"><a name="p137414311617"></a><a name="p137414311617"></a>codes_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p06662231878"><a name="p06662231878"></a><a name="p06662231878"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p16744431269"><a name="p16744431269"></a><a name="p16744431269"></a>码本数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p127494317611"><a name="p127494317611"></a><a name="p127494317611"></a>nsq/2*ncode，其中<span class="parmname" id="parmname4131155510115"><a name="parmname4131155510115"></a><a name="parmname4131155510115"></a>“nsq”</span>为子空间数量，<span class="parmname" id="parmname1013120552111"><a name="parmname1013120552111"></a><a name="parmname1013120552111"></a>“ncode”</span>为底库向量总数。</p>
</td>
</tr>
<tr id="row97004477597"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p1258316232715"><a name="p1258316232715"></a><a name="p1258316232715"></a>LUT_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p6403112617719"><a name="p6403112617719"></a><a name="p6403112617719"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p1258316212714"><a name="p1258316212714"></a><a name="p1258316212714"></a>距离表数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1658311212279"><a name="p1658311212279"></a><a name="p1658311212279"></a>nsq*16，其中<span class="parmname" id="parmname584361843817"><a name="parmname584361843817"></a><a name="parmname584361843817"></a>“nsq”</span>为子空间数量。</p>
</td>
</tr>
<tr id="row67009473597"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p1753316619720"><a name="p1753316619720"></a><a name="p1753316619720"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p64039264714"><a name="p64039264714"></a><a name="p64039264714"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p54111354134020"><a name="p54111354134020"></a><a name="p54111354134020"></a>存储距离结果数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p175331661478"><a name="p175331661478"></a><a name="p175331661478"></a>ncode，其中<span class="parmname" id="parmname89954141011"><a name="parmname89954141011"></a><a name="parmname89954141011"></a>“ncode”</span>为底库向量总数。</p>
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
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a>正常运行时返回0，异常退出返回对应错误码。</p>
</td>
</tr>
</tbody>
</table>

**使用示例**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

// 辅助函数：将float转换为fp16
uint16_t float_to_fp16(float value);

int main() {
    // 4bit PQ参数配置（fp16距离表）
    size_t nsq = 64;        // 子空间数量（必须为偶数）
    size_t ncode = 1000;    // 底库向量总数
    size_t ksub = 16;       // 4bit索引

    // 准备码本（4bit打包）
    size_t codes_size = (nsq / 2) * ncode;
    uint8_t* codes = (uint8_t*)malloc(codes_size * sizeof(uint8_t));
    for (size_t i = 0; i < codes_size; i++) {
        uint8_t low = rand() % ksub;
        uint8_t high = rand() % ksub;
        codes[i] = (high << 4) | low;
    }

    // 准备fp16距离表
    size_t LUT_size = nsq * ksub;
    uint16_t* LUT = (uint16_t*)malloc(LUT_size * sizeof(uint16_t));
    for (size_t i = 0; i < LUT_size; i++) {
        // 将距离值转换为fp16格式
        float dist = (float)(rand() % 1000) / 100.0f;
        LUT[i] = float_to_fp16(dist);
    }

    // 准备距离结果数组（输出为float）
    float* distances = (float*)malloc(ncode * sizeof(float));

    // 执行fp16的4bit查表累和
    uint16_t dis0 = float_to_fp16(0.0f);  // 初始距离为0
    int ret = krl_table_lookup_4b_f16(
        nsq,
        ncode,
        codes,
        LUT,
        distances,
        dis0,
        codes_size,
        LUT_size,
        ncode
    );

    if (ret != 0) {
        printf("fp16 4bit查表累和失败，错误码: %d\n", ret);
        goto cleanup;
    }

    printf("fp16 4bit查表累和计算成功\n");

    // 找出最小距离（最近邻）
    float min_dist = distances[0];
    size_t min_idx = 0;
    for (size_t i = 1; i < ncode; i++) {
        if (distances[i] < min_dist) {
            min_dist = distances[i];
            min_idx = i;
        }
    }
    printf("最近邻: 索引=%zu, PQ距离=%f\n", min_idx, min_dist);

cleanup:
    free(codes);
    free(LUT);
    free(distances);

    return ret;
}
```

### krl\_pack\_codes\_4b

**接口定义<a name="section172317194488"></a>**

int krl\_pack\_codes\_4b\(const uint8\_t\* codes, size\_t ncode, size\_t nsq, uint8\_t\* blocks, size\_t batchsize, int dim\_cross, size\_t codes\_size, size\_t blocks\_size\);

**接口用途<a name="section1153124784912"></a>**

单独处理数据类型为fp16的查询向量的4比特查表累和过滤压缩算子。计算1个查询向量与多个底库向量间的内积距离，距离的初始值为dis\_f16。此接口不会进行过滤压缩（与阈值进行比较）。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.541554155415543%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.611461146114612%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p14381721205612"><a name="p14381721205612"></a><a name="p14381721205612"></a>codes</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p7438122115569"><a name="p7438122115569"></a><a name="p7438122115569"></a>const uint8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p18438121155616"><a name="p18438121155616"></a><a name="p18438121155616"></a>底库向量数据。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p13438102185617"><a name="p13438102185617"></a><a name="p13438102185617"></a>限制长度为codes_size，其中<span class="parmname" id="parmname18125825132915"><a name="parmname18125825132915"></a><a name="parmname18125825132915"></a>“codes_size”</span>为底库向量数组的长度。</p>
</td>
</tr>
<tr id="row587315210197"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p14873021151914"><a name="p14873021151914"></a><a name="p14873021151914"></a>ncode</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p887382119197"><a name="p887382119197"></a><a name="p887382119197"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p287382118190"><a name="p287382118190"></a><a name="p287382118190"></a>底库向量总数。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>[1,2^30-1]</p>
</td>
</tr>
<tr id="row18840143271918"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p4840832111916"><a name="p4840832111916"></a><a name="p4840832111916"></a>nsq</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p68401332181920"><a name="p68401332181920"></a><a name="p68401332181920"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p08401632111917"><a name="p08401632111917"></a><a name="p08401632111917"></a>子空间数量。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p20840123241914"><a name="p20840123241914"></a><a name="p20840123241914"></a>[1,65535]</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p734604031220"><a name="p734604031220"></a><a name="p734604031220"></a>blocks</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p7532158856"><a name="p7532158856"></a><a name="p7532158856"></a>uint8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p36611261054"><a name="p36611261054"></a><a name="p36611261054"></a>pack后的底库向量数据。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>限制长度为blocks_size，其中<span class="parmname" id="parmname204555717"><a name="parmname204555717"></a><a name="parmname204555717"></a>“blocks_size”</span>为pack后的底库向量数组的长度。需预先分配内存。</p>
</td>
</tr>
<tr id="row103951453161513"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p14723141215409"><a name="p14723141215409"></a><a name="p14723141215409"></a>batchsize</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p4723181210404"><a name="p4723181210404"></a><a name="p4723181210404"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p672341218403"><a name="p672341218403"></a><a name="p672341218403"></a>底库向量分块大小。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p6723181274010"><a name="p6723181274010"></a><a name="p6723181274010"></a>大于0且为16的倍数。需要与查表累和算子相适应。</p>
<a name="ul1810376145316"></a><a name="ul1810376145316"></a><ul id="ul1810376145316"><li>设置为32：</li></ul>
<p id="p2989163595213"><a name="p2989163595213"></a><a name="p2989163595213"></a>krl_table_lookup_step</p>
<a name="ul342518815320"></a><a name="ul342518815320"></a><ul id="ul342518815320"><li>设置为64：</li></ul>
<p id="p19989135155218"><a name="p19989135155218"></a><a name="p19989135155218"></a>krl_L2_table_lookup_fast_scan_bs64</p>
<p id="p398933517522"><a name="p398933517522"></a><a name="p398933517522"></a>krl_IP_table_lookup_fast_scan_bs64</p>
<p id="p1998973515521"><a name="p1998973515521"></a><a name="p1998973515521"></a>krl_table_lookup_4b_f16</p>
<a name="ul13296171112536"></a><a name="ul13296171112536"></a><ul id="ul13296171112536"><li>设置为96：</li></ul>
<p id="p3989203517528"><a name="p3989203517528"></a><a name="p3989203517528"></a>krl_L2_table_lookup_fast_scan_bs96</p>
<p id="p16989173512524"><a name="p16989173512524"></a><a name="p16989173512524"></a>krl_IP_table_lookup_fast_scan_bs96</p>
</td>
</tr>
<tr id="row1875218456372"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p564545281211"><a name="p564545281211"></a><a name="p564545281211"></a>dim_cross</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p7753045173714"><a name="p7753045173714"></a><a name="p7753045173714"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p17531445103716"><a name="p17531445103716"></a><a name="p17531445103716"></a>距离数据是否为8bit</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p69179904614"><a name="p69179904614"></a><a name="p69179904614"></a>[0,1]，取值表示距离数据是否为8bit：</p>
<a name="ul164886121012"></a><a name="ul164886121012"></a><ul id="ul164886121012"><li>0：距离数据为8bit。</li><li>1:  距离数据为16bit。</li></ul>
</td>
</tr>
<tr id="row67711025367"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p137414311617"><a name="p137414311617"></a><a name="p137414311617"></a>codes_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p06662231878"><a name="p06662231878"></a><a name="p06662231878"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p16744431269"><a name="p16744431269"></a><a name="p16744431269"></a>底库向量数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p127494317611"><a name="p127494317611"></a><a name="p127494317611"></a>ncode*nsq/2，其中<span class="parmname" id="parmname1078717121273"><a name="parmname1078717121273"></a><a name="parmname1078717121273"></a>“ncode”</span>为底库向量总数，<span class="parmname" id="parmname07871121373"><a name="parmname07871121373"></a><a name="parmname07871121373"></a>“nsq”</span>为子空间数量。</p>
</td>
</tr>
<tr id="row4903281565"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p292753515619"><a name="p292753515619"></a><a name="p292753515619"></a>blocks_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p15927335864"><a name="p15927335864"></a><a name="p15927335864"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p2927183515614"><a name="p2927183515614"></a><a name="p2927183515614"></a>pack后的底库向量数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p99271635566"><a name="p99271635566"></a><a name="p99271635566"></a>ceil(ncode/batchsize)*batchsize*ceil(nsq/2)，其中<span class="parmname" id="parmname81372591969"><a name="parmname81372591969"></a><a name="parmname81372591969"></a>“ncode”</span>为底库向量总数，<span class="parmname" id="parmname101371859767"><a name="parmname101371859767"></a><a name="parmname101371859767"></a>“batchsize”</span>为底库向量分块大小，<span class="parmname" id="parmname813745915619"><a name="parmname813745915619"></a><a name="parmname813745915619"></a>“nsq”</span>为子空间数量。</p>
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
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a>正常运行时返回0，异常退出返回对应错误码。</p>
</td>
</tr>
</tbody>
</table>

**使用示例**

```c
#include <stdio.h>
#include <stdlib.h>
#include <math.h>
#include "krl.h"

int main() {
    // 参数配置
    size_t ncode = 10000;   // 底库向量总数
    size_t nsq = 64;        // 子空间数量
    size_t batchsize = 64;  // 分块大小（对应bs64接口）
    int dim_cross = 0;      // 使用8bit距离

    // 准备原始4bit码本
    // 原始格式：每个向量有nsq个4bit索引
    // 存储时每2个4bit索引打包为1个uint8
    size_t codes_size = ncode * nsq / 2;
    uint8_t* codes = (uint8_t*)malloc(codes_size * sizeof(uint8_t));
    
    // 模拟原始码本数据
    for (size_t i = 0; i < codes_size; i++) {
        uint8_t low = rand() % 16;   // 低4位：0-15
        uint8_t high = rand() % 16;  // 高4位：0-15
        codes[i] = (high << 4) | low;
    }

    // 计算pack后的数组大小
    size_t num_blocks = (ncode + batchsize - 1) / batchsize;  // 向上取整
    size_t blocks_size = num_blocks * batchsize * ((nsq + 1) / 2);
    uint8_t* blocks = (uint8_t*)malloc(blocks_size * sizeof(uint8_t));

    // 执行码本打包
    int ret = krl_pack_codes_4b(
        codes,
        ncode,
        nsq,
        blocks,
        batchsize,
        dim_cross,
        codes_size,
        blocks_size
    );

    if (ret != 0) {
        printf("码本打包失败，错误码: %d\n", ret);
        goto cleanup;
    }

    printf("4bit码本打包成功\n");
    printf("  原始码本大小: %zu bytes\n", codes_size);
    printf("  打包后大小: %zu bytes\n", blocks_size);
    printf("  分块大小: %zu\n", batchsize);
    printf("  分块数量: %zu\n", num_blocks);

    // 现在可以使用blocks进行快速查表
    // 例如：krl_L2_table_lookup_fast_scan_bs64(...)

cleanup:
    free(codes);
    free(blocks);

    return ret;
}
```

## 重排接口

### krl\_reorder\_2\_vector

**接口定义<a name="section172317194488"></a>**

int krl\_reorder\_2\_vector\(const KRLDistanceHandle\* kdh, int64\_t base\_k, float\* base\_dis, int64\_t\* base\_idx, const float\* query\_vector, int64\_t k, float\* dis, int64\_t\* idx, size\_t query\_vector\_size\);

**接口用途<a name="section1153124784912"></a>**

计算1个查询向量与多个不连续底库向量间的高精度距离并排序。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.541554155415543%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.611461146114612%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="29.532953295329534%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="40.31403140314032%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p14381721205612"><a name="p14381721205612"></a><a name="p14381721205612"></a>kdh</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p7438122115569"><a name="p7438122115569"></a><a name="p7438122115569"></a>const KRLDistanceHandle*</p>
</td>
<td class="cellrowborder" valign="top" width="29.532953295329534%" headers="mcps1.1.5.1.3 "><p id="p18438121155616"><a name="p18438121155616"></a><a name="p18438121155616"></a>KRLDistanceHandle指针。</p>
</td>
<td class="cellrowborder" valign="top" width="40.31403140314032%" headers="mcps1.1.5.1.4 "><p id="p13438102185617"><a name="p13438102185617"></a><a name="p13438102185617"></a>限制非空。需使用krl_create_reorder_handle初始化。</p>
</td>
</tr>
<tr id="row587315210197"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p14873021151914"><a name="p14873021151914"></a><a name="p14873021151914"></a>base_k</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p887382119197"><a name="p887382119197"></a><a name="p887382119197"></a>int64_t</p>
</td>
<td class="cellrowborder" valign="top" width="29.532953295329534%" headers="mcps1.1.5.1.3 "><p id="p287382118190"><a name="p287382118190"></a><a name="p287382118190"></a>使用低精度检索算法得到的候选点数量。</p>
</td>
<td class="cellrowborder" valign="top" width="40.31403140314032%" headers="mcps1.1.5.1.4 "><p id="p1487318214195"><a name="p1487318214195"></a><a name="p1487318214195"></a>[k,codes_num]，其中<span class="parmname" id="parmname03911818344"><a name="parmname03911818344"></a><a name="parmname03911818344"></a>“k”</span>为最近邻点数量，<span class="parmname" id="parmname23948153415"><a name="parmname23948153415"></a><a name="parmname23948153415"></a>“codes_num”</span>为每个查询向量计算的底库向量数量。</p>
</td>
</tr>
<tr id="row18840143271918"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p4840832111916"><a name="p4840832111916"></a><a name="p4840832111916"></a>base_dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p68401332181920"><a name="p68401332181920"></a><a name="p68401332181920"></a>float*</p>
</td>
<td class="cellrowborder" valign="top" width="29.532953295329534%" headers="mcps1.1.5.1.3 "><p id="p08401632111917"><a name="p08401632111917"></a><a name="p08401632111917"></a>使用低精度检索算法得到的低精度距离。</p>
</td>
<td class="cellrowborder" valign="top" width="40.31403140314032%" headers="mcps1.1.5.1.4 "><p id="p20840123241914"><a name="p20840123241914"></a><a name="p20840123241914"></a>限制长度为base_k，其中<span class="parmname" id="parmname95721316125517"><a name="parmname95721316125517"></a><a name="parmname95721316125517"></a>“base_k”</span>为使用低精度检索算法得到的候选点数量。</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p734604031220"><a name="p734604031220"></a><a name="p734604031220"></a>base_idx</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p7532158856"><a name="p7532158856"></a><a name="p7532158856"></a>int64_t*</p>
</td>
<td class="cellrowborder" valign="top" width="29.532953295329534%" headers="mcps1.1.5.1.3 "><p id="p36611261054"><a name="p36611261054"></a><a name="p36611261054"></a>使用低精度检索算法得到的候选点ID。</p>
</td>
<td class="cellrowborder" valign="top" width="40.31403140314032%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>限制长度为base_k，其中<span class="parmname" id="parmname17965921181220"><a name="parmname17965921181220"></a><a name="parmname17965921181220"></a>“base_k”</span>为使用低精度检索算法得到的候选点数量。[-1,codes_num]，其中<span class="parmname" id="parmname880205993515"><a name="parmname880205993515"></a><a name="parmname880205993515"></a>“codes_num”</span>为每个查询向量计算的底库向量数量。ID需单调递增。若存在无需计算的占位符-1，则需要集中于向量末尾。</p>
</td>
</tr>
<tr id="row103951453161513"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p14723141215409"><a name="p14723141215409"></a><a name="p14723141215409"></a>query_vector</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p4723181210404"><a name="p4723181210404"></a><a name="p4723181210404"></a>const float*</p>
</td>
<td class="cellrowborder" valign="top" width="29.532953295329534%" headers="mcps1.1.5.1.3 "><p id="p672341218403"><a name="p672341218403"></a><a name="p672341218403"></a>查询向量数据。</p>
</td>
<td class="cellrowborder" valign="top" width="40.31403140314032%" headers="mcps1.1.5.1.4 "><p id="p6723181274010"><a name="p6723181274010"></a><a name="p6723181274010"></a>限制长度为query_vector_size，其中<span class="parmname" id="parmname14495193514370"><a name="parmname14495193514370"></a><a name="parmname14495193514370"></a>“query_vector_size”</span>为查询向量数组的长度。</p>
</td>
</tr>
<tr id="row1875218456372"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p564545281211"><a name="p564545281211"></a><a name="p564545281211"></a>k</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p7753045173714"><a name="p7753045173714"></a><a name="p7753045173714"></a>int64_t</p>
</td>
<td class="cellrowborder" valign="top" width="29.532953295329534%" headers="mcps1.1.5.1.3 "><p id="p164563717334"><a name="p164563717334"></a><a name="p164563717334"></a>计算所得的最近邻点数量。</p>
</td>
<td class="cellrowborder" valign="top" width="40.31403140314032%" headers="mcps1.1.5.1.4 "><p id="p10984160193814"><a name="p10984160193814"></a><a name="p10984160193814"></a>[1,base_k]，其中<span class="parmname" id="parmname134564943817"><a name="parmname134564943817"></a><a name="parmname134564943817"></a>“base_k”</span>为使用低精度检索算法得到的候选点数量。</p>
</td>
</tr>
<tr id="row1959261153015"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p159201112305"><a name="p159201112305"></a><a name="p159201112305"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p95921611183016"><a name="p95921611183016"></a><a name="p95921611183016"></a>float*</p>
</td>
<td class="cellrowborder" valign="top" width="29.532953295329534%" headers="mcps1.1.5.1.3 "><p id="p5592171115307"><a name="p5592171115307"></a><a name="p5592171115307"></a>存储计算所得的最近邻点与查询向量间的距离。</p>
</td>
<td class="cellrowborder" valign="top" width="40.31403140314032%" headers="mcps1.1.5.1.4 "><p id="p5592141183018"><a name="p5592141183018"></a><a name="p5592141183018"></a>限制长度为k，其中<span class="parmname" id="parmname1754134103818"><a name="parmname1754134103818"></a><a name="parmname1754134103818"></a>“k”</span>为最近邻点数量。需预先分配内存。</p>
</td>
</tr>
<tr id="row8439920305"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p1243209163013"><a name="p1243209163013"></a><a name="p1243209163013"></a>idx</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p174410973020"><a name="p174410973020"></a><a name="p174410973020"></a>int64_t*</p>
</td>
<td class="cellrowborder" valign="top" width="29.532953295329534%" headers="mcps1.1.5.1.3 "><p id="p344169173011"><a name="p344169173011"></a><a name="p344169173011"></a>存储计算所得的最近邻点ID。</p>
</td>
<td class="cellrowborder" valign="top" width="40.31403140314032%" headers="mcps1.1.5.1.4 "><p id="p14445915305"><a name="p14445915305"></a><a name="p14445915305"></a>限制长度为k，其中<span class="parmname" id="parmname4523545103814"><a name="parmname4523545103814"></a><a name="parmname4523545103814"></a>“k”</span>为最近邻点数量。需预先分配内存。</p>
</td>
</tr>
<tr id="row76471455191816"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p16648125510182"><a name="p16648125510182"></a><a name="p16648125510182"></a>query_vector_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p11648125510182"><a name="p11648125510182"></a><a name="p11648125510182"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="29.532953295329534%" headers="mcps1.1.5.1.3 "><p id="p06484557186"><a name="p06484557186"></a><a name="p06484557186"></a>查询向量数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="40.31403140314032%" headers="mcps1.1.5.1.4 "><p id="p176481955171818"><a name="p176481955171818"></a><a name="p176481955171818"></a>dim，其中<span class="parmname" id="parmname1554714318208"><a name="parmname1554714318208"></a><a name="parmname1554714318208"></a>“dim”</span>为向量维度。</p>
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
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a>正常运行时返回0，异常退出返回对应错误码。</p>
</td>
</tr>
</tbody>
</table>

**使用示例**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

int main() {
    // 参数配置
    size_t dim = 128;           // 向量维度
    size_t codes_num = 100000;  // 底库向量总数
    int64_t base_k = 100;       // 低精度检索返回的候选点数量
    int64_t k = 10;             // 最终需要的Top-K结果
    int metric_type = 0;        // 0: L2距离

    // 准备底库向量数据
    float* base_vectors = (float*)malloc(codes_num * dim * sizeof(float));
    for (size_t i = 0; i < codes_num * dim; i++) {
        base_vectors[i] = (float)(rand() % 1000) / 100.0f;
    }

    // 创建重排Handle
    KRLDistanceHandle* kdh = NULL;
    int ret = krl_create_reorder_handle(
        &kdh,
        base_vectors,
        codes_num,
        dim,
        metric_type,
        codes_num * dim
    );
    if (ret != 0) {
        printf("创建重排Handle失败: %d\n", ret);
        free(base_vectors);
        return -1;
    }

    // 准备查询向量
    float* query_vector = (float*)malloc(dim * sizeof(float));
    for (size_t i = 0; i < dim; i++) {
        query_vector[i] = (float)(rand() % 1000) / 100.0f;
    }

    // 模拟低精度检索结果
    // 实际使用中，这些结果来自PQ或其他近似检索算法
    float* base_dis = (float*)malloc(base_k * sizeof(float));
    int64_t* base_idx = (int64_t*)malloc(base_k * sizeof(int64_t));
    
    // 模拟候选点ID（必须单调递增）
    for (int64_t i = 0; i < base_k; i++) {
        base_idx[i] = i * 100;  // ID: 0, 100, 200, ...
        base_dis[i] = (float)(rand() % 10000) / 10.0f;  // 低精度距离
    }

    // 分配结果数组
    float* result_dis = (float*)malloc(k * sizeof(float));
    int64_t* result_idx = (int64_t*)malloc(k * sizeof(int64_t));

    // 执行高精度重排
    ret = krl_reorder_2_vector(
        kdh,
        base_k,
        base_dis,
        base_idx,
        query_vector,
        k,
        result_dis,
        result_idx,
        dim
    );

    if (ret != 0) {
        printf("重排计算失败，错误码: %d\n", ret);
        goto cleanup;
    }

    // 输出结果
    printf("高精度重排完成，Top-%lld 结果:\n", (long long)k);
    for (int64_t i = 0; i < k; i++) {
        printf("  第%lld名: ID=%lld, 高精度距离=%f\n",
               (long long)(i + 1),
               (long long)result_idx[i],
               result_dis[i]);
    }

cleanup:
    krl_clean_reorder_handle(&kdh);
    free(base_vectors);
    free(query_vector);
    free(base_dis);
    free(base_idx);
    free(result_dis);
    free(result_idx);

    return ret;
}
```

### krl\_reorder\_2\_vector\_continuous

**接口定义<a name="section172317194488"></a>**

int krl\_reorder\_2\_vector\_continuous\(const KRLDistanceHandle\* kdh, int64\_t base\_k, int64\_t begin\_id, const float\* query\_vector, int64\_t k, float\* dis, int64\_t\* idx, size\_t query\_vector\_size\);

**接口用途<a name="section1153124784912"></a>**

计算1个查询向量与多个连续底库向量间的高精度距离并排序。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.541554155415543%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.611461146114612%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p14381721205612"><a name="p14381721205612"></a><a name="p14381721205612"></a>kdh</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p7438122115569"><a name="p7438122115569"></a><a name="p7438122115569"></a>const KRLDistanceHandle*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p18438121155616"><a name="p18438121155616"></a><a name="p18438121155616"></a>KRLDistanceHandle指针。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p13438102185617"><a name="p13438102185617"></a><a name="p13438102185617"></a>限制非空，需使用krl_create_reorder_handle初始化。</p>
</td>
</tr>
<tr id="row587315210197"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p14873021151914"><a name="p14873021151914"></a><a name="p14873021151914"></a>base_k</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p887382119197"><a name="p887382119197"></a><a name="p887382119197"></a>int64_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p287382118190"><a name="p287382118190"></a><a name="p287382118190"></a>使用低精度检索算法得到的候选点数量。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1487318214195"><a name="p1487318214195"></a><a name="p1487318214195"></a>[k,codes_num]，其中<span class="parmname" id="parmname03911818344"><a name="parmname03911818344"></a><a name="parmname03911818344"></a>“k”</span>为最近邻点数量，<span class="parmname" id="parmname23948153415"><a name="parmname23948153415"></a><a name="parmname23948153415"></a>“codes_num”</span>为每个查询向量计算的底库向量数量。</p>
</td>
</tr>
<tr id="row18840143271918"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p4840832111916"><a name="p4840832111916"></a><a name="p4840832111916"></a>begin_id</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p68401332181920"><a name="p68401332181920"></a><a name="p68401332181920"></a>int64_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p08401632111917"><a name="p08401632111917"></a><a name="p08401632111917"></a>参与计算的底库向量的起始ID</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p20840123241914"><a name="p20840123241914"></a><a name="p20840123241914"></a>[0,codes_num-base_k]，其中<span class="parmname" id="parmname465311317415"><a name="parmname465311317415"></a><a name="parmname465311317415"></a>“codes_num”</span>为每个查询向量计算的底库向量数量，<span class="parmname" id="parmname1943364604117"><a name="parmname1943364604117"></a><a name="parmname1943364604117"></a>“base_k”</span>为使用低精度检索算法得到的候选点数量。</p>
</td>
</tr>
<tr id="row103951453161513"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p14723141215409"><a name="p14723141215409"></a><a name="p14723141215409"></a>query_vector</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p4723181210404"><a name="p4723181210404"></a><a name="p4723181210404"></a>const float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p672341218403"><a name="p672341218403"></a><a name="p672341218403"></a>查询向量数据。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p6723181274010"><a name="p6723181274010"></a><a name="p6723181274010"></a>限制长度为query_vector_size，其中<span class="parmname" id="parmname14495193514370"><a name="parmname14495193514370"></a><a name="parmname14495193514370"></a>“query_vector_size”</span>为查询向量数组的长度。</p>
</td>
</tr>
<tr id="row1875218456372"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p564545281211"><a name="p564545281211"></a><a name="p564545281211"></a>k</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p7753045173714"><a name="p7753045173714"></a><a name="p7753045173714"></a>int64_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p164563717334"><a name="p164563717334"></a><a name="p164563717334"></a>计算所得的最近邻点数量。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p10984160193814"><a name="p10984160193814"></a><a name="p10984160193814"></a>[1,base_k]，其中<span class="parmname" id="parmname134564943817"><a name="parmname134564943817"></a><a name="parmname134564943817"></a>“base_k”</span>为使用低精度检索算法得到的候选点数量。</p>
</td>
</tr>
<tr id="row1959261153015"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p159201112305"><a name="p159201112305"></a><a name="p159201112305"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p95921611183016"><a name="p95921611183016"></a><a name="p95921611183016"></a>float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p5592171115307"><a name="p5592171115307"></a><a name="p5592171115307"></a>存储计算所得的最近邻点与查询向量间的距离。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p5592141183018"><a name="p5592141183018"></a><a name="p5592141183018"></a>限制长度为k，其中<span class="parmname" id="parmname1754134103818"><a name="parmname1754134103818"></a><a name="parmname1754134103818"></a>“k”</span>为最近邻点数量。需预先分配内存。</p>
</td>
</tr>
<tr id="row8439920305"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p1243209163013"><a name="p1243209163013"></a><a name="p1243209163013"></a>idx</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p174410973020"><a name="p174410973020"></a><a name="p174410973020"></a>int64_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p344169173011"><a name="p344169173011"></a><a name="p344169173011"></a>存储计算所得的最近邻点ID。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p14445915305"><a name="p14445915305"></a><a name="p14445915305"></a>限制长度为k，其中<span class="parmname" id="parmname4523545103814"><a name="parmname4523545103814"></a><a name="parmname4523545103814"></a>“k”</span>为最近邻点数量。需预先分配内存。</p>
</td>
</tr>
<tr id="row355263412118"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p16648125510182"><a name="p16648125510182"></a><a name="p16648125510182"></a>query_vector_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p11648125510182"><a name="p11648125510182"></a><a name="p11648125510182"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p06484557186"><a name="p06484557186"></a><a name="p06484557186"></a>查询向量数组的长度。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p176481955171818"><a name="p176481955171818"></a><a name="p176481955171818"></a>dim，其中<span class="parmname" id="parmname1554714318208"><a name="parmname1554714318208"></a><a name="parmname1554714318208"></a>“dim”</span>为向量维度。</p>
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
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a>正常运行时返回0，异常退出返回对应错误码。</p>
</td>
</tr>
</tbody>
</table>

**使用示例**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

int main() {
    // 参数配置
    size_t dim = 128;
    size_t codes_num = 100000;
    int64_t base_k = 1000;      // 连续候选点数量
    int64_t begin_id = 5000;    // 起始ID（例如某个聚类簇的起始位置）
    int64_t k = 10;             // 最终Top-K
    int metric_type = 0;        // L2距离

    // 准备底库向量
    float* base_vectors = (float*)malloc(codes_num * dim * sizeof(float));
    for (size_t i = 0; i < codes_num * dim; i++) {
        base_vectors[i] = (float)(rand() % 1000) / 100.0f;
    }

    // 创建重排Handle
    KRLDistanceHandle* kdh = NULL;
    int ret = krl_create_reorder_handle(
        &kdh, base_vectors, codes_num, dim, metric_type, codes_num * dim
    );
    if (ret != 0) {
        printf("创建重排Handle失败: %d\n", ret);
        free(base_vectors);
        return -1;
    }

    // 准备查询向量
    float* query_vector = (float*)malloc(dim * sizeof(float));
    for (size_t i = 0; i < dim; i++) {
        query_vector[i] = (float)(rand() % 1000) / 100.0f;
    }

    // 分配结果数组
    float* result_dis = (float*)malloc(k * sizeof(float));
    int64_t* result_idx = (int64_t*)malloc(k * sizeof(int64_t));

    // 执行连续向量的高精度重排
    ret = krl_reorder_2_vector_continuous(
        kdh,
        base_k,
        begin_id,
        query_vector,
        k,
        result_dis,
        result_idx,
        dim
    );

    if (ret != 0) {
        printf("连续重排计算失败，错误码: %d\n", ret);
        goto cleanup;
    }

    // 输出结果
    printf("连续向量重排完成\n");
    printf("搜索范围: ID [%lld, %lld)\n",
           (long long)begin_id,
           (long long)(begin_id + base_k));
    printf("Top-%lld 结果:\n", (long long)k);
    for (int64_t i = 0; i < k; i++) {
        printf("  第%lld名: ID=%lld, 距离=%f\n",
               (long long)(i + 1),
               (long long)result_idx[i],
               result_dis[i]);
    }

cleanup:
    krl_clean_reorder_handle(&kdh);
    free(base_vectors);
    free(query_vector);
    free(result_dis);
    free(result_idx);

    return ret;
}
```

## 保存/加载接口

### krl\_store\_LUT8Handle

**接口定义<a name="section172317194488"></a>**

int krl\_store\_LUT8Handle\(FILE\* f, const KRLLUT8bHandle\* klh\);

**接口用途<a name="section1153124784912"></a>**

将8bit查找表句柄保存到文件中。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.541554155415543%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.611461146114612%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p14381721205612"><a name="p14381721205612"></a><a name="p14381721205612"></a>f</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p7438122115569"><a name="p7438122115569"></a><a name="p7438122115569"></a>FILE*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p1018720320568"><a name="p1018720320568"></a><a name="p1018720320568"></a>写入的文件句柄。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p4187123185620"><a name="p4187123185620"></a><a name="p4187123185620"></a>限制非空。</p>
</td>
</tr>
<tr id="row587315210197"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p14873021151914"><a name="p14873021151914"></a><a name="p14873021151914"></a>klh</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p887382119197"><a name="p887382119197"></a><a name="p887382119197"></a>const KRLLUT8bHandle*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p287382118190"><a name="p287382118190"></a><a name="p287382118190"></a>KRLLUT8bHandle指针。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1487318214195"><a name="p1487318214195"></a><a name="p1487318214195"></a>限制非空。</p>
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
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a>正常运行时返回0，异常退出返回对应错误码。</p>
</td>
</tr>
</tbody>
</table>

**使用示例**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

// 保存Handle到文件
int save_lut8_handle(const char* filename, KRLLUT8bHandle* klh) {
    FILE* f = fopen(filename, "wb");
    if (f == NULL) {
        printf("无法打开文件进行写入: %s\n", filename);
        return -1;
    }

    int ret = krl_store_LUT8Handle(f, klh);
    fclose(f);

    if (ret == 0) {
        printf("LUT8bHandle已保存到: %s\n", filename);
    } else {
        printf("保存失败，错误码: %d\n", ret);
    }
    return ret;
}

// 从文件加载Handle
int load_lut8_handle(const char* filename, KRLLUT8bHandle** klh) {
    FILE* f = fopen(filename, "rb");
    if (f == NULL) {
        printf("无法打开文件进行读取: %s\n", filename);
        return -1;
    }

    int ret = krl_build_LUT8Handle_fromfile(f, klh);
    fclose(f);

    if (ret == 0) {
        printf("LUT8bHandle已从文件加载: %s\n", filename);
    } else {
        printf("加载失败，错误码: %d\n", ret);
    }
    return ret;
}

int main() {
    const char* filename = "lut8_handle.bin";
    
    // 创建并初始化Handle
    KRLLUT8bHandle* klh = NULL;
    int use_idx = 1;
    size_t capacity = 10000;
    
    int ret = krl_create_LUT8b_handle(&klh, use_idx, capacity);
    if (ret != 0) {
        printf("创建Handle失败\n");
        return -1;
    }

    // 设置一些数据
    size_t* idx_ptr = krl_get_idx_pointer(klh);
    for (size_t i = 0; i < 100; i++) {
        idx_ptr[i] = i * 10;
    }

    // 保存Handle
    ret = save_lut8_handle(filename, klh);
    if (ret != 0) {
        krl_clean_LUT8b_handle(&klh);
        return -1;
    }

    // 清理原Handle
    krl_clean_LUT8b_handle(&klh);
    klh = NULL;

    // 从文件重新加载
    ret = load_lut8_handle(filename, &klh);
    if (ret != 0) {
        return -1;
    }

    // 验证加载的数据
    size_t* loaded_idx = krl_get_idx_pointer(klh);
    printf("验证加载的数据:\n");
    for (size_t i = 0; i < 5; i++) {
        printf("  idx[%zu] = %zu\n", i, loaded_idx[i]);
    }

    // 清理
    krl_clean_LUT8b_handle(&klh);
    
    return 0;
}
```

### krl\_build\_LUT8Handle\_fromfile

**接口定义<a name="section172317194488"></a>**

int krl\_build\_LUT8Handle\_fromfile\(FILE\* f, KRLLUT8bHandle\*\* klh\);

**接口用途<a name="section1153124784912"></a>**

从文件中读取并重建8bit查找表句柄。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.541554155415543%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.611461146114612%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p14381721205612"><a name="p14381721205612"></a><a name="p14381721205612"></a>f</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p7438122115569"><a name="p7438122115569"></a><a name="p7438122115569"></a>FILE*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p6717120145712"><a name="p6717120145712"></a><a name="p6717120145712"></a>读取的文件句柄。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p4187123185620"><a name="p4187123185620"></a><a name="p4187123185620"></a>限制非空。</p>
</td>
</tr>
<tr id="row587315210197"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p14873021151914"><a name="p14873021151914"></a><a name="p14873021151914"></a>klh</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p887382119197"><a name="p887382119197"></a><a name="p887382119197"></a>KRLLUT8bHandle*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p287382118190"><a name="p287382118190"></a><a name="p287382118190"></a>KRLLUT8bHandle指针。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1487318214195"><a name="p1487318214195"></a><a name="p1487318214195"></a>限制非空。</p>
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
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a>正常运行时返回0，异常退出返回对应错误码。</p>
</td>
</tr>
</tbody>
</table>

**使用示例**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

// 保存Handle到文件
int save_lut8_handle(const char* filename, KRLLUT8bHandle* klh) {
    FILE* f = fopen(filename, "wb");
    if (f == NULL) {
        printf("无法打开文件进行写入: %s\n", filename);
        return -1;
    }

    int ret = krl_store_LUT8Handle(f, klh);
    fclose(f);

    if (ret == 0) {
        printf("LUT8bHandle已保存到: %s\n", filename);
    } else {
        printf("保存失败，错误码: %d\n", ret);
    }
    return ret;
}

// 从文件加载Handle
int load_lut8_handle(const char* filename, KRLLUT8bHandle** klh) {
    FILE* f = fopen(filename, "rb");
    if (f == NULL) {
        printf("无法打开文件进行读取: %s\n", filename);
        return -1;
    }

    int ret = krl_build_LUT8Handle_fromfile(f, klh);
    fclose(f);

    if (ret == 0) {
        printf("LUT8bHandle已从文件加载: %s\n", filename);
    } else {
        printf("加载失败，错误码: %d\n", ret);
    }
    return ret;
}

int main() {
    const char* filename = "lut8_handle.bin";
    
    // 创建并初始化Handle
    KRLLUT8bHandle* klh = NULL;
    int use_idx = 1;
    size_t capacity = 10000;
    
    int ret = krl_create_LUT8b_handle(&klh, use_idx, capacity);
    if (ret != 0) {
        printf("创建Handle失败\n");
        return -1;
    }

    // 设置一些数据
    size_t* idx_ptr = krl_get_idx_pointer(klh);
    for (size_t i = 0; i < 100; i++) {
        idx_ptr[i] = i * 10;
    }

    // 保存Handle
    ret = save_lut8_handle(filename, klh);
    if (ret != 0) {
        krl_clean_LUT8b_handle(&klh);
        return -1;
    }

    // 清理原Handle
    krl_clean_LUT8b_handle(&klh);
    klh = NULL;

    // 从文件重新加载
    ret = load_lut8_handle(filename, &klh);
    if (ret != 0) {
        return -1;
    }

    // 验证加载的数据
    size_t* loaded_idx = krl_get_idx_pointer(klh);
    printf("验证加载的数据:\n");
    for (size_t i = 0; i < 5; i++) {
        printf("  idx[%zu] = %zu\n", i, loaded_idx[i]);
    }

    // 清理
    krl_clean_LUT8b_handle(&klh);
    
    return 0;
}
```

### krl\_store\_distanceHandle

**接口定义<a name="section172317194488"></a>**

int krl\_store\_distanceHandle\(FILE\* f, const KRLDistanceHandle\* kdh\);

**接口用途<a name="section1153124784912"></a>**

将距离计算句柄保存到文件中。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.541554155415543%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.611461146114612%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p14381721205612"><a name="p14381721205612"></a><a name="p14381721205612"></a>f</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p7438122115569"><a name="p7438122115569"></a><a name="p7438122115569"></a>FILE*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p1018720320568"><a name="p1018720320568"></a><a name="p1018720320568"></a>写入的文件句柄。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p4187123185620"><a name="p4187123185620"></a><a name="p4187123185620"></a>限制非空。</p>
</td>
</tr>
<tr id="row587315210197"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p123371053104616"><a name="p123371053104616"></a><a name="p123371053104616"></a>kdh</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p9468096466"><a name="p9468096466"></a><a name="p9468096466"></a>const KRLDistanceHandle*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p287382118190"><a name="p287382118190"></a><a name="p287382118190"></a>KRLDistanceHandle指针。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1487318214195"><a name="p1487318214195"></a><a name="p1487318214195"></a>限制非空。</p>
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
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a>正常运行时返回0，异常退出返回对应错误码。</p>
</td>
</tr>
</tbody>
</table>

**使用示例**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

int main() {
    const char* filename = "distance_handle.bin";
    
    // 参数配置
    size_t dim = 128;
    size_t ny = 10000;
    int metric_type = 0;  // L2距离

    // 准备底库向量
    float* base_vectors = (float*)malloc(ny * dim * sizeof(float));
    for (size_t i = 0; i < ny * dim; i++) {
        base_vectors[i] = (float)(rand() % 1000) / 100.0f;
    }

    // 创建Handle
    KRLDistanceHandle* kdh = NULL;
    int ret = krl_create_distance_handle(
        &kdh, base_vectors, ny, dim, metric_type, ny * dim
    );
    if (ret != 0) {
        printf("创建DistanceHandle失败\n");
        free(base_vectors);
        return -1;
    }

    // 保存Handle到文件
    FILE* f_write = fopen(filename, "wb");
    if (f_write == NULL) {
        printf("无法打开文件进行写入\n");
        krl_clean_distance_handle(&kdh);
        free(base_vectors);
        return -1;
    }

    ret = krl_store_distanceHandle(f_write, kdh);
    fclose(f_write);
    
    if (ret != 0) {
        printf("保存DistanceHandle失败: %d\n", ret);
        krl_clean_distance_handle(&kdh);
        free(base_vectors);
        return -1;
    }
    printf("DistanceHandle已保存到: %s\n", filename);

    // 清理原Handle
    krl_clean_distance_handle(&kdh);
    kdh = NULL;

    // 从文件加载Handle
    FILE* f_read = fopen(filename, "rb");
    if (f_read == NULL) {
        printf("无法打开文件进行读取\n");
        free(base_vectors);
        return -1;
    }

    ret = krl_build_distanceHandle_fromfile(f_read, &kdh);
    fclose(f_read);

    if (ret != 0) {
        printf("加载DistanceHandle失败: %d\n", ret);
        free(base_vectors);
        return -1;
    }
    printf("DistanceHandle已从文件加载\n");

    // 使用加载的Handle进行距离计算
    float* query = (float*)malloc(dim * sizeof(float));
    for (size_t i = 0; i < dim; i++) {
        query[i] = (float)(rand() % 1000) / 100.0f;
    }

    float distance;
    ret = krl_L2sqr_with_handle(kdh, query, 0, &distance, dim);
    if (ret == 0) {
        printf("使用加载的Handle计算距离成功: %f\n", distance);
    }

    // 清理
    krl_clean_distance_handle(&kdh);
    free(base_vectors);
    free(query);

    return 0;
}
```

### krl\_build\_distanceHandle\_fromfile

**接口定义<a name="section172317194488"></a>**

int krl\_build\_distanceHandle\_fromfile\(FILE\* f, KRLDistanceHandle\*\* kdh\);

**接口用途<a name="section1153124784912"></a>**

从文件中读取并重建距离计算句柄。

**参数说明<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.541554155415543%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.611461146114612%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>取值范围</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p14381721205612"><a name="p14381721205612"></a><a name="p14381721205612"></a>f</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p7438122115569"><a name="p7438122115569"></a><a name="p7438122115569"></a>FILE*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p6717120145712"><a name="p6717120145712"></a><a name="p6717120145712"></a>读取的文件句柄。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p4187123185620"><a name="p4187123185620"></a><a name="p4187123185620"></a>限制非空。</p>
</td>
</tr>
<tr id="row587315210197"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p123371053104616"><a name="p123371053104616"></a><a name="p123371053104616"></a>kdh</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p9468096466"><a name="p9468096466"></a><a name="p9468096466"></a>const KRLDistanceHandle*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p287382118190"><a name="p287382118190"></a><a name="p287382118190"></a>KRLDistanceHandle指针。</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1487318214195"><a name="p1487318214195"></a><a name="p1487318214195"></a>限制非空。</p>
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
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a>正常运行时返回0，异常退出返回对应错误码。</p>
</td>
</tr>
</tbody>
</table>

## 错误码

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>错误码</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>0</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a>正常运行时返回0。</p>
</td>
</tr>
<tr id="row2932411194415"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p99338112449"><a name="p99338112449"></a><a name="p99338112449"></a>-1</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p8763115484411"><a name="p8763115484411"></a><a name="p8763115484411"></a>非法指针。</p>
</td>
</tr>
<tr id="row1410418141442"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p810461414413"><a name="p810461414413"></a><a name="p810461414413"></a>-2</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p7104191418447"><a name="p7104191418447"></a><a name="p7104191418447"></a>内存分配失败。</p>
</td>
</tr>
<tr id="row628451718442"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p2028411717447"><a name="p2028411717447"></a><a name="p2028411717447"></a>-3</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p728431784411"><a name="p728431784411"></a><a name="p728431784411"></a>非法入参。</p>
</td>
</tr>
<tr id="row3524122294419"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p20524162216440"><a name="p20524162216440"></a><a name="p20524162216440"></a>-4</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p18524122210449"><a name="p18524122210449"></a><a name="p18524122210449"></a>双重释放。</p>
</td>
</tr>
<tr id="row8864111915443"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p0864219184413"><a name="p0864219184413"></a><a name="p0864219184413"></a>-5</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p786412199445"><a name="p786412199445"></a><a name="p786412199445"></a>不安全内存操作。</p>
</td>
</tr>
<tr id="row114641147134412"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p746415479447"><a name="p746415479447"></a><a name="p746415479447"></a>-6</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p14640472441"><a name="p14640472441"></a><a name="p14640472441"></a>IO失败。</p>
</td>
</tr>
</tbody>
</table>

**使用示例**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

int main() {
    const char* filename = "distance_handle.bin";
    
    // 参数配置
    size_t dim = 128;
    size_t ny = 10000;
    int metric_type = 0;  // L2距离

    // 准备底库向量
    float* base_vectors = (float*)malloc(ny * dim * sizeof(float));
    for (size_t i = 0; i < ny * dim; i++) {
        base_vectors[i] = (float)(rand() % 1000) / 100.0f;
    }

    // 创建Handle
    KRLDistanceHandle* kdh = NULL;
    int ret = krl_create_distance_handle(
        &kdh, base_vectors, ny, dim, metric_type, ny * dim
    );
    if (ret != 0) {
        printf("创建DistanceHandle失败\n");
        free(base_vectors);
        return -1;
    }

    // 保存Handle到文件
    FILE* f_write = fopen(filename, "wb");
    if (f_write == NULL) {
        printf("无法打开文件进行写入\n");
        krl_clean_distance_handle(&kdh);
        free(base_vectors);
        return -1;
    }

    ret = krl_store_distanceHandle(f_write, kdh);
    fclose(f_write);
    
    if (ret != 0) {
        printf("保存DistanceHandle失败: %d\n", ret);
        krl_clean_distance_handle(&kdh);
        free(base_vectors);
        return -1;
    }
    printf("DistanceHandle已保存到: %s\n", filename);

    // 清理原Handle
    krl_clean_distance_handle(&kdh);
    kdh = NULL;

    // 从文件加载Handle
    FILE* f_read = fopen(filename, "rb");
    if (f_read == NULL) {
        printf("无法打开文件进行读取\n");
        free(base_vectors);
        return -1;
    }

    ret = krl_build_distanceHandle_fromfile(f_read, &kdh);
    fclose(f_read);

    if (ret != 0) {
        printf("加载DistanceHandle失败: %d\n", ret);
        free(base_vectors);
        return -1;
    }
    printf("DistanceHandle已从文件加载\n");

    // 使用加载的Handle进行距离计算
    float* query = (float*)malloc(dim * sizeof(float));
    for (size_t i = 0; i < dim; i++) {
        query[i] = (float)(rand() % 1000) / 100.0f;
    }

    float distance;
    ret = krl_L2sqr_with_handle(kdh, query, 0, &distance, dim);
    if (ret == 0) {
        printf("使用加载的Handle计算距离成功: %f\n", distance);
    }

    // 清理
    krl_clean_distance_handle(&kdh);
    free(base_vectors);
    free(query);

    return 0;
}
```
