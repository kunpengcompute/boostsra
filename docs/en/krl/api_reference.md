# API Reference

## APIs

[**Table 1** KRL interfaces](#krl-interfaces) describes the interfaces provided by KRL.

**Table 1** KRL interfaces<a id="krl-interfaces"></a>

<a name="table1194910128449"></a>
<table><thead align="left"><tr id="row99491812134412"><th class="cellrowborder" valign="top" width="13.059999999999999%" id="mcps1.2.4.1.1"><p id="p768563014173"><a name="p768563014173"></a><a name="p768563014173"></a>Type</p>
</th>
<th class="cellrowborder" valign="top" width="23.380000000000003%" id="mcps1.2.4.1.2"><p id="p1794951224415"><a name="p1794951224415"></a><a name="p1794951224415"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="63.56%" id="mcps1.2.4.1.3"><p id="p6949612124415"><a name="p6949612124415"></a><a name="p6949612124415"></a>Function</p>
</th>
</tr>
</thead>
<tbody><tr id="row712018285575"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p1468583012176"><a name="p1468583012176"></a><a name="p1468583012176"></a>Handle class interfaces</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p8993524101814"><a name="p8993524101814"></a><a name="p8993524101814"></a>krl_create_distance_handle</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p14993924101811"><a name="p14993924101811"></a><a name="p14993924101811"></a>Initializes and constructs a KRLDistanceHandle instance for dense distance computation.</p>
</td>
</tr>
<tr id="row119491112174414"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p163141052196"><a name="p163141052196"></a><a name="p163141052196"></a>Handle class interfaces</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p175854912238"><a name="p175854912238"></a><a name="p175854912238"></a>krl_create_reorder_handle</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p09931024131816"><a name="p09931024131816"></a><a name="p09931024131816"></a>Initializes and constructs a KRLDistanceHandle instance for reranking computation.</p>
</td>
</tr>
<tr id="row9949131219443"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p831619512197"><a name="p831619512197"></a><a name="p831619512197"></a>Handle class interfaces</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p19936249184"><a name="p19936249184"></a><a name="p19936249184"></a>krl_clean_distance_handle</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p7729162612418"><a name="p7729162612418"></a><a name="p7729162612418"></a>Destroys the KRLDistanceHandle instance and releases memory space.</p>
</td>
</tr>
<tr id="row1594913120443"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p16317151193"><a name="p16317151193"></a><a name="p16317151193"></a>Handle class interfaces</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p799319246182"><a name="p799319246182"></a><a name="p799319246182"></a>krl_create_LUT8b_handle</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p7993122417187"><a name="p7993122417187"></a><a name="p7993122417187"></a>Initializes and constructs a KRLLUT8bHandle instance for accumulation based on 8-bit table lookup.</p>
</td>
</tr>
<tr id="row6949131274416"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p13180551910"><a name="p13180551910"></a><a name="p13180551910"></a>Handle class interfaces</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p12993324191819"><a name="p12993324191819"></a><a name="p12993324191819"></a>krl_clean_LUT8b_handle</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p139801643145818"><a name="p139801643145818"></a><a name="p139801643145818"></a>Destroys the KRLLUT8bHandle instance and releases memory space.</p>
</td>
</tr>
<tr id="row13975184141820"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p531917514195"><a name="p531917514195"></a><a name="p531917514195"></a>Handle class interfaces</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p7975114191820"><a name="p7975114191820"></a><a name="p7975114191820"></a>krl_get_idx_pointer</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p192601719115616"><a name="p192601719115616"></a><a name="p192601719115616"></a>Obtains the IDs of to-be-computed base vectors stored in the KRLLUT8bHandle instance.</p>
</td>
</tr>
<tr id="row1682414614182"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p183211558190"><a name="p183211558190"></a><a name="p183211558190"></a>Handle class interfaces</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p621722142419"><a name="p621722142419"></a><a name="p621722142419"></a>krl_get_dist_pointer</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p2824164621814"><a name="p2824164621814"></a><a name="p2824164621814"></a>Obtains the start address of the distance array stored in the KRLLUT8bHandle instance. The address contains a random number before a table lookup-based accumulation operator is called, and holds the computed distance value after the operator is called.</p>
</td>
</tr>
<tr id="row891194810189"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p6685230201716"><a name="p6685230201716"></a><a name="p6685230201716"></a>Distance computation interfaces</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p12911154891819"><a name="p12911154891819"></a><a name="p12911154891819"></a>krl_L2sqr</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p5911184810186"><a name="p5911184810186"></a><a name="p5911184810186"></a>Performs one-to-one Euclidean distance computation on vectors represented in float precision.</p>
</td>
</tr>
<tr id="row1710165116183"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p120601371911"><a name="p120601371911"></a><a name="p120601371911"></a>Distance Computation Interfaces</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p710165111184"><a name="p710165111184"></a><a name="p710165111184"></a>krl_L2sqr_f16f32</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p1693388205916"><a name="p1693388205916"></a><a name="p1693388205916"></a>Performs one-to-one Euclidean distance computation on vectors represented in fp16 precision.</p>
</td>
</tr>
<tr id="row490119533188"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p14208191316192"><a name="p14208191316192"></a><a name="p14208191316192"></a>Distance computation interfaces</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p179011053151819"><a name="p179011053151819"></a><a name="p179011053151819"></a>krl_L2sqr_u8u32</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p790155315187"><a name="p790155315187"></a><a name="p790155315187"></a>Performs one-to-one Euclidean distance computation on vectors represented as 8-bit unsigned integers (uint8).</p>
</td>
</tr>
<tr id="row1785925518184"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p11209713131919"><a name="p11209713131919"></a><a name="p11209713131919"></a>Distance computation interfaces</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p4860165531811"><a name="p4860165531811"></a><a name="p4860165531811"></a>krl_ipdis</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p158609551186"><a name="p158609551186"></a><a name="p158609551186"></a>Performs one-to-one distance computation using inner product on vectors represented in float precision.</p>
</td>
</tr>
<tr id="row197613573181"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p321121341919"><a name="p321121341919"></a><a name="p321121341919"></a>Distance computation interfaces</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p5761135713185"><a name="p5761135713185"></a><a name="p5761135713185"></a>krl_negative_ipdis_f16f32</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p20381543012"><a name="p20381543012"></a><a name="p20381543012"></a>Performs one-to-one distance computation using inner product on vectors represented in fp16 precision.</p>
</td>
</tr>
<tr id="row2030213041919"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p521251381911"><a name="p521251381911"></a><a name="p521251381911"></a>Distance computation interfaces</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p15619557252"><a name="p15619557252"></a><a name="p15619557252"></a>krl_negative_ipdis_s8s32</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p17303140191918"><a name="p17303140191918"></a><a name="p17303140191918"></a>Performs one-to-one distance computation using inner product on vectors represented as 8-bit signed integers (int8).</p>
</td>
</tr>
<tr id="row238412241914"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p15213213161920"><a name="p15213213161920"></a><a name="p15213213161920"></a>Distance computation interfaces</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p1138418201911"><a name="p1138418201911"></a><a name="p1138418201911"></a>krl_L2sqr_by_idx</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p203841126192"><a name="p203841126192"></a><a name="p203841126192"></a>Performs one-to-many Euclidean distance computation on vectors represented in float precision.</p>
</td>
</tr>
<tr id="row0391358193"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p192142139194"><a name="p192142139194"></a><a name="p192142139194"></a>Distance computation interfaces</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p2725181712253"><a name="p2725181712253"></a><a name="p2725181712253"></a>krl_L2sqr_by_idx_f16f32</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p133913511915"><a name="p133913511915"></a><a name="p133913511915"></a>Performs one-to-many Euclidean distance computation on vectors represented in fp16 precision.</p>
</td>
</tr>
<tr id="row151611671195"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p12215201391920"><a name="p12215201391920"></a><a name="p12215201391920"></a>Distance computation interfaces</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p20161197101911"><a name="p20161197101911"></a><a name="p20161197101911"></a>krl_L2sqr_by_idx_u8f32</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p1616177151919"><a name="p1616177151919"></a><a name="p1616177151919"></a>Performs one-to-many Euclidean distance computation on vectors represented as 8-bit unsigned integers (uint8).</p>
</td>
</tr>
<tr id="row5354120161911"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p321691321913"><a name="p321691321913"></a><a name="p321691321913"></a>Distance computation interfaces</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p0354420111913"><a name="p0354420111913"></a><a name="p0354420111913"></a>krl_inner_product_by_idx</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p2354132010196"><a name="p2354132010196"></a><a name="p2354132010196"></a>Performs one-to-many distance computation using inner product on vectors represented in float precision.</p>
</td>
</tr>
<tr id="row1423643420194"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p221741341915"><a name="p221741341915"></a><a name="p221741341915"></a>Distance computation interfaces</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p5233173872520"><a name="p5233173872520"></a><a name="p5233173872520"></a>krl_inner_product_by_idx_f16f32</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p2354132010196"><a name="p2354132010196"></a><a name="p2354132010196"></a>Performs one-to-many distance computation using inner product on vectors represented in fp16 precision.</p>
</td>
</tr>
<tr id="row1792738101914"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p10218111381917"><a name="p10218111381917"></a><a name="p10218111381917"></a>Distance computation interfaces</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p18810342182514"><a name="p18810342182514"></a><a name="p18810342182514"></a>krl_negative_inner_product_by_idx_f16f32</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p27921838121916"><a name="p27921838121916"></a><a name="p27921838121916"></a>Performs one-to-many distance computation using inner product on vectors represented in fp16 precision, and negates the computation results.</p>
</td>
</tr>
<tr id="row7651940121918"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p32191513101918"><a name="p32191513101918"></a><a name="p32191513101918"></a>Distance computation interfaces</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p186516406195"><a name="p186516406195"></a><a name="p186516406195"></a>krl_inner_product_by_idx_s8f32</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p196511640121916"><a name="p196511640121916"></a><a name="p196511640121916"></a>Performs one-to-many distance computation using inner product on vectors represented as 8-bit signed integers (int8).</p>
</td>
</tr>
<tr id="row283274219196"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p822001319194"><a name="p822001319194"></a><a name="p822001319194"></a>Distance computation interfaces</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p383264213197"><a name="p383264213197"></a><a name="p383264213197"></a>krl_L2sqr_ny</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p168329424199"><a name="p168329424199"></a><a name="p168329424199"></a>Performs one-to-many Euclidean distance computation on vectors represented in float precision.</p>
</td>
</tr>
<tr id="row47661344161914"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p1922131381913"><a name="p1922131381913"></a><a name="p1922131381913"></a>Distance computation interfaces</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p207661044101919"><a name="p207661044101919"></a><a name="p207661044101919"></a>krl_L2sqr_ny_f16f32</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p1176710447191"><a name="p1176710447191"></a><a name="p1176710447191"></a>Performs one-to-many Euclidean distance computation on vectors represented in fp16 precision.</p>
</td>
</tr>
<tr id="row0904184681920"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p112221813111918"><a name="p112221813111918"></a><a name="p112221813111918"></a>Distance computation interfaces</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p1090416468197"><a name="p1090416468197"></a><a name="p1090416468197"></a>krl_L2sqr_ny_u8f32</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p19047462196"><a name="p19047462196"></a><a name="p19047462196"></a>Performs one-to-many Euclidean distance computation on vectors represented as 8-bit unsigned integers (uint8).</p>
</td>
</tr>
<tr id="row1149011486191"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p222361351918"><a name="p222361351918"></a><a name="p222361351918"></a>Distance computation interfaces</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p9490144814199"><a name="p9490144814199"></a><a name="p9490144814199"></a>krl_L2sqr_ny_with_handle</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p64901848191916"><a name="p64901848191916"></a><a name="p64901848191916"></a>Performs one-to-many Euclidean distance computation on vectors represented in float precision. The base vectors and dimensions are stored in the handle.</p>
</td>
</tr>
<tr id="row221135114193"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p15224131313192"><a name="p15224131313192"></a><a name="p15224131313192"></a>Distance computation interfaces</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p13221351171919"><a name="p13221351171919"></a><a name="p13221351171919"></a>krl_inner_product_ny</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p1022851141912"><a name="p1022851141912"></a><a name="p1022851141912"></a>Performs one-to-many distance computation using inner product on vectors represented in float precision.</p>
</td>
</tr>
<tr id="row1670318531197"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p022551361914"><a name="p022551361914"></a><a name="p022551361914"></a>Distance computation interfaces</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p370305310196"><a name="p370305310196"></a><a name="p370305310196"></a>krl_inner_product_ny_f16f32</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p1570335316191"><a name="p1570335316191"></a><a name="p1570335316191"></a>Performs one-to-many distance computation using inner product on vectors represented in fp16 precision.</p>
</td>
</tr>
<tr id="row1659115614196"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p222621316199"><a name="p222621316199"></a><a name="p222621316199"></a>Distance computation interfaces</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p05910561199"><a name="p05910561199"></a><a name="p05910561199"></a>krl_inner_product_ny_s8f32</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p135911256161914"><a name="p135911256161914"></a><a name="p135911256161914"></a>Performs one-to-many distance computation using inner product on vectors represented as 8-bit signed integers (int8).</p>
</td>
</tr>
<tr id="row86397594196"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p11227813101917"><a name="p11227813101917"></a><a name="p11227813101917"></a>Distance computation interfaces</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p2640125961913"><a name="p2640125961913"></a><a name="p2640125961913"></a>krl_inner_product_ny_with_handle</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p8640159201914"><a name="p8640159201914"></a><a name="p8640159201914"></a>Performs one-to-many distance computation using inner product on vectors represented in float precision. The base vectors and dimensions are stored in the handle.</p>
</td>
</tr>
<tr id="row166751616206"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p206851730131710"><a name="p206851730131710"></a><a name="p206851730131710"></a>8-bit table lookup-based accumulation interfaces</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p196762119202"><a name="p196762119202"></a><a name="p196762119202"></a>krl_table_lookup_8b_f32</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p126761515204"><a name="p126761515204"></a><a name="p126761515204"></a>Obtains distance values from the float-type LUT using 8-bit indexes, accumulates the distance values, adds <code>dis0</code> to the result after accumulation, and stores the final result in <code>distance</code>.</p>
</td>
</tr>
<tr id="row1380243132018"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p3506620151918"><a name="p3506620151918"></a><a name="p3506620151918"></a>8-bit table lookup-based accumulation interfaces</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p28034302020"><a name="p28034302020"></a><a name="p28034302020"></a>krl_table_lookup_8b_f32_by_idx</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p4803034206"><a name="p4803034206"></a><a name="p4803034206"></a>Obtains distance values from the float-type LUT using 8-bit indexes, accumulates the distance values, adds <code>dis0</code> to the result after accumulation, and stores the final result in <code>distance</code>. Only the base vectors whose IDs are in the <code>idx</code> array are used for computation.</p>
</td>
</tr>
<tr id="row13704145182016"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p45071220161916"><a name="p45071220161916"></a><a name="p45071220161916"></a>8-bit table lookup-based accumulation interfaces</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p270425132019"><a name="p270425132019"></a><a name="p270425132019"></a>krl_table_lookup_8b_f32_with_handle</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p27041512013"><a name="p27041512013"></a><a name="p27041512013"></a>Obtains distance values from the float-type LUT using 8-bit indexes, accumulates the distance values, adds <code>dis0</code> to the result after accumulation, and stores the final result in <code>distance</code>. The <code>idx</code> and <code>distance</code> arrays are contained in the KRLLUT8bHandle instance. Only the base vectors whose IDs are in the <code>idx</code> array are used for computation.</p>
</td>
</tr>
<tr id="row1040647122014"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p46851630141710"><a name="p46851630141710"></a><a name="p46851630141710"></a>4-bit table lookup-based accumulation interfaces</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p12407197202019"><a name="p12407197202019"></a><a name="p12407197202019"></a>krl_fast_table_lookup_step</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p040757182014"><a name="p040757182014"></a><a name="p040757182014"></a>An operator designed for 4-bit table lookup, accumulation, filtering, and compression. It is used for batch processing of float-type query vectors. This operator is used to compute distances between a maximum of 16 query vectors and 32 base vectors. After the distance computation, each result is compared against a threshold. If a distance value is less than the threshold, the bit in <code>lt_mask</code> of the corresponding base vector is set to <code>1</code>. Otherwise, it is set to <code>0</code>.</p>
</td>
</tr>
<tr id="row187412920207"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p1962812276198"><a name="p1962812276198"></a><a name="p1962812276198"></a>4-bit table lookup-based accumulation interfaces</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p1332135182717"><a name="p1332135182717"></a><a name="p1332135182717"></a>krl_L2_table_lookup_fast_scan_bs64</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p1974249132015"><a name="p1974249132015"></a><a name="p1974249132015"></a>An operator designed for 4-bit table lookup, accumulation, filtering, and compression. It is used for processing float-type query vectors individually. Computes Euclidean distances between a query vector and 64 base vectors. Based on the distance comparison rule, if a distance value meets the comparison rule, the bit in <code>lt_mask</code> of the corresponding base vector is set to <code>1</code>. Otherwise, it is set to <code>0</code>.</p>
</td>
</tr>
<tr id="row10185812122010"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p1630327101916"><a name="p1630327101916"></a><a name="p1630327101916"></a>4-bit table lookup-based accumulation interfaces</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p1618516126202"><a name="p1618516126202"></a><a name="p1618516126202"></a>krl_IP_table_lookup_fast_scan_bs64</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p2405162815416"><a name="p2405162815416"></a><a name="p2405162815416"></a>An operator designed for 4-bit table lookup, accumulation, filtering, and compression. It is used for processing float-type query vectors individually. It computes distances between a query vector and 64 base vectors using inner product. Based on the distance comparison rule, if a distance value meets the comparison rule, the bit in <code>lt_mask</code> of the corresponding base vector is set to <code>1</code>. Otherwise, it is set to <code>0</code>.</p>
</td>
</tr>
<tr id="row17962171310208"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p3631162715196"><a name="p3631162715196"></a><a name="p3631162715196"></a>4-bit table lookup-based accumulation interfaces</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p3585133102819"><a name="p3585133102819"></a><a name="p3585133102819"></a>krl_L2_table_lookup_fast_scan_bs96</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p18962121362013"><a name="p18962121362013"></a><a name="p18962121362013"></a>An operator designed for 4-bit table lookup, accumulation, filtering, and compression. It is used for processing float-type query vectors individually. It computes Euclidean distances between a query vector and 96 base vectors. Based on the distance comparison rule, if a distance value meets the comparison rule, the bit in <code>lt_mask</code> of the corresponding base vector is set to <code>1</code>. Otherwise, it is set to <code>0</code>.</p>
</td>
</tr>
<tr id="row39991716192015"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p56321127121916"><a name="p56321127121916"></a><a name="p56321127121916"></a>4-bit table lookup-based accumulation interfaces</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p1999916102012"><a name="p1999916102012"></a><a name="p1999916102012"></a>krl_IP_table_lookup_fast_scan_bs96</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p8999816192019"><a name="p8999816192019"></a><a name="p8999816192019"></a>An operator designed for 4-bit table lookup, accumulation, filtering, and compression. It is used for processing float-type query vectors individually. Computes distances between a query vector and 96 base vectors using inner product. Based on the distance comparison rule, if a distance value meets the comparison rule, the bit in <code>lt_mask</code> of the corresponding base vector is set to <code>1</code>. Otherwise, it is set to <code>0</code>.</p>
</td>
</tr>
<tr id="row879313188203"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p106331927191916"><a name="p106331927191916"></a><a name="p106331927191916"></a>4-bit table lookup-based accumulation interfaces</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p979311816203"><a name="p979311816203"></a><a name="p979311816203"></a>krl_table_lookup_4b_f16</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p1479391832015"><a name="p1479391832015"></a><a name="p1479391832015"></a>An operator designed for 4-bit table lookup, accumulation, filtering, and compression. It is used for processing fp16 query vectors individually. It computes distances between a query vector and multiple base vectors using inner product. The initial distance is <code>dis_f16</code>. This interface does not perform filtering or compression (that is, comparison with the threshold).</p>
</td>
</tr>
<tr id="row54279217209"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p136351727111911"><a name="p136351727111911"></a><a name="p136351727111911"></a>4-bit table lookup-based accumulation interfaces</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p1120132012282"><a name="p1120132012282"></a><a name="p1120132012282"></a>krl_pack_codes_4b</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p16427162162010"><a name="p16427162162010"></a><a name="p16427162162010"></a>An operator designed for 4-bit table lookup, accumulation, filtering, and compression. It is used for processing fp16 query vectors individually. It computes distances between a query vector and multiple base vectors using inner product. The initial distance is <code>dis_f16</code>. This interface does not perform filtering or compression (that is, comparison with the threshold).</p>
</td>
</tr>
<tr id="row2013422482018"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p18685113014176"><a name="p18685113014176"></a><a name="p18685113014176"></a>Reranking interfaces</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p5134202413207"><a name="p5134202413207"></a><a name="p5134202413207"></a>krl_reorder_2_vector</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p6358251857"><a name="p6358251857"></a><a name="p6358251857"></a>Computes high-accuracy distances between a single query vector and multiple non-contiguous base vectors, and returns the results sorted by distance.</p>
</td>
</tr>
<tr id="row071714259208"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p1177182991910"><a name="p1177182991910"></a><a name="p1177182991910"></a>Reranking interfaces</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p671762518203"><a name="p671762518203"></a><a name="p671762518203"></a>krl_reorder_2_vector_continuous</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p157171825162016"><a name="p157171825162016"></a><a name="p157171825162016"></a>Computes high-accuracy distances between a single query vector and multiple contiguous base vectors, and returns the results sorted by distance.</p>
</td>
</tr>
<tr id="row101930282204"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p17685630131711"><a name="p17685630131711"></a><a name="p17685630131711"></a>Store/Load interfaces</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p619382822013"><a name="p619382822013"></a><a name="p619382822013"></a>krl_store_LUT8Handle</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p15193228102018"><a name="p15193228102018"></a><a name="p15193228102018"></a>Stores the handle of an 8-bit lookup table into a file.</p>
</td>
</tr>
<tr id="row418063172011"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p188531538101912"><a name="p188531538101912"></a><a name="p188531538101912"></a>Store/Load interfaces</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p4180133110202"><a name="p4180133110202"></a><a name="p4180133110202"></a>krl_build_LUT8Handle_fromfile</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p157004230511"><a name="p157004230511"></a><a name="p157004230511"></a>Reads data of an 8-bit lookup table from a file and rebuilds a handle.</p>
</td>
</tr>
<tr id="row4520183315206"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p385513812191"><a name="p385513812191"></a><a name="p385513812191"></a>Store/Load interfaces</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p11520103311205"><a name="p11520103311205"></a><a name="p11520103311205"></a>krl_store_distanceHandle</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p952053342012"><a name="p952053342012"></a><a name="p952053342012"></a>Stores the handle for distance computation into a file.</p>
</td>
</tr>
<tr id="row514503519205"><td class="cellrowborder" valign="top" width="13.059999999999999%" headers="mcps1.2.4.1.1 "><p id="p2856173821913"><a name="p2856173821913"></a><a name="p2856173821913"></a>Store/Load interfaces</p>
</td>
<td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.2.4.1.2 "><p id="p3146835102018"><a name="p3146835102018"></a><a name="p3146835102018"></a>krl_build_distanceHandle_fromfile</p>
</td>
<td class="cellrowborder" valign="top" width="63.56%" headers="mcps1.2.4.1.3 "><p id="p144261417573"><a name="p144261417573"></a><a name="p144261417573"></a>Reads data of a distance computation handle from a file and rebuilds the handle.</p>
</td>
</tr>
</tbody>
</table>

## Handle Class Interfaces

### krl\_create\_distance\_handle

**Interface Definition <a name="section172317194488"></a>**

int krl\_create\_distance\_handle\(KRLDistanceHandle\*\* kdh, size\_t accu\_level, size\_t blocksize, size\_t codes\_num, size\_t dim, size\_t num\_base, int metric\_type, const uint8\_t\* codes, size\_t codes\_size\);

**Function<a name="section1153124784912"></a>**

Initializes and constructs a KRLDistanceHandle instance for dense distance computation.

**Parameters<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.56155615561556%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="14.591459145914593%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>kdh</p>
</td>
<td class="cellrowborder" valign="top" width="14.591459145914593%" headers="mcps1.1.5.1.2 "><p id="p98931015893"><a name="p98931015893"></a><a name="p98931015893"></a>KRLDistanceHandle**</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p182303331508"><a name="p182303331508"></a><a name="p182303331508"></a>Pointer to the KRLDistanceHandle instance to be initialized.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>It cannot be null and should point to a null pointer.</p>
</td>
</tr>
<tr id="row11230173385019"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p22301333165015"><a name="p22301333165015"></a><a name="p22301333165015"></a>accu_level</p>
</td>
<td class="cellrowborder" valign="top" width="14.591459145914593%" headers="mcps1.1.5.1.2 "><p id="p5893141517919"><a name="p5893141517919"></a><a name="p5893141517919"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p10230433115013"><a name="p10230433115013"></a><a name="p10230433115013"></a>Quantization level during computation.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p77289581198"><a name="p77289581198"></a><a name="p77289581198"></a>[1, 3]</p>
<a name="ul164886121012"></a><a name="ul164886121012"></a><ul id="ul164886121012"><li><code>1</code>: int8 </li><li><code>2</code>: fp16 </li><li><code>3</code>: fp32</li></ul>
</td>
</tr>
<tr id="row1368063274610"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p116802032174613"><a name="p116802032174613"></a><a name="p116802032174613"></a>blocksize</p>
</td>
<td class="cellrowborder" valign="top" width="14.591459145914593%" headers="mcps1.1.5.1.2 "><p id="p489312151893"><a name="p489312151893"></a><a name="p489312151893"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p268013224617"><a name="p268013224617"></a><a name="p268013224617"></a>Data block size.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p6989158192510"><a name="p6989158192510"></a><a name="p6989158192510"></a>16, 32, or 64. Select the largest value that exactly divides the total number of base vectors.</p>
</td>
</tr>
<tr id="row8597534164617"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p4597734184616"><a name="p4597734184616"></a><a name="p4597734184616"></a>codes_num</p>
</td>
<td class="cellrowborder" valign="top" width="14.591459145914593%" headers="mcps1.1.5.1.2 "><p id="p178931015394"><a name="p178931015394"></a><a name="p178931015394"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p65975343465"><a name="p65975343465"></a><a name="p65975343465"></a>Number of base vectors computed for each query vector.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p16989883251"><a name="p16989883251"></a><a name="p16989883251"></a>[1, 2^30-1]</p>
</td>
</tr>
<tr id="row523013315504"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p10230123316509"><a name="p10230123316509"></a><a name="p10230123316509"></a>dim</p>
</td>
<td class="cellrowborder" valign="top" width="14.591459145914593%" headers="mcps1.1.5.1.2 "><p id="p2894215596"><a name="p2894215596"></a><a name="p2894215596"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p102301133105015"><a name="p102301133105015"></a><a name="p102301133105015"></a>Vector dimension.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p296864410116"><a name="p296864410116"></a><a name="p296864410116"></a>[1, 65535]</p>
</td>
</tr>
<tr id="row1523083315012"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p10230433105020"><a name="p10230433105020"></a><a name="p10230433105020"></a>num_base</p>
</td>
<td class="cellrowborder" valign="top" width="14.591459145914593%" headers="mcps1.1.5.1.2 "><p id="p15894141519917"><a name="p15894141519917"></a><a name="p15894141519917"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p623053365015"><a name="p623053365015"></a><a name="p623053365015"></a>Number of vectors processed in a batch.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1946832961016"><a name="p1946832961016"></a><a name="p1946832961016"></a>[1, 65535]</p>
</td>
</tr>
<tr id="row387211011106"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p2023791201011"><a name="p2023791201011"></a><a name="p2023791201011"></a>metric_type</p>
</td>
<td class="cellrowborder" valign="top" width="14.591459145914593%" headers="mcps1.1.5.1.2 "><p id="p198722006101"><a name="p198722006101"></a><a name="p198722006101"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p10237212111013"><a name="p10237212111013"></a><a name="p10237212111013"></a>Distance measurement type.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p5904125914109"><a name="p5904125914109"></a><a name="p5904125914109"></a>[0, 1]</p>
<a name="ul396901541013"></a><a name="ul396901541013"></a><ul id="ul396901541013"><li><code>0</code>: inner product distance </li><li><code>1</code>: Euclidean distance</li></ul>
</td>
</tr>
<tr id="row7131153011107"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p1546185591017"><a name="p1546185591017"></a><a name="p1546185591017"></a>codes</p>
</td>
<td class="cellrowborder" valign="top" width="14.591459145914593%" headers="mcps1.1.5.1.2 "><p id="p19131103031011"><a name="p19131103031011"></a><a name="p19131103031011"></a>const uint8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p55461255161011"><a name="p55461255161011"></a><a name="p55461255161011"></a>Base vectors (float).</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p213293001016"><a name="p213293001016"></a><a name="p213293001016"></a>The size is specified by <code>codes_size</code>.</p>
</td>
</tr>
<tr id="row1351603315418"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p1151717330417"><a name="p1151717330417"></a><a name="p1151717330417"></a>codes_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.591459145914593%" headers="mcps1.1.5.1.2 "><p id="p351703319417"><a name="p351703319417"></a><a name="p351703319417"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p6517433144111"><a name="p6517433144111"></a><a name="p6517433144111"></a>Length of base vectors.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p135171733184112"><a name="p135171733184112"></a><a name="p135171733184112"></a><code>codes_num</code> x <code>dim</code> x 4</p>
</td>
</tr>
</tbody>
</table>

**Return Values<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a><code>0</code> is returned on successful execution. In case of failure, an error code is returned to indicate the specific issue.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c
#include <stdio.h>
#include <stdlib.h>
#include <string.h>
#include "krl.h"

int main() {
    // Parameter configuration
    size_t dim = 128;           // Vector dimension
    size_t num_base = 1;        // Number of query vectors processed in a single batch
    size_t codes_num = 1000;    // Number of base vectors
    size_t accu_level = 3;      // Quantization level
    size_t blocksize = 32;      // Data block size (<code>codes_num</code> must be divisible by the data block size)
    int metric_type = 1;        // Euclidean distance

    // Base vector data preparation
    size_t codes_size = num_base * codes_num * dim * sizeof(float);
    float* codes_data = (float*)malloc(codes_size);
    //... Populate codes_data ...

    // Handle creation
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
        printf("Failed to create the handle. Error code: %d\n", ret);
        free(codes_data);
        return -1;
    }

    printf("KRLDistanceHandle created successfully.\n");

    //... Use kdh to compute the distance ...

    // Resources cleanup
    krl_clean_distance_handle(&kdh);
    free(codes_data);

    return 0;
}
```

### krl\_create\_reorder\_handle

**Interface Definition<a name="section172317194488"></a>**

int krl\_create\_reorder\_handle\(KRLDistanceHandle\*\* kdh, size\_t accu\_level, size\_t full\_accu\_level, size\_t codes\_num, size\_t dim, int metric\_type, const uint8\_t\* codes, size\_t codes\_size\);

**Function<a name="section1153124784912"></a>**

Initializes and constructs a KRLDistanceHandle instance for reranking computation.

**Parameters<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.56155615561556%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="14.591459145914593%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="30.29302930293029%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="39.55395539553955%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>kdh</p>
</td>
<td class="cellrowborder" valign="top" width="14.591459145914593%" headers="mcps1.1.5.1.2 "><p id="p98931015893"><a name="p98931015893"></a><a name="p98931015893"></a>KRLDistanceHandle**</p>
</td>
<td class="cellrowborder" valign="top" width="30.29302930293029%" headers="mcps1.1.5.1.3 "><p id="p182303331508"><a name="p182303331508"></a><a name="p182303331508"></a>Pointer to the KRLDistanceHandle instance to be initialized.</p>
</td>
<td class="cellrowborder" valign="top" width="39.55395539553955%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>It cannot be null and should point to a null pointer.</p>
</td>
</tr>
<tr id="row11230173385019"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p22301333165015"><a name="p22301333165015"></a><a name="p22301333165015"></a>accu_level</p>
</td>
<td class="cellrowborder" valign="top" width="14.591459145914593%" headers="mcps1.1.5.1.2 "><p id="p5893141517919"><a name="p5893141517919"></a><a name="p5893141517919"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="30.29302930293029%" headers="mcps1.1.5.1.3 "><p id="p10230433115013"><a name="p10230433115013"></a><a name="p10230433115013"></a>Quantization level in low-accuracy coarse ranking.</p>
</td>
<td class="cellrowborder" valign="top" width="39.55395539553955%" headers="mcps1.1.5.1.4 "><p id="p77289581198"><a name="p77289581198"></a><a name="p77289581198"></a>[1, 3]</p>
<a name="ul164886121012"></a><a name="ul164886121012"></a><ul id="ul164886121012"><li><code>1</code>: int8 </li><li><code>2</code>: fp16 </li><li><code>3</code>: fp32</li></ul>
</td>
</tr>
<tr id="row1368063274610"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p116802032174613"><a name="p116802032174613"></a><a name="p116802032174613"></a>full_accu_level</p>
</td>
<td class="cellrowborder" valign="top" width="14.591459145914593%" headers="mcps1.1.5.1.2 "><p id="p489312151893"><a name="p489312151893"></a><a name="p489312151893"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="30.29302930293029%" headers="mcps1.1.5.1.3 "><p id="p268013224617"><a name="p268013224617"></a><a name="p268013224617"></a>Quantization level in high-accuracy reranking.</p>
</td>
<td class="cellrowborder" valign="top" width="39.55395539553955%" headers="mcps1.1.5.1.4 "><p id="p11884449121914"><a name="p11884449121914"></a><a name="p11884449121914"></a>[1, 3]</p>
<a name="ul1588418498192"></a><a name="ul1588418498192"></a><ul id="ul1588418498192"><li><code>1</code>: int8 </li><li><code>2</code>: fp16 </li><li><code>3</code>: fp32</li></ul>
</td>
</tr>
<tr id="row8597534164617"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p4597734184616"><a name="p4597734184616"></a><a name="p4597734184616"></a>codes_num</p>
</td>
<td class="cellrowborder" valign="top" width="14.591459145914593%" headers="mcps1.1.5.1.2 "><p id="p178931015394"><a name="p178931015394"></a><a name="p178931015394"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="30.29302930293029%" headers="mcps1.1.5.1.3 "><p id="p65975343465"><a name="p65975343465"></a><a name="p65975343465"></a>Number of base vectors computed for each query vector.</p>
</td>
<td class="cellrowborder" valign="top" width="39.55395539553955%" headers="mcps1.1.5.1.4 "><p id="p16989883251"><a name="p16989883251"></a><a name="p16989883251"></a>[1, 2^30-1]</p>
</td>
</tr>
<tr id="row523013315504"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p10230123316509"><a name="p10230123316509"></a><a name="p10230123316509"></a>dim</p>
</td>
<td class="cellrowborder" valign="top" width="14.591459145914593%" headers="mcps1.1.5.1.2 "><p id="p2894215596"><a name="p2894215596"></a><a name="p2894215596"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="30.29302930293029%" headers="mcps1.1.5.1.3 "><p id="p102301133105015"><a name="p102301133105015"></a><a name="p102301133105015"></a>Vector dimension.</p>
</td>
<td class="cellrowborder" valign="top" width="39.55395539553955%" headers="mcps1.1.5.1.4 "><p id="p296864410116"><a name="p296864410116"></a><a name="p296864410116"></a>[1, 65535]</p>
</td>
</tr>
<tr id="row387211011106"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p2023791201011"><a name="p2023791201011"></a><a name="p2023791201011"></a>metric_type</p>
</td>
<td class="cellrowborder" valign="top" width="14.591459145914593%" headers="mcps1.1.5.1.2 "><p id="p198722006101"><a name="p198722006101"></a><a name="p198722006101"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="30.29302930293029%" headers="mcps1.1.5.1.3 "><p id="p10237212111013"><a name="p10237212111013"></a><a name="p10237212111013"></a>Distance measurement type.</p>
</td>
<td class="cellrowborder" valign="top" width="39.55395539553955%" headers="mcps1.1.5.1.4 "><p id="p5904125914109"><a name="p5904125914109"></a><a name="p5904125914109"></a>[0, 1]</p>
<a name="ul396901541013"></a><a name="ul396901541013"></a><ul id="ul396901541013"><li><code>0</code>: inner product distance </li><li><code>1</code>: Euclidean distance</li></ul>
</td>
</tr>
<tr id="row7131153011107"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p1546185591017"><a name="p1546185591017"></a><a name="p1546185591017"></a>codes</p>
</td>
<td class="cellrowborder" valign="top" width="14.591459145914593%" headers="mcps1.1.5.1.2 "><p id="p19131103031011"><a name="p19131103031011"></a><a name="p19131103031011"></a>const uint8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="30.29302930293029%" headers="mcps1.1.5.1.3 "><p id="p55461255161011"><a name="p55461255161011"></a><a name="p55461255161011"></a>Base vectors (float).</p>
</td>
<td class="cellrowborder" valign="top" width="39.55395539553955%" headers="mcps1.1.5.1.4 "><p id="p213293001016"><a name="p213293001016"></a><a name="p213293001016"></a>The size is specified by <code>codes_size</code>.</p>
</td>
</tr>
<tr id="row104562557484"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p1151717330417"><a name="p1151717330417"></a><a name="p1151717330417"></a>codes_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.591459145914593%" headers="mcps1.1.5.1.2 "><p id="p351703319417"><a name="p351703319417"></a><a name="p351703319417"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="30.29302930293029%" headers="mcps1.1.5.1.3 "><p id="p6517433144111"><a name="p6517433144111"></a><a name="p6517433144111"></a>Length of base vectors.</p>
</td>
<td class="cellrowborder" valign="top" width="39.55395539553955%" headers="mcps1.1.5.1.4 "><p id="p135171733184112"><a name="p135171733184112"></a><a name="p135171733184112"></a><code>codes_num</code> x <code>dim</code> x 4</p>
</td>
</tr>
</tbody>
</table>

**Return Values<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a><code>0</code> is returned on successful execution. In case of failure, an error code is returned to indicate the specific issue.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

int main() {
    // Parameter configuration
    size_t dim = 128;           // Vector dimension
    size_t codes_num = 100;         // Number of candidate vectors for reranking
    size_t accu_level = 1;          // int8 for coarse ranking
    size_t full_accu_level = 3;     // fp32 for reranking
    int metric_type = 1;            // Euclidean distance

    // Base vector data preparation
    size_t codes_size = codes_num * dim * sizeof(float);
    float* codes_data = (float*)malloc(codes_size);
    //... Populate codes_data ...

    // Reranking handle creation
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
        printf("Failed to create the reranking handle. Error code: %d\n", ret);
        free(codes_data);
        return -1;
    }

    printf("KRLDistanceHandle created successfully.\n");

    //... Use kdh to perform reranking computation...

    // Resources cleanup
    krl_clean_distance_handle(&kdh);
    free(codes_data);

    return 0;
}
```

### krl\_clean\_distance\_handle

**Interface Definition<a name="section172317194488"></a>**

void krl\_clean\_distance\_handle\(KRLDistanceHandle\*\* kdh\);

**Function<a name="section1153124784912"></a>**

Destroys the KRLDistanceHandle instance and releases memory space.

**Parameters<a name="section157501312135019"></a>**

<a name="table1646711617442"></a>
<table><thead align="left"><tr id="row846751612442"><th class="cellrowborder" valign="top" width="21.349999999999998%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="28.82%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="22.98%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="26.85%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row146815169448"><td class="cellrowborder" valign="top" width="21.349999999999998%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>kdh</p>
</td>
<td class="cellrowborder" valign="top" width="28.82%" headers="mcps1.1.5.1.2 "><p id="p98931015893"><a name="p98931015893"></a><a name="p98931015893"></a>KRLDistanceHandle**</p>
</td>
<td class="cellrowborder" valign="top" width="22.98%" headers="mcps1.1.5.1.3 "><p id="p182303331508"><a name="p182303331508"></a><a name="p182303331508"></a>Pointer to the KRLDistanceHandle instance to be destroyed.</p>
</td>
<td class="cellrowborder" valign="top" width="26.85%" headers="mcps1.1.5.1.4 "><p id="p12182012132917"><a name="p12182012132917"></a><a name="p12182012132917"></a>Points to a pointer that should be initialized by krl_create_distance_handle.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c
#include <stdio.h>
#include "krl.h"

int main() {
    KRLDistanceHandle* kdh = NULL;
    
    // Prerequisite: handle creation
    size_t dim = 128;
    size_t codes_num = 1000;
    size_t codes_size = 1 * codes_num * dim * sizeof(float);
    float* codes_data = (float*)malloc(codes_size);
    // ... Populate with data ...

    int ret = krl_create_distance_handle(&kdh, 3, 32, codes_num, dim, 1, 1, 
                                          (const uint8_t*)codes_data, codes_size);
    if (ret != 0) {
        free(codes_data);
        return -1;
    }

    //... Use kdh to perform computation...

    // Handle cleanup
    krl_clean_distance_handle(&kdh);
    // In this case, the pointer to which kdh points has been set to NULL.

    free(codes_data);
    printf("Resource cleanup completed\n");

    return 0;
}
```

### krl\_create\_LUT8b\_handle

**Interface Definition<a name="section172317194488"></a>**

int krl\_create\_LUT8b\_handle\(KRLLUT8bHandle\*\* klh, int use\_idx, size\_t capacity\);

**Function<a name="section1153124784912"></a>**

Initializes and constructs a KRLLUT8bHandle instance for accumulation based on 8-bit table lookup.

**Parameters<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.56155615561556%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="14.591459145914593%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="33.96339633963397%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="35.88358835883588%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>klh</p>
</td>
<td class="cellrowborder" valign="top" width="14.591459145914593%" headers="mcps1.1.5.1.2 "><p id="p98931015893"><a name="p98931015893"></a><a name="p98931015893"></a>KRLLUT8bHandle**</p>
</td>
<td class="cellrowborder" valign="top" width="33.96339633963397%" headers="mcps1.1.5.1.3 "><p id="p182303331508"><a name="p182303331508"></a><a name="p182303331508"></a>Pointer to the KRLLUT8bHandle instance to be initialized.</p>
</td>
<td class="cellrowborder" valign="top" width="35.88358835883588%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>It cannot be null and should point to a null pointer.</p>
</td>
</tr>
<tr id="row11230173385019"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p22301333165015"><a name="p22301333165015"></a><a name="p22301333165015"></a>use_idx</p>
</td>
<td class="cellrowborder" valign="top" width="14.591459145914593%" headers="mcps1.1.5.1.2 "><p id="p5893141517919"><a name="p5893141517919"></a><a name="p5893141517919"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="33.96339633963397%" headers="mcps1.1.5.1.3 "><p id="p10230433115013"><a name="p10230433115013"></a><a name="p10230433115013"></a>Indicates whether to filter base vectors.</p>
</td>
<td class="cellrowborder" valign="top" width="35.88358835883588%" headers="mcps1.1.5.1.4 "><p id="p77289581198"><a name="p77289581198"></a><a name="p77289581198"></a>[0, 1]</p>
<a name="ul164886121012"></a><a name="ul164886121012"></a><ul id="ul164886121012"><li><code>0</code>: filtering disabled </li><li><code>1</code>: filtering enabled</li></ul>
</td>
</tr>
<tr id="row1368063274610"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p10579191284217"><a name="p10579191284217"></a><a name="p10579191284217"></a>capacity</p>
</td>
<td class="cellrowborder" valign="top" width="14.591459145914593%" headers="mcps1.1.5.1.2 "><p id="p489312151893"><a name="p489312151893"></a><a name="p489312151893"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.96339633963397%" headers="mcps1.1.5.1.3 "><p id="p268013224617"><a name="p268013224617"></a><a name="p268013224617"></a>Handle class capacity, which is the maximum possible size of distance vectors and filtering vectors.</p>
</td>
<td class="cellrowborder" valign="top" width="35.88358835883588%" headers="mcps1.1.5.1.4 "><p id="p173108137452"><a name="p173108137452"></a><a name="p173108137452"></a>≥ 1. The value is ≥ <code>ncode</code> when krl_table_lookup_8b_f32_with_handle is called. <code>ncode</code> indicates the total number of base vectors.</p>
</td>
</tr>
</tbody>
</table>

**Return Values<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a><code>0</code> is returned on successful execution. In case of failure, an error code is returned to indicate the specific issue.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c
#include <stdio.h>
#include "krl.h"

int main() {
    // Parameter configuration
    int use_idx = 1; // Enable filtering of base vectors.
    size_t capacity = 10000; // A maximum of 10,000 base vectors are supported.

    // LUT8b handle creation
    KRLLUT8bHandle* klh = NULL;
    int ret = krl_create_LUT8b_handle(&klh, use_idx, capacity);

    if (ret != 0) {
        printf("Failed to create the LUT8b handle. Error code: %d\n", ret);
        return -1;
    }

    printf("KRLLUT8bHandle created successfully.\n");

    // Obtain a pointer to the index array (to set IDs of vectors to be computed).
    size_t* idx_ptr = krl_get_idx_pointer(klh);

    // Obtain a pointer to the distance array (to store the computation results).
    float* dist_ptr = krl_get_dist_pointer(klh);

    //... Use klh to perform accumulation based on table lookup ...

    // Resources cleanup
    krl_clean_LUT8b_handle(&klh);

    return 0;
}
```

### krl\_clean\_LUT8b\_handle

**Interface Definition<a name="section172317194488"></a>**

void krl\_clean\_LUT8b\_handle\(KRLLUT8bHandle\*\* klh\);

**Function<a name="section1153124784912"></a>**

Destroys the KRLLUT8bHandle instance and releases memory space.

**Parameters<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.56155615561556%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="14.591459145914593%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>klh</p>
</td>
<td class="cellrowborder" valign="top" width="14.591459145914593%" headers="mcps1.1.5.1.2 "><p id="p98931015893"><a name="p98931015893"></a><a name="p98931015893"></a>KRLLUT8bHandle**</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p182303331508"><a name="p182303331508"></a><a name="p182303331508"></a>Pointer to the KRLLUT8bHandle instance to be destroyed.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>The pointer pointed to by this parameter should be initialized by krl_create_LUT8b_handle.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c
#include <stdio.h>
#include "krl.h"

int main() {
    KRLLUT8bHandle* klh = NULL;

    // Prerequisite: handle creation
    int ret = krl_create_LUT8b_handle(&klh, 1, 10000);
    if (ret != 0) {
        return -1;
    }

    //... Use klh for computation ...

    // Handle cleanup
    krl_clean_LUT8b_handle(&klh);
    // In this case, the pointer to which klh points has been set to NULL.

    printf("KRLLUT8bHandle resources cleaned up.\n");

    return 0;
}
```

### krl\_get\_idx\_pointer

**Interface Definition<a name="section172317194488"></a>**

size\_t\* krl\_get\_idx\_pointer\(const KRLLUT8bHandle\* klh\);

**Function<a name="section1153124784912"></a>**

Obtains the IDs of to-be-computed base vectors stored in the KRLLUT8bHandle instance.

**Parameters<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.56155615561556%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="14.591459145914593%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>klh</p>
</td>
<td class="cellrowborder" valign="top" width="14.591459145914593%" headers="mcps1.1.5.1.2 "><p id="p98931015893"><a name="p98931015893"></a><a name="p98931015893"></a>KRLLUT8bHandle**</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p182303331508"><a name="p182303331508"></a><a name="p182303331508"></a>Pointer to the KRLLUT8bHandle instance.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>The value cannot be null.</p>
</td>
</tr>
</tbody>
</table>

**Return Values<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>size_t*</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p3457449204814"><a name="p3457449204814"></a><a name="p3457449204814"></a>IDs of to-be-computed base vectors stored in the KRLLUT8bHandle instance.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c
#include <stdio.h>
#include "krl.h"

int main() {
    KRLLUT8bHandle* klh = NULL;
    size_t capacity = 1000;

    // Prerequisite: handle creation
    int ret = krl_create_LUT8b_handle(&klh, 1, capacity);
    if (ret != 0) {
        return -1;
    }

    // Obtain a pointer to the index array.
    size_t* idx_ptr = krl_get_idx_pointer(klh);

    // Set IDs of base vectors to be used for distance computation.
    // For example, only compute distances for vectors with IDs 0, 5, 10, 15, and 20.
    size_t selected_count = 5;
    idx_ptr[0] = 0;
    idx_ptr[1] = 5;
    idx_ptr[2] = 10;
    idx_ptr[3] = 15;
    idx_ptr[4] = 20;

    printf(printf("%zu base vector IDs have been set for distance computation. \n", selected_count);

    //... Call table lookup-based accumulation interfaces for subsequent steps ...

    krl_clean_LUT8b_handle(&klh);

    return 0;
}
```

### krl\_get\_dist\_pointer

**Interface Definition<a name="section172317194488"></a>**

float\* krl\_get\_dist\_pointer\(const KRLLUT8bHandle\* klh\);

**Function<a name="section1153124784912"></a>**

Obtains the start address of the distance array stored in the KRLLUT8bHandle instance. The address contains a random number before a table lookup-based accumulation operator is called, and holds the computed distance value after the operator is called.

**Parameters<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.56155615561556%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="14.591459145914593%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.56155615561556%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>klh</p>
</td>
<td class="cellrowborder" valign="top" width="14.591459145914593%" headers="mcps1.1.5.1.2 "><p id="p98931015893"><a name="p98931015893"></a><a name="p98931015893"></a>KRLLUT8bHandle*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p182303331508"><a name="p182303331508"></a><a name="p182303331508"></a>Pointer to the KRLLUT8bHandle instance.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>The value cannot be null.</p>
</td>
</tr>
</tbody>
</table>

**Return Values<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>float*</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p3457449204814"><a name="p3457449204814"></a><a name="p3457449204814"></a>Start address of the distance array stored in the KRLLUT8bHandle instance. The address contains a random number before a table lookup-based accumulation operator is called, and holds the computed distance value after the operator is called.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c
#include <stdio.h>
#include "krl.h"

int main() {
    KRLLUT8bHandle* klh = NULL;
    size_t capacity = 1000;

    // Prerequisite: handle creation
    int ret = krl_create_LUT8b_handle(&klh, 0, capacity);
    if (ret != 0) {
        return -1;
    }

    // Obtain a pointer to the distance array.
    float* dist_ptr = krl_get_dist_pointer(klh);

    // Note: The value in dist_ptr is a random number.
    // A valid distance value is available only after the table lookup-based accumulation interface is called.

    //... Call table lookup-based accumulation interfaces ...

    // After the computation is complete, read the distance result.
    size_t num_results = 100;  // Assume that 100 vectors are used for distance computation.
    printf("First 5 distance results:\n");
    for (size_t i = 0; i < 5 && i < num_results; i++) {
        printf("  dist[%zu] = %f\n", i, dist_ptr[i]);
    }

    krl_clean_LUT8b_handle(&klh);

    return 0;
}
```

## Distance Computation Interfaces

### krl\_L2sqr

**Interface Definition<a name="section172317194488"></a>**

int krl\_L2sqr\(const float\* x, const float\* \_\_restrict y, const size\_t d, float\* dis, size\_t dis\_size\);

**Function<a name="section1153124784912"></a>**

Performs one-to-one Euclidean distance computation on vectors represented in float precision.

**Parameters<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="14.601460146014599%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p953215815518"><a name="p953215815518"></a><a name="p953215815518"></a>const float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p18661136253"><a name="p18661136253"></a><a name="p18661136253"></a>Query vector for distance computation.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>The vector has a dimension of <code>d</code>.</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4982142445414"><a name="p4982142445414"></a><a name="p4982142445414"></a>y</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7532158856"><a name="p7532158856"></a><a name="p7532158856"></a>const float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p36611261054"><a name="p36611261054"></a><a name="p36611261054"></a>Base vector for distance computation.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>The vector has a dimension of <code>d</code>.</p>
</td>
</tr>
<tr id="row106882715416"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p46812710547"><a name="p46812710547"></a><a name="p46812710547"></a>d</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p45311183519"><a name="p45311183519"></a><a name="p45311183519"></a>const size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p17661261256"><a name="p17661261256"></a><a name="p17661261256"></a>Vector dimension.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p46952755416"><a name="p46952755416"></a><a name="p46952755416"></a>[1, 65535]</p>
</td>
</tr>
<tr id="row2848154911529"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4849194916526"><a name="p4849194916526"></a><a name="p4849194916526"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p484916497520"><a name="p484916497520"></a><a name="p484916497520"></a>float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p184912496525"><a name="p184912496525"></a><a name="p184912496525"></a>Stores the distance computation result.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1984914498527"><a name="p1984914498527"></a><a name="p1984914498527"></a>The size is specified by <code>dis_size</code>. The memory needs to be allocated in advance.</p>
</td>
</tr>
<tr id="row13612117522"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p271521115212"><a name="p271521115212"></a><a name="p271521115212"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p10722125214"><a name="p10722125214"></a><a name="p10722125214"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p1762116529"><a name="p1762116529"></a><a name="p1762116529"></a>Size of the distance result array.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p17182165214"><a name="p17182165214"></a><a name="p17182165214"></a>The value is <code>1</code>.</p>
</td>
</tr>
</tbody>
</table>

**Return Values<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a><code>0</code> is returned on successful execution. In case of failure, an error code is returned to indicate the specific issue.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

int main() {
    size_t dim = 128;  // Vector dimension

    // Prepare the query vector and base vector.
    float* query_vec = (float*)malloc(dim * sizeof(float));
    float* base_vec = (float*)malloc(dim * sizeof(float));

    // Populate with the example data.
    for (size_t i = 0; i < dim; i++) {
        query_vec[i] = (float)i / dim;
        base_vec[i] = (float)(dim - i) / dim;
    }

    // Store the distance result.
    float distance = 0.0f;

    // Compute the Euclidean distance.
    int ret = krl_L2sqr(query_vec, base_vec, dim, &distance, 1);

    if (ret != 0) {
        printf("Distance computation failed. Error code: %d\n", ret);
        free(query_vec);
        free(base_vec);
        return -1;
    }

    printf("Euclidean distance (L2 squared): %f\n", distance);

    free(query_vec);
    free(base_vec);

    return 0;
}
```

### krl\_L2sqr\_f16f32

**Interface Definition<a name="section172317194488"></a>**

int krl\_L2sqr\_f16f32\(const uint16\_t\* x, const uint16\_t\* \_\_restrict y, size\_t d, float\* dis, size\_t dis\_size\);

**Function<a name="section1153124784912"></a>**

Performs one-to-one Euclidean distance computation on vectors represented in fp16 precision.

**Parameters<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="14.601460146014599%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p953215815518"><a name="p953215815518"></a><a name="p953215815518"></a>const uint16_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p18661136253"><a name="p18661136253"></a><a name="p18661136253"></a>Query vector for distance computation.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>The vector has a dimension of <code>d</code>.</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4982142445414"><a name="p4982142445414"></a><a name="p4982142445414"></a>y</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7532158856"><a name="p7532158856"></a><a name="p7532158856"></a>const uint16_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p36611261054"><a name="p36611261054"></a><a name="p36611261054"></a>Base vector for distance computation.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>The vector has a dimension of <code>d</code>.</p>
</td>
</tr>
<tr id="row106882715416"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p46812710547"><a name="p46812710547"></a><a name="p46812710547"></a>d</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p45311183519"><a name="p45311183519"></a><a name="p45311183519"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p17661261256"><a name="p17661261256"></a><a name="p17661261256"></a>Vector dimension.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p46952755416"><a name="p46952755416"></a><a name="p46952755416"></a>[1, 65535]</p>
</td>
</tr>
<tr id="row6435174117149"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4849194916526"><a name="p4849194916526"></a><a name="p4849194916526"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p484916497520"><a name="p484916497520"></a><a name="p484916497520"></a>float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p184912496525"><a name="p184912496525"></a><a name="p184912496525"></a>Stores the distance computation result.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1984914498527"><a name="p1984914498527"></a><a name="p1984914498527"></a>The size is specified by <code>dis_size</code>. The memory needs to be allocated in advance.</p>
</td>
</tr>
<tr id="row14276273554"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p271521115212"><a name="p271521115212"></a><a name="p271521115212"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p10722125214"><a name="p10722125214"></a><a name="p10722125214"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p1762116529"><a name="p1762116529"></a><a name="p1762116529"></a>Size of the distance result array.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p17182165214"><a name="p17182165214"></a><a name="p17182165214"></a>The value is <code>1</code>.</p>
</td>
</tr>
</tbody>
</table>

**Return Values<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a><code>0</code> is returned on successful execution. In case of failure, an error code is returned to indicate the specific issue.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

// Auxiliary function: Convert float to fp16.
uint16_t float_to_fp16(float value);

int main() {
    size_t dim = 128;  // Vector dimension

    // Prepare query and base vectors in fp16 format.
    uint16_t* query_vec_fp16 = (uint16_t*)malloc(dim * sizeof(uint16_t));
    uint16_t* base_vec_fp16 = (uint16_t*)malloc(dim * sizeof(uint16_t));

    // Populate with example data (converting the data to fp16 first).
    for (size_t i = 0; i < dim; i++) {
        query_vec_fp16[i] = float_to_fp16((float)i / dim);
        base_vec_fp16[i] = float_to_fp16((float)(dim - i) / dim);
    }

    // Store the distance result (output type is float).
    float distance = 0.0f;

    // Compute the Euclidean distance of fp16 vectors.
    int ret = krl_L2sqr_f16f32(query_vec_fp16, base_vec_fp16, dim, &distance, 1);

    if (ret != 0) {
        printf("fp16 distance computation failed. Error code: %d\n", ret);
        free(query_vec_fp16);
        free(base_vec_fp16);
        return -1;
    }

    printf("fp16 Euclidean distance (L2 squared): %f\n", distance);

    free(query_vec_fp16);
    free(base_vec_fp16);

    return 0;
}
```

### krl\_L2sqr\_u8u32

**Interface Definition<a name="section172317194488"></a>**

int krl\_L2sqr\_u8u32\(const uint8\_t\* x, const uint8\_t\* \_\_restrict y, size\_t d, uint32\_t\* dis, size\_t dis\_size\);

**Function<a name="section1153124784912"></a>**

Performs one-to-one Euclidean distance computation on vectors represented as 8-bit unsigned integers (uint8).

**Parameters<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="14.601460146014599%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="33.77337733773377%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="36.07360736073608%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p953215815518"><a name="p953215815518"></a><a name="p953215815518"></a>const uint8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.77337733773377%" headers="mcps1.1.5.1.3 "><p id="p18661136253"><a name="p18661136253"></a><a name="p18661136253"></a>Query vector for distance computation.</p>
</td>
<td class="cellrowborder" valign="top" width="36.07360736073608%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>The vector has a dimension of <code>d</code>.</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4982142445414"><a name="p4982142445414"></a><a name="p4982142445414"></a>y</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7532158856"><a name="p7532158856"></a><a name="p7532158856"></a>const uint8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.77337733773377%" headers="mcps1.1.5.1.3 "><p id="p36611261054"><a name="p36611261054"></a><a name="p36611261054"></a>Base vector for distance computation.</p>
</td>
<td class="cellrowborder" valign="top" width="36.07360736073608%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>The vector has a dimension of <code>d</code>.</p>
</td>
</tr>
<tr id="row106882715416"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p46812710547"><a name="p46812710547"></a><a name="p46812710547"></a>d</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p45311183519"><a name="p45311183519"></a><a name="p45311183519"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.77337733773377%" headers="mcps1.1.5.1.3 "><p id="p17661261256"><a name="p17661261256"></a><a name="p17661261256"></a>Vector dimension.</p>
</td>
<td class="cellrowborder" valign="top" width="36.07360736073608%" headers="mcps1.1.5.1.4 "><p id="p46952755416"><a name="p46952755416"></a><a name="p46952755416"></a>[1, 65535]</p>
</td>
</tr>
<tr id="row5811550198"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4849194916526"><a name="p4849194916526"></a><a name="p4849194916526"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p484916497520"><a name="p484916497520"></a><a name="p484916497520"></a>uint32_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.77337733773377%" headers="mcps1.1.5.1.3 "><p id="p184912496525"><a name="p184912496525"></a><a name="p184912496525"></a>Stores the distance computation result.</p>
</td>
<td class="cellrowborder" valign="top" width="36.07360736073608%" headers="mcps1.1.5.1.4 "><p id="p1984914498527"><a name="p1984914498527"></a><a name="p1984914498527"></a>The size is specified by <code>dis_size</code>. The memory needs to be allocated in advance.</p>
</td>
</tr>
<tr id="row1971384576"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p271521115212"><a name="p271521115212"></a><a name="p271521115212"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p10722125214"><a name="p10722125214"></a><a name="p10722125214"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.77337733773377%" headers="mcps1.1.5.1.3 "><p id="p1762116529"><a name="p1762116529"></a><a name="p1762116529"></a>Size of the distance result array.</p>
</td>
<td class="cellrowborder" valign="top" width="36.07360736073608%" headers="mcps1.1.5.1.4 "><p id="p17182165214"><a name="p17182165214"></a><a name="p17182165214"></a>The value is <code>1</code>.</p>
</td>
</tr>
</tbody>
</table>

**Return Values<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a><code>0</code> is returned on successful execution. In case of failure, an error code is returned to indicate the specific issue.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

int main() {
    size_t dim = 128;  // Vector dimension

    // Prepare query and base vectors in the uint8 type.
    uint8_t* query_vec = (uint8_t*)malloc(dim * sizeof(uint8_t));
    uint8_t* base_vec = (uint8_t*)malloc(dim * sizeof(uint8_t));

    // Populate with the example data (integers ranging from 0 to 255).
    for (size_t i = 0; i < dim; i++) {
        query_vec[i] = (uint8_t)(i * 2 % 256);
        base_vec[i] = (uint8_t)((dim - i) * 2 % 256);
    }

    // Store the distance result (uint32 type).
    uint32_t distance = 0;

    // Compute the Euclidean distance of uint8 vectors.
    int ret = krl_L2sqr_u8u32(query_vec, base_vec, dim, &distance, 1);

    if (ret != 0) {
        printf("uint8 distance computation failed. Error code: %d\n", ret);
        free(query_vec);
        free(base_vec);
        return -1;
    }

    printf("uint8 Euclidean distance (L2 squared): %u\n", distance);

    free(query_vec);
    free(base_vec);

    return 0;
}
```

### krl\_ipdis

**Interface Definition<a name="section172317194488"></a>**

int krl\_ipdis\(const float\* x, const float\* \_\_restrict y, const size\_t d, float\* dis, size\_t dis\_size\);

**Function<a name="section1153124784912"></a>**

Performs one-to-one distance computation using inner product on vectors represented in float precision.

**Parameters<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="14.591459145914593%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="34.003400340034005%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="14.591459145914593%" headers="mcps1.1.5.1.2 "><p id="p953215815518"><a name="p953215815518"></a><a name="p953215815518"></a>const float*</p>
</td>
<td class="cellrowborder" valign="top" width="34.003400340034005%" headers="mcps1.1.5.1.3 "><p id="p18661136253"><a name="p18661136253"></a><a name="p18661136253"></a>Query vector for distance computation.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>The vector has a dimension of <code>d</code>.</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4982142445414"><a name="p4982142445414"></a><a name="p4982142445414"></a>y</p>
</td>
<td class="cellrowborder" valign="top" width="14.591459145914593%" headers="mcps1.1.5.1.2 "><p id="p7532158856"><a name="p7532158856"></a><a name="p7532158856"></a>const float*</p>
</td>
<td class="cellrowborder" valign="top" width="34.003400340034005%" headers="mcps1.1.5.1.3 "><p id="p36611261054"><a name="p36611261054"></a><a name="p36611261054"></a>Base vector for distance computation.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>The vector has a dimension of <code>d</code>.</p>
</td>
</tr>
<tr id="row106882715416"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p46812710547"><a name="p46812710547"></a><a name="p46812710547"></a>d</p>
</td>
<td class="cellrowborder" valign="top" width="14.591459145914593%" headers="mcps1.1.5.1.2 "><p id="p45311183519"><a name="p45311183519"></a><a name="p45311183519"></a>const size_t</p>
</td>
<td class="cellrowborder" valign="top" width="34.003400340034005%" headers="mcps1.1.5.1.3 "><p id="p17661261256"><a name="p17661261256"></a><a name="p17661261256"></a>Vector dimension.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p46952755416"><a name="p46952755416"></a><a name="p46952755416"></a>[1, 65535]</p>
</td>
</tr>
<tr id="row6516613222"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p8546192216"><a name="p8546192216"></a><a name="p8546192216"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.591459145914593%" headers="mcps1.1.5.1.2 "><p id="p484916497520"><a name="p484916497520"></a><a name="p484916497520"></a>float*</p>
</td>
<td class="cellrowborder" valign="top" width="34.003400340034005%" headers="mcps1.1.5.1.3 "><p id="p184912496525"><a name="p184912496525"></a><a name="p184912496525"></a>Stores the distance computation result.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1984914498527"><a name="p1984914498527"></a><a name="p1984914498527"></a>The size is specified by <code>dis_size</code>. The memory needs to be allocated in advance.</p>
</td>
</tr>
<tr id="row976544717599"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p271521115212"><a name="p271521115212"></a><a name="p271521115212"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.591459145914593%" headers="mcps1.1.5.1.2 "><p id="p10722125214"><a name="p10722125214"></a><a name="p10722125214"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="34.003400340034005%" headers="mcps1.1.5.1.3 "><p id="p1762116529"><a name="p1762116529"></a><a name="p1762116529"></a>Size of the distance result array.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p17182165214"><a name="p17182165214"></a><a name="p17182165214"></a>The value is <code>1</code>.</p>
</td>
</tr>
</tbody>
</table>

**Return Values<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a><code>0</code> is returned on successful execution. In case of failure, an error code is returned to indicate the specific issue.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

int main() {
    size_t dim = 128;  // Vector dimension

    // Prepare the query vector and base vector.
    float* query_vec = (float*)malloc(dim * sizeof(float));
    float* base_vec = (float*)malloc(dim * sizeof(float));

    // Populate with the example data.
    float norm_q = 0.0f, norm_b = 0.0f;
    for (size_t i = 0; i < dim; i++) {
        query_vec[i] = (float)i;
        base_vec[i] = (float)(dim - i);
        norm_q += query_vec[i] * query_vec[i];
        norm_b += base_vec[i] * base_vec[i];
    }
    // Normalization
    norm_q = sqrtf(norm_q);
    norm_b = sqrtf(norm_b);
    for (size_t i = 0; i < dim; i++) {
        query_vec[i] /= norm_q;
        base_vec[i] /= norm_b;
    }

    // Store the distance result.
    float distance = 0.0f;

    // Compute the inner product distance.
    int ret = krl_ipdis(query_vec, base_vec, dim, &distance, 1);

    if (ret != 0) {
        printf("Failed to compute the inner product distance. Error code: %d\n", ret);
        free(query_vec);
        free(base_vec);
        return -1;
    }

    printf("inner product distance: %f\n", distance);
    // For normalized vectors, the inner product distance ranges from [–1, 1].

    free(query_vec);
    free(base_vec);

    return 0;
}
```

### krl\_negative\_ipdis\_f16f32

**Interface Definition<a name="section172317194488"></a>**

float krl\_negative\_ipdis\_f16f32\(const uint16\_t\* x, const uint16\_t\* \_\_restrict y, const size\_t d, float\* dis, size\_t dis\_size\);

**Function<a name="section1153124784912"></a>**

Performs one-to-one distance computation using inner product on vectors represented in fp16 precision.

**Parameters<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="14.601460146014599%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p953215815518"><a name="p953215815518"></a><a name="p953215815518"></a>const uint16_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p18661136253"><a name="p18661136253"></a><a name="p18661136253"></a>Query vector for distance computation.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>The vector has a dimension of <code>d</code>.</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4982142445414"><a name="p4982142445414"></a><a name="p4982142445414"></a>y</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7532158856"><a name="p7532158856"></a><a name="p7532158856"></a>const uint16_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p36611261054"><a name="p36611261054"></a><a name="p36611261054"></a>Base vector for distance computation.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>The vector has a dimension of <code>d</code>.</p>
</td>
</tr>
<tr id="row106882715416"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p46812710547"><a name="p46812710547"></a><a name="p46812710547"></a>d</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p45311183519"><a name="p45311183519"></a><a name="p45311183519"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p17661261256"><a name="p17661261256"></a><a name="p17661261256"></a>Vector dimension.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p46952755416"><a name="p46952755416"></a><a name="p46952755416"></a>[1, 65535]</p>
</td>
</tr>
<tr id="row172931135182017"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p8546192216"><a name="p8546192216"></a><a name="p8546192216"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p484916497520"><a name="p484916497520"></a><a name="p484916497520"></a>float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p184912496525"><a name="p184912496525"></a><a name="p184912496525"></a>Stores the distance computation result.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1984914498527"><a name="p1984914498527"></a><a name="p1984914498527"></a>The size is specified by <code>dis_size</code>. The memory needs to be allocated in advance.</p>
</td>
</tr>
<tr id="row54317463111"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p271521115212"><a name="p271521115212"></a><a name="p271521115212"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p10722125214"><a name="p10722125214"></a><a name="p10722125214"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p1762116529"><a name="p1762116529"></a><a name="p1762116529"></a>Size of the distance result array.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p17182165214"><a name="p17182165214"></a><a name="p17182165214"></a>The value is <code>1</code>.</p>
</td>
</tr>
</tbody>
</table>

**Return Values<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a><code>0</code> is returned on successful execution. In case of failure, an error code is returned to indicate the specific issue.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

// Auxiliary function: Convert float to fp16.
uint16_t float_to_fp16(float value);

int main() {
    size_t dim = 128;  // Vector dimension

    // Prepare vectors in fp16 format.
    uint16_t* query_vec_fp16 = (uint16_t*)malloc(dim * sizeof(uint16_t));
    uint16_t* base_vec_fp16 = (uint16_t*)malloc(dim * sizeof(uint16_t));

    // Populate with the example data.
    for (size_t i = 0; i < dim; i++) {
        query_vec_fp16[i] = float_to_fp16(0.1f);
        base_vec_fp16[i] = float_to_fp16(0.2f);
    }

    // Store the distance result.
    float distance = 0.0f;

    // Compute the inner product distance for fp16 vectors (returns the negated inner product).
    int ret = krl_negative_ipdis_f16f32(query_vec_fp16, base_vec_fp16, dim, &distance, 1);

    if (ret != 0) {
        printf("Failed to compute the inner product distance for fp16 vectors. Error code: %d\n", ret);
        free(query_vec_fp16);
        free(base_vec_fp16);
        return -1;
    }

    printf("Negative inner product distance for fp16 vectors: %f\n", distance);

    free(query_vec_fp16);
    free(base_vec_fp16);

    return 0;
}
```

### krl\_negative\_ipdis\_s8s32

**Interface Definition <a name="section172317194488"></a>**

int krl\_negative\_ipdis\_s8s32\(const int8\_t\* x, const int8\_t\* \_\_restrict y, const size\_t d, int32\_t\* dis, size\_t dis\_size\);

**Function<a name="section1153124784912"></a>**

Performs one-to-one distance computation using inner product on vectors represented as 8-bit signed integers (int8).

**Parameters<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="14.601460146014599%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p953215815518"><a name="p953215815518"></a><a name="p953215815518"></a>const int8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p18661136253"><a name="p18661136253"></a><a name="p18661136253"></a>Query vector for distance computation.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>The vector has a dimension of <code>d</code>.</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4982142445414"><a name="p4982142445414"></a><a name="p4982142445414"></a>y</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7532158856"><a name="p7532158856"></a><a name="p7532158856"></a>const int8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p36611261054"><a name="p36611261054"></a><a name="p36611261054"></a>Base vector for distance computation.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>The vector has a dimension of <code>d</code>.</p>
</td>
</tr>
<tr id="row106882715416"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p46812710547"><a name="p46812710547"></a><a name="p46812710547"></a>d</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p45311183519"><a name="p45311183519"></a><a name="p45311183519"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p17661261256"><a name="p17661261256"></a><a name="p17661261256"></a>Vector dimension.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p46952755416"><a name="p46952755416"></a><a name="p46952755416"></a>[1, 65535]</p>
</td>
</tr>
<tr id="row78157718211"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4816127192115"><a name="p4816127192115"></a><a name="p4816127192115"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p28168718210"><a name="p28168718210"></a><a name="p28168718210"></a>int32_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p184912496525"><a name="p184912496525"></a><a name="p184912496525"></a>Stores the distance computation result.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1984914498527"><a name="p1984914498527"></a><a name="p1984914498527"></a>The size is specified by <code>dis_size</code>. The memory needs to be allocated in advance.</p>
</td>
</tr>
<tr id="row162270523"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p271521115212"><a name="p271521115212"></a><a name="p271521115212"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p10722125214"><a name="p10722125214"></a><a name="p10722125214"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p1762116529"><a name="p1762116529"></a><a name="p1762116529"></a>Size of the distance result array.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p17182165214"><a name="p17182165214"></a><a name="p17182165214"></a>The value is <code>1</code>.</p>
</td>
</tr>
</tbody>
</table>

**Return Values<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a><code>0</code> is returned on successful execution. In case of failure, an error code is returned to indicate the specific issue.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

int main() {
    size_t dim = 128;  // Vector dimension

    // Prepare vectors of the int8 type.
    int8_t* query_vec = (int8_t*)malloc(dim * sizeof(int8_t));
    int8_t* base_vec = (int8_t*)malloc(dim * sizeof(int8_t));

    // Populate with the example data (ranging from –128 to 127).
    for (size_t i = 0; i < dim; i++) {
        query_vec[i] = (int8_t)(i % 128);
        base_vec[i] = (int8_t)((dim - i) % 128);
    }

    // Store the distance result (int32 type).
    int32_t distance = 0;

    // Compute the inner product distance for int8 vectors.
    int ret = krl_negative_ipdis_s8s32(query_vec, base_vec, dim, &distance, 1);

    if (ret != 0) {
        printf("Failed to compute the inner product distance for int8 vectors. Error code: %d\n", ret);
        free(query_vec);
        free(base_vec);
        return -1;
    }

    printf("Negative inner product distance for int8 vectors: %d\n", distance);

    free(query_vec);
    free(base_vec);

    return 0;
}
```

### krl\_L2sqr\_by\_idx

**Interface Definition<a name="section172317194488"></a>**

int krl\_L2sqr\_by\_idx\(float\* dis, const float\* x, const float\* y, const int64\_t\* ids, size\_t d, size\_t ny, size\_t dis\_size\);

**Function<a name="section1153124784912"></a>**

Performs one-to-many Euclidean distance computation on vectors represented in float precision.

**Parameters<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="14.601460146014599%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row92301478154"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p223015479158"><a name="p223015479158"></a><a name="p223015479158"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p11230154710156"><a name="p11230154710156"></a><a name="p11230154710156"></a>float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p82303471154"><a name="p82303471154"></a><a name="p82303471154"></a>Stores the distance computation result.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1984914498527"><a name="p1984914498527"></a><a name="p1984914498527"></a>The size is specified by <code>dis_size</code>. The memory needs to be allocated in advance.</p>
</td>
</tr>
<tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p953215815518"><a name="p953215815518"></a><a name="p953215815518"></a>const float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p18661136253"><a name="p18661136253"></a><a name="p18661136253"></a>Query vector for distance computation.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>The vector has a dimension of <code>d</code>.</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4982142445414"><a name="p4982142445414"></a><a name="p4982142445414"></a>y</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7532158856"><a name="p7532158856"></a><a name="p7532158856"></a>const float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p36611261054"><a name="p36611261054"></a><a name="p36611261054"></a>Base vector for distance computation.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>The size is specified by <code>d</code> × <code>ny</code>.</p>
</td>
</tr>
<tr id="row103951453161513"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p1395185361518"><a name="p1395185361518"></a><a name="p1395185361518"></a>ids</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p93958532154"><a name="p93958532154"></a><a name="p93958532154"></a>const int64_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p2039510531150"><a name="p2039510531150"></a><a name="p2039510531150"></a>IDs of base vectors.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p6395135351511"><a name="p6395135351511"></a><a name="p6395135351511"></a>The ID value is greater than or equal to 0  and less than the total number of base vectors.</p>
</td>
</tr>
<tr id="row106882715416"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p46812710547"><a name="p46812710547"></a><a name="p46812710547"></a>d</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p45311183519"><a name="p45311183519"></a><a name="p45311183519"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p17661261256"><a name="p17661261256"></a><a name="p17661261256"></a>Vector dimension.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p46952755416"><a name="p46952755416"></a><a name="p46952755416"></a>[1, 65535]</p>
</td>
</tr>
<tr id="row37151957141516"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p171515741513"><a name="p171515741513"></a><a name="p171515741513"></a>ny</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p3715105741513"><a name="p3715105741513"></a><a name="p3715105741513"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p197153572157"><a name="p197153572157"></a><a name="p197153572157"></a>Number of base vectors for distance computation.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1071517573156"><a name="p1071517573156"></a><a name="p1071517573156"></a>[1, 2^30-1]</p>
</td>
</tr>
<tr id="row1396217381443"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p39628388417"><a name="p39628388417"></a><a name="p39628388417"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p10722125214"><a name="p10722125214"></a><a name="p10722125214"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p1762116529"><a name="p1762116529"></a><a name="p1762116529"></a>Size of the distance result array.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p154517391451"><a name="p154517391451"></a><a name="p154517391451"></a>The value is specified by <code>ny</code>.</p>
</td>
</tr>
</tbody>
</table>

**Return Values<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a><code>0</code> is returned on successful execution. In case of failure, an error code is returned to indicate the specific issue.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

int main() {
    size_t dim = 128;                     // Vector dimension
    size_t total_base_vectors = 10000;    // Total number of base vectors
    size_t ny = 100;                      // Number of vectors to be used for distance computation.

    // Prepare the query vector.
    float* query_vec = (float*)malloc(dim * sizeof(float));
    for (size_t i = 0; i < dim; i++) {
        query_vec[i] = (float)(rand() % 1000) / 1000.0f;
    }

    // Prepare the base vector (which are usually loaded from a file or database in actual scenarios).
    float* base_vectors = (float*)malloc(total_base_vectors * dim * sizeof(float));
    for (size_t i = 0; i < total_base_vectors * dim; i++) {
        base_vectors[i] = (float)(rand() % 1000) / 1000.0f;
    }

    // Specify IDs of base vectors to be used for distance computation.
    // For example, compute distances for vectors with IDs 0, 10, 20, 30, ...
    int64_t* ids = (int64_t*)malloc(ny * sizeof(int64_t));
    for (size_t i = 0; i < ny; i++) {
        ids[i] = (int64_t)(i * 10); // Select one every 10.
    }

    // Allocate the distance result array.
    float* distances = (float*)malloc(ny * sizeof(float));

    // Perform one-to-many Euclidean distance computation.
    int ret = krl_L2sqr_by_idx(
        distances,      // Output
        query_vec, // Query vector
        base_vectors, // Base vector
        ids, // Specified vector IDs
        dim, // Vector dimension
        ny,             // Number of vectors for distance computation
        ny              // Length of the result array
    );

    if (ret != 0) {
        printf("Failed to compute the one-to-many distance. Error code: %d\n", ret);
        goto cleanup;
    }

    // Output the first five results.
    printf("One-to-many Euclidean distance computation result (first five results):\n");
    for (size_t i = 0; i < 5 && i < ny; i++) {
        printf("Distance to vector ID [%ld]: %f\n", ids[i], distances[i]);
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

**Interface Definition<a name="section172317194488"></a>**

int krl\_L2sqr\_by\_idx\_f16f32\(float\* dis, const uint16\_t\* x, const uint16\_t\* y, const int64\_t\* ids, size\_t d, size\_t ny, size\_t dis\_size\);

**Function<a name="section1153124784912"></a>**

Performs one-to-many Euclidean distance computation on vectors represented in fp16 precision.

**Parameters<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="14.601460146014599%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row92301478154"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p223015479158"><a name="p223015479158"></a><a name="p223015479158"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p11230154710156"><a name="p11230154710156"></a><a name="p11230154710156"></a>float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p184912496525"><a name="p184912496525"></a><a name="p184912496525"></a>Stores the distance computation result.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p923018478155"><a name="p923018478155"></a><a name="p923018478155"></a>The size is specified by <code>dis_size</code>. The memory needs to be allocated in advance.</p>
</td>
</tr>
<tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p953215815518"><a name="p953215815518"></a><a name="p953215815518"></a>const uint16_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p18661136253"><a name="p18661136253"></a><a name="p18661136253"></a>Query vector for distance computation.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>The vector has a dimension of <code>d</code>.</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4982142445414"><a name="p4982142445414"></a><a name="p4982142445414"></a>y</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7532158856"><a name="p7532158856"></a><a name="p7532158856"></a>const uint16_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p36611261054"><a name="p36611261054"></a><a name="p36611261054"></a>Base vector for distance computation.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>The size is specified by <code>d</code> × <code>ny</code>.</p>
</td>
</tr>
<tr id="row103951453161513"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p1395185361518"><a name="p1395185361518"></a><a name="p1395185361518"></a>ids</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p93958532154"><a name="p93958532154"></a><a name="p93958532154"></a>const int64_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p2039510531150"><a name="p2039510531150"></a><a name="p2039510531150"></a>IDs of base vectors.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p6395135351511"><a name="p6395135351511"></a><a name="p6395135351511"></a>The ID value is greater than or equal to 0  and less than the total number of base vectors.</p>
</td>
</tr>
<tr id="row106882715416"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p46812710547"><a name="p46812710547"></a><a name="p46812710547"></a>d</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p45311183519"><a name="p45311183519"></a><a name="p45311183519"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p17661261256"><a name="p17661261256"></a><a name="p17661261256"></a>Vector dimension.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p46952755416"><a name="p46952755416"></a><a name="p46952755416"></a>[1, 65535]</p>
</td>
</tr>
<tr id="row37151957141516"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p171515741513"><a name="p171515741513"></a><a name="p171515741513"></a>ny</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p3715105741513"><a name="p3715105741513"></a><a name="p3715105741513"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p197153572157"><a name="p197153572157"></a><a name="p197153572157"></a>Number of base vectors for distance computation.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1071517573156"><a name="p1071517573156"></a><a name="p1071517573156"></a>[1, 2^30-1]</p>
</td>
</tr>
<tr id="row106371540187"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p39628388417"><a name="p39628388417"></a><a name="p39628388417"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p10722125214"><a name="p10722125214"></a><a name="p10722125214"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p1762116529"><a name="p1762116529"></a><a name="p1762116529"></a>Size of the distance result array.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p154517391451"><a name="p154517391451"></a><a name="p154517391451"></a>The value is specified by <code>ny</code>.</p>
</td>
</tr>
</tbody>
</table>

**Return Values<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a><code>0</code> is returned on successful execution. In case of failure, an error code is returned to indicate the specific issue.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

// Auxiliary function: Convert float to fp16.
uint16_t float_to_fp16(float value);

int main() {
    size_t dim = 128;
    size_t total_base_vectors = 10000;
    size_t ny = 50; // Compute the distances for 50 vectors.

    // Prepare query vectors in fp16 format.
    uint16_t* query_vec_fp16 = (uint16_t*)malloc(dim * sizeof(uint16_t));
    for (size_t i = 0; i < dim; i++) {
        query_vec_fp16[i] = float_to_fp16((float)(rand() % 1000) / 1000.0f);
    }

    // Prepare base vectors in fp16 format.
    uint16_t* base_vectors_fp16 = (uint16_t*)malloc(total_base_vectors * dim * sizeof(uint16_t));
    for (size_t i = 0; i < total_base_vectors * dim; i++) {
        base_vectors_fp16[i] = float_to_fp16((float)(rand() % 1000) / 1000.0f);
    }

    // Specify IDs of vectors for distance computation (randomly selected).
    int64_t* ids = (int64_t*)malloc(ny * sizeof(int64_t));
    for (size_t i = 0; i < ny; i++) {
        ids[i] = rand() % total_base_vectors;
    }

    // Allocate the distance result array (the output type is still float).
    float* distances = (float*)malloc(ny * sizeof(float));

    // Perform one-to-many Euclidean distance computation on vectors represented in fp16 precision.
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
        printf("Failed to compute the one-to-many distance for fp16 vectors. Error code: %d\n", ret);
        goto cleanup;
    }

    printf("Successfully computed the one-to-many Euclidean distance for fp16 vectors.\n");
    printf("First 3 results:\n");
    for (size_t i = 0; i < 3 && i < ny; i++) {
        printf("  Vector ID [%ld]: distance = %f\n", ids[i], distances[i]);
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

**Interface Definition<a name="section172317194488"></a>**

int krl\_L2sqr\_by\_idx\_u8f32\(float\* dis, const uint8\_t\* x, const uint8\_t\* y, const int64\_t\* ids, size\_t d, size\_t ny, size\_t dis\_size\);

**Function<a name="section1153124784912"></a>**

Performs one-to-many Euclidean distance computation on vectors represented as 8-bit unsigned integers (uint8).

**Parameters<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="14.601460146014599%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row92301478154"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p223015479158"><a name="p223015479158"></a><a name="p223015479158"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p11230154710156"><a name="p11230154710156"></a><a name="p11230154710156"></a>float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p184912496525"><a name="p184912496525"></a><a name="p184912496525"></a>Stores the distance computation result.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p923018478155"><a name="p923018478155"></a><a name="p923018478155"></a>The size is specified by <code>dis_size</code>. The memory needs to be allocated in advance.</p>
</td>
</tr>
<tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p953215815518"><a name="p953215815518"></a><a name="p953215815518"></a>const uint8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p18661136253"><a name="p18661136253"></a><a name="p18661136253"></a>Query vector for distance computation.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>The vector has a dimension of <code>d</code>.</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4982142445414"><a name="p4982142445414"></a><a name="p4982142445414"></a>y</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p154911116102813"><a name="p154911116102813"></a><a name="p154911116102813"></a>const uint8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p36611261054"><a name="p36611261054"></a><a name="p36611261054"></a>Base vector for distance computation.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>The size is specified by <code>d</code> × <code>ny</code>.</p>
</td>
</tr>
<tr id="row103951453161513"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p1395185361518"><a name="p1395185361518"></a><a name="p1395185361518"></a>ids</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p93958532154"><a name="p93958532154"></a><a name="p93958532154"></a>const int64_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p2039510531150"><a name="p2039510531150"></a><a name="p2039510531150"></a>IDs of base vectors.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p19345103171215"><a name="p19345103171215"></a><a name="p19345103171215"></a>The ID value is greater than or equal to 0  and less than the total number of base vectors.</p>
</td>
</tr>
<tr id="row106882715416"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p46812710547"><a name="p46812710547"></a><a name="p46812710547"></a>d</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p45311183519"><a name="p45311183519"></a><a name="p45311183519"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p17661261256"><a name="p17661261256"></a><a name="p17661261256"></a>Vector dimension.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p46952755416"><a name="p46952755416"></a><a name="p46952755416"></a>[1, 65535]</p>
</td>
</tr>
<tr id="row37151957141516"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p171515741513"><a name="p171515741513"></a><a name="p171515741513"></a>ny</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p3715105741513"><a name="p3715105741513"></a><a name="p3715105741513"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p197153572157"><a name="p197153572157"></a><a name="p197153572157"></a>Number of base vectors for distance computation.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1071517573156"><a name="p1071517573156"></a><a name="p1071517573156"></a>[1, 2^30-1]</p>
</td>
</tr>
<tr id="row1689332720259"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p39628388417"><a name="p39628388417"></a><a name="p39628388417"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p10722125214"><a name="p10722125214"></a><a name="p10722125214"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p1762116529"><a name="p1762116529"></a><a name="p1762116529"></a>Size of the distance result array.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p154517391451"><a name="p154517391451"></a><a name="p154517391451"></a>The value is specified by <code>ny</code>.</p>
</td>
</tr>
</tbody>
</table>

**Return Values<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a><code>0</code> is returned on successful execution. In case of failure, an error code is returned to indicate the specific issue.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

int main() {
    size_t dim = 128;
    size_t total_base_vectors = 5000;
    size_t ny = 200;  // Compute the distances for 200 vectors.

    // Prepare the query vector of the uint8 type.
    uint8_t* query_vec = (uint8_t*)malloc(dim * sizeof(uint8_t));
    for (size_t i = 0; i < dim; i++) {
        query_vec[i] = (uint8_t)(rand() % 256);
    }

    // Prepare base vectors of the uint8 type.
    uint8_t* base_vectors = (uint8_t*)malloc(total_base_vectors * dim * sizeof(uint8_t));
    for (size_t i = 0; i < total_base_vectors * dim; i++) {
        base_vectors[i] = (uint8_t)(rand() % 256);
    }

    // Specify IDs of vectors for distance computation.
    int64_t* ids = (int64_t*)malloc(ny * sizeof(int64_t));
    for (size_t i = 0; i < ny; i++) {
        ids[i] = (int64_t)(i * 25); // Select one every 25.
    }

    // Allocate the distance result array (the output type is float).
    float* distances = (float*)malloc(ny * sizeof(float));

    // Perform one-to-many Euclidean distance computation on vectors represented as 8-bit unsigned integers (uint8).
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
        printf("Failed to compute the one-to-many distance for vectors in the uint8 type. Error code: %d\n", ret);
        goto cleanup;
    }

    printf("Successfully computed the one-to-many Euclidean distance for vectors in the uint8 type\n");
    
    // Determine the minimum distance.
    float min_dist = distances[0];
    int64_t min_id = ids[0];
    for (size_t i = 1; i < ny; i++) {
        if (distances[i] < min_dist) {
            min_dist = distances[i];
            min_id = ids[i];
        }
    }
    printf("ID of the nearest neighbor vector: %ld, distance: %f\n", min_id, min_dist);

cleanup:
    free(query_vec);
    free(base_vectors);
    free(ids);
    free(distances);

    return ret;
}
```

### krl\_inner\_product\_by\_idx

**Interface Definition<a name="section172317194488"></a>**

int krl\_inner\_product\_by\_idx\(float\* dis, const float\* x, const float\* y, const int64\_t\* ids, size\_t d, size\_t ny, size\_t dis\_size\);

**Function<a name="section1153124784912"></a>**

Performs one-to-many distance computation using inner product on vectors represented in float precision.

**Parameters<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="14.601460146014599%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="33.97339733973397%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="35.873587358735875%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row92301478154"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p223015479158"><a name="p223015479158"></a><a name="p223015479158"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p11230154710156"><a name="p11230154710156"></a><a name="p11230154710156"></a>float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.97339733973397%" headers="mcps1.1.5.1.3 "><p id="p82303471154"><a name="p82303471154"></a><a name="p82303471154"></a>Stores the distance computation result.</p>
</td>
<td class="cellrowborder" valign="top" width="35.873587358735875%" headers="mcps1.1.5.1.4 "><p id="p923018478155"><a name="p923018478155"></a><a name="p923018478155"></a>The size is specified by <code>dis_size</code>. The memory needs to be allocated in advance.</p>
</td>
</tr>
<tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p953215815518"><a name="p953215815518"></a><a name="p953215815518"></a>const float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.97339733973397%" headers="mcps1.1.5.1.3 "><p id="p18661136253"><a name="p18661136253"></a><a name="p18661136253"></a>Query vector for distance computation.</p>
</td>
<td class="cellrowborder" valign="top" width="35.873587358735875%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>The vector has a dimension of <code>d</code>.</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4982142445414"><a name="p4982142445414"></a><a name="p4982142445414"></a>y</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7532158856"><a name="p7532158856"></a><a name="p7532158856"></a>const float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.97339733973397%" headers="mcps1.1.5.1.3 "><p id="p36611261054"><a name="p36611261054"></a><a name="p36611261054"></a>Base vector for distance computation.</p>
</td>
<td class="cellrowborder" valign="top" width="35.873587358735875%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>The size is specified by <code>d</code> × <code>ny</code>.</p>
</td>
</tr>
<tr id="row103951453161513"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p1395185361518"><a name="p1395185361518"></a><a name="p1395185361518"></a>ids</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p93958532154"><a name="p93958532154"></a><a name="p93958532154"></a>const int64_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.97339733973397%" headers="mcps1.1.5.1.3 "><p id="p2039510531150"><a name="p2039510531150"></a><a name="p2039510531150"></a>IDs of base vectors.</p>
</td>
<td class="cellrowborder" valign="top" width="35.873587358735875%" headers="mcps1.1.5.1.4 "><p id="p6395135351511"><a name="p6395135351511"></a><a name="p6395135351511"></a>The ID value is greater than or equal to 0  and less than the total number of base vectors.</p>
</td>
</tr>
<tr id="row106882715416"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p46812710547"><a name="p46812710547"></a><a name="p46812710547"></a>d</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p45311183519"><a name="p45311183519"></a><a name="p45311183519"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.97339733973397%" headers="mcps1.1.5.1.3 "><p id="p17661261256"><a name="p17661261256"></a><a name="p17661261256"></a>Vector dimension.</p>
</td>
<td class="cellrowborder" valign="top" width="35.873587358735875%" headers="mcps1.1.5.1.4 "><p id="p46952755416"><a name="p46952755416"></a><a name="p46952755416"></a>[1, 65535]</p>
</td>
</tr>
<tr id="row37151957141516"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p171515741513"><a name="p171515741513"></a><a name="p171515741513"></a>ny</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p3715105741513"><a name="p3715105741513"></a><a name="p3715105741513"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.97339733973397%" headers="mcps1.1.5.1.3 "><p id="p197153572157"><a name="p197153572157"></a><a name="p197153572157"></a>Number of base vectors for distance computation.</p>
</td>
<td class="cellrowborder" valign="top" width="35.873587358735875%" headers="mcps1.1.5.1.4 "><p id="p1071517573156"><a name="p1071517573156"></a><a name="p1071517573156"></a>[1, 2^30-1]</p>
</td>
</tr>
<tr id="row195051882311"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p39628388417"><a name="p39628388417"></a><a name="p39628388417"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p10722125214"><a name="p10722125214"></a><a name="p10722125214"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.97339733973397%" headers="mcps1.1.5.1.3 "><p id="p1762116529"><a name="p1762116529"></a><a name="p1762116529"></a>Size of the distance result array.</p>
</td>
<td class="cellrowborder" valign="top" width="35.873587358735875%" headers="mcps1.1.5.1.4 "><p id="p154517391451"><a name="p154517391451"></a><a name="p154517391451"></a>The value is specified by <code>ny</code>.</p>
</td>
</tr>
</tbody>
</table>

**Return Values<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a><code>0</code> is returned on successful execution. In case of failure, an error code is returned to indicate the specific issue.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c
#include <stdio.h>
#include <stdlib.h>
#include <math.h>
#include "krl.h"

// Auxiliary function: vector normalization
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

    // Prepare the query vector and normalize it.
    float* query_vec = (float*)malloc(dim * sizeof(float));
    for (size_t i = 0; i < dim; i++) {
        query_vec[i] = (float)(rand() % 1000) / 1000.0f;
    }
    normalize_vector(query_vec, dim);

    // Prepare the base vector and normalize it.
    float* base_vectors = (float*)malloc(total_base_vectors * dim * sizeof(float));
    for (size_t j = 0; j < total_base_vectors; j++) {
        for (size_t i = 0; i < dim; i++) {
            base_vectors[j * dim + i] = (float)(rand() % 1000) / 1000.0f;
        }
        normalize_vector(&base_vectors[j * dim], dim);
    }

    // Specify IDs of vectors for distance computation.
    int64_t* ids = (int64_t*)malloc(ny * sizeof(int64_t));
    for (size_t i = 0; i < ny; i++) {
        ids[i] = rand() % total_base_vectors;
    }

    // Allocate the distance result array.
    float* distances = (float*)malloc(ny * sizeof(float));

    // Perform one-to-many inner product distance computation.
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
        printf("Failed to compute the one-to-many inner product distance. Error code: %d\n", ret);
        goto cleanup;
    }

    printf("Successfully computed the one-to-many inner product distance.\n");
    
    // For normalized vectors, a larger inner product value indicates higher similarity.
    // Determine the maximum inner product (most similar).
    float max_ip = distances[0];
    int64_t max_id = ids[0];
    for (size_t i = 1; i < ny; i++) {
        if (distances[i] > max_ip) {
            max_ip = distances[i];
            max_id = ids[i];
        }
    }
    printf("ID of the most similar vector: %ld, inner product value: %f\n", max_id, max_ip);

cleanup:
    free(query_vec);
    free(base_vectors);
    free(ids);
    free(distances);

    return ret;
}
```

### krl\_inner\_product\_by\_idx\_f16f32

**Interface Definition<a name="section172317194488"></a>**

int krl\_inner\_product\_by\_idx\_f16f32\(float\* dis, const uint16\_t\* x, const uint16\_t\* y, const int64\_t\* ids, size\_t d, size\_t ny, size\_t dis\_size\);

**Function<a name="section1153124784912"></a>**

Performs one-to-many distance computation using inner product on vectors represented in fp16 precision.

**Parameters<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="14.601460146014599%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="33.663366336633665%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="36.18361836183618%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row92301478154"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p223015479158"><a name="p223015479158"></a><a name="p223015479158"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p11230154710156"><a name="p11230154710156"></a><a name="p11230154710156"></a>float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.663366336633665%" headers="mcps1.1.5.1.3 "><p id="p82303471154"><a name="p82303471154"></a><a name="p82303471154"></a>Stores the distance computation result.</p>
</td>
<td class="cellrowborder" valign="top" width="36.18361836183618%" headers="mcps1.1.5.1.4 "><p id="p923018478155"><a name="p923018478155"></a><a name="p923018478155"></a>The size is specified by <code>dis_size</code>. The memory needs to be allocated in advance.</p>
</td>
</tr>
<tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p953215815518"><a name="p953215815518"></a><a name="p953215815518"></a>const uint16_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.663366336633665%" headers="mcps1.1.5.1.3 "><p id="p18661136253"><a name="p18661136253"></a><a name="p18661136253"></a>Query vector for distance computation.</p>
</td>
<td class="cellrowborder" valign="top" width="36.18361836183618%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>The vector has a dimension of <code>d</code>.</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4982142445414"><a name="p4982142445414"></a><a name="p4982142445414"></a>y</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7532158856"><a name="p7532158856"></a><a name="p7532158856"></a>const uint16_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.663366336633665%" headers="mcps1.1.5.1.3 "><p id="p36611261054"><a name="p36611261054"></a><a name="p36611261054"></a>Base vector for distance computation.</p>
</td>
<td class="cellrowborder" valign="top" width="36.18361836183618%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>The size is specified by <code>d</code> × <code>ny</code>.</p>
</td>
</tr>
<tr id="row103951453161513"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p1395185361518"><a name="p1395185361518"></a><a name="p1395185361518"></a>ids</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p93958532154"><a name="p93958532154"></a><a name="p93958532154"></a>const int64_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.663366336633665%" headers="mcps1.1.5.1.3 "><p id="p2039510531150"><a name="p2039510531150"></a><a name="p2039510531150"></a>IDs of base vectors.</p>
</td>
<td class="cellrowborder" valign="top" width="36.18361836183618%" headers="mcps1.1.5.1.4 "><p id="p6395135351511"><a name="p6395135351511"></a><a name="p6395135351511"></a>The ID value is greater than or equal to 0  and less than the total number of base vectors.</p>
</td>
</tr>
<tr id="row106882715416"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p46812710547"><a name="p46812710547"></a><a name="p46812710547"></a>d</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p45311183519"><a name="p45311183519"></a><a name="p45311183519"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.663366336633665%" headers="mcps1.1.5.1.3 "><p id="p17661261256"><a name="p17661261256"></a><a name="p17661261256"></a>Vector dimension.</p>
</td>
<td class="cellrowborder" valign="top" width="36.18361836183618%" headers="mcps1.1.5.1.4 "><p id="p46952755416"><a name="p46952755416"></a><a name="p46952755416"></a>[1, 65535]</p>
</td>
</tr>
<tr id="row37151957141516"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p171515741513"><a name="p171515741513"></a><a name="p171515741513"></a>ny</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p3715105741513"><a name="p3715105741513"></a><a name="p3715105741513"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.663366336633665%" headers="mcps1.1.5.1.3 "><p id="p197153572157"><a name="p197153572157"></a><a name="p197153572157"></a>Number of base vectors for distance computation.</p>
</td>
<td class="cellrowborder" valign="top" width="36.18361836183618%" headers="mcps1.1.5.1.4 "><p id="p1071517573156"><a name="p1071517573156"></a><a name="p1071517573156"></a>[1, 2^30-1]</p>
</td>
</tr>
<tr id="row36562453314"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p39628388417"><a name="p39628388417"></a><a name="p39628388417"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p10722125214"><a name="p10722125214"></a><a name="p10722125214"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.663366336633665%" headers="mcps1.1.5.1.3 "><p id="p1762116529"><a name="p1762116529"></a><a name="p1762116529"></a>Size of the distance result array.</p>
</td>
<td class="cellrowborder" valign="top" width="36.18361836183618%" headers="mcps1.1.5.1.4 "><p id="p154517391451"><a name="p154517391451"></a><a name="p154517391451"></a>The value is specified by <code>ny</code>.</p>
</td>
</tr>
</tbody>
</table>

**Return Values<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a><code>0</code> is returned on successful execution. In case of failure, an error code is returned to indicate the specific issue.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

// Auxiliary function: Convert float to fp16.
uint16_t float_to_fp16(float value);

int main() {
    size_t dim = 256;
    size_t total_base_vectors = 8000;
    size_t ny = 64;

    // Prepare query vectors in fp16 format.
    uint16_t* query_vec_fp16 = (uint16_t*)malloc(dim * sizeof(uint16_t));
    for (size_t i = 0; i < dim; i++) {
        query_vec_fp16[i] = float_to_fp16(0.1f);
    }

    // Prepare base vectors in fp16 format.
    uint16_t* base_vectors_fp16 = (uint16_t*)malloc(total_base_vectors * dim * sizeof(uint16_t));
    for (size_t i = 0; i < total_base_vectors * dim; i++) {
        base_vectors_fp16[i] = float_to_fp16((float)(rand() % 100) / 100.0f);
    }

    // Specify IDs of vectors for distance computation.
    int64_t* ids = (int64_t*)malloc(ny * sizeof(int64_t));
    for (size_t i = 0; i < ny; i++) {
        ids[i] = (int64_t)(i * 100);
    }

    // Allocate the distance result array.
    float* distances = (float*)malloc(ny * sizeof(float));

    // Perform one-to-many inner product distance computation on vectors represented in fp16 precision.
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
        printf("Failed to compute the one-to-many inner product distance for vectors represented in fp16 precision. Error code: %d\n", ret);
        goto cleanup;
    }

    printf("Successfully computed the one-to-many inner product distance for vectors represented in fp16 precision.\n");
    printf("First 5 results:\n");
    for (size_t i = 0; i < 5 && i < ny; i++) {
        printf("  Vector ID [%ld]: inner product = %f\n", ids[i], distances[i]);
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

**Interface Definition<a name="section172317194488"></a>**

int krl\_negative\_inner\_product\_by\_idx\_f16f32\(float\* dis, const uint16\_t\* x, const uint16\_t\* y, const int64\_t\* ids, size\_t d, size\_t ny, size\_t dis\_size\);

**Function<a name="section1153124784912"></a>**

Performs one-to-many distance computation using inner product on vectors represented in fp16 precision, and negates the computation results.

**Parameters<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="14.661466146614663%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="33.93339333933393%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row92301478154"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p223015479158"><a name="p223015479158"></a><a name="p223015479158"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.661466146614663%" headers="mcps1.1.5.1.2 "><p id="p11230154710156"><a name="p11230154710156"></a><a name="p11230154710156"></a>float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.93339333933393%" headers="mcps1.1.5.1.3 "><p id="p82303471154"><a name="p82303471154"></a><a name="p82303471154"></a>Stores the distance computation result.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p923018478155"><a name="p923018478155"></a><a name="p923018478155"></a>The size is specified by <code>dis_size</code>. The memory needs to be allocated in advance.</p>
</td>
</tr>
<tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="14.661466146614663%" headers="mcps1.1.5.1.2 "><p id="p953215815518"><a name="p953215815518"></a><a name="p953215815518"></a>const uint16_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.93339333933393%" headers="mcps1.1.5.1.3 "><p id="p18661136253"><a name="p18661136253"></a><a name="p18661136253"></a>Query vector for distance computation.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>The vector has a dimension of <code>d</code>.</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4982142445414"><a name="p4982142445414"></a><a name="p4982142445414"></a>y</p>
</td>
<td class="cellrowborder" valign="top" width="14.661466146614663%" headers="mcps1.1.5.1.2 "><p id="p7532158856"><a name="p7532158856"></a><a name="p7532158856"></a>const uint16_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.93339333933393%" headers="mcps1.1.5.1.3 "><p id="p36611261054"><a name="p36611261054"></a><a name="p36611261054"></a>Base vector for distance computation.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>The size is specified by <code>d</code> × <code>ny</code>.</p>
</td>
</tr>
<tr id="row103951453161513"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p1395185361518"><a name="p1395185361518"></a><a name="p1395185361518"></a>ids</p>
</td>
<td class="cellrowborder" valign="top" width="14.661466146614663%" headers="mcps1.1.5.1.2 "><p id="p93958532154"><a name="p93958532154"></a><a name="p93958532154"></a>const int64_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.93339333933393%" headers="mcps1.1.5.1.3 "><p id="p2039510531150"><a name="p2039510531150"></a><a name="p2039510531150"></a>IDs of base vectors.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p6395135351511"><a name="p6395135351511"></a><a name="p6395135351511"></a>The ID value is greater than or equal to 0  and less than the total number of base vectors.</p>
</td>
</tr>
<tr id="row106882715416"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p46812710547"><a name="p46812710547"></a><a name="p46812710547"></a>d</p>
</td>
<td class="cellrowborder" valign="top" width="14.661466146614663%" headers="mcps1.1.5.1.2 "><p id="p45311183519"><a name="p45311183519"></a><a name="p45311183519"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.93339333933393%" headers="mcps1.1.5.1.3 "><p id="p17661261256"><a name="p17661261256"></a><a name="p17661261256"></a>Vector dimension.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p46952755416"><a name="p46952755416"></a><a name="p46952755416"></a>[1, 65535]</p>
</td>
</tr>
<tr id="row37151957141516"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p171515741513"><a name="p171515741513"></a><a name="p171515741513"></a>ny</p>
</td>
<td class="cellrowborder" valign="top" width="14.661466146614663%" headers="mcps1.1.5.1.2 "><p id="p3715105741513"><a name="p3715105741513"></a><a name="p3715105741513"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.93339333933393%" headers="mcps1.1.5.1.3 "><p id="p197153572157"><a name="p197153572157"></a><a name="p197153572157"></a>Number of base vectors for distance computation.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1071517573156"><a name="p1071517573156"></a><a name="p1071517573156"></a>[1, 2^30-1]</p>
</td>
</tr>
<tr id="row17278128173918"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p39628388417"><a name="p39628388417"></a><a name="p39628388417"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.661466146614663%" headers="mcps1.1.5.1.2 "><p id="p10722125214"><a name="p10722125214"></a><a name="p10722125214"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.93339333933393%" headers="mcps1.1.5.1.3 "><p id="p1762116529"><a name="p1762116529"></a><a name="p1762116529"></a>Size of the distance result array.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p154517391451"><a name="p154517391451"></a><a name="p154517391451"></a>The value is specified by <code>ny</code>.</p>
</td>
</tr>
</tbody>
</table>

**Return Values<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a><code>0</code> is returned on successful execution. In case of failure, an error code is returned to indicate the specific issue.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

// Auxiliary function: Convert float to fp16.
uint16_t float_to_fp16(float value);

int main() {
    size_t dim = 128;
    size_t total_base_vectors = 5000;
    size_t ny = 100;

    // Prepare query vectors in fp16 format.
    uint16_t* query_vec_fp16 = (uint16_t*)malloc(dim * sizeof(uint16_t));
    for (size_t i = 0; i < dim; i++) {
        query_vec_fp16[i] = float_to_fp16(0.5f);
    }

    // Prepare base vectors in fp16 format.
    uint16_t* base_vectors_fp16 = (uint16_t*)malloc(total_base_vectors * dim * sizeof(uint16_t));
    for (size_t i = 0; i < total_base_vectors * dim; i++) {
        base_vectors_fp16[i] = float_to_fp16((float)(rand() % 100) / 100.0f);
    }

    // Specify IDs of vectors for distance computation.
    int64_t* ids = (int64_t*)malloc(ny * sizeof(int64_t));
    for (size_t i = 0; i < ny; i++) {
        ids[i] = rand() % total_base_vectors;
    }

    // Allocate the distance result array.
    float* distances = (float*)malloc(ny * sizeof(float));

    // Perform one-to-many negative inner product distance computation on vectors represented in fp16 precision.
    // Note: The result is the negative value of the inner product, which can be directly used in a min-heap to find the most similar vectors.
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
        printf("Failed to compute the one-to-many negative inner product distance for vectors represented in fp16 precision. Error code: %d\n", ret);
        goto cleanup;
    }

    printf("Successfully computed the one-to-many negative inner product distance for vectors represented in fp16 precision.\n");
    
    // When the negative inner product is used, a smaller value indicates a larger original inner product (higher similarity).
    // Therefore, you can directly use the minimum value to find the most similar vector.
    float min_neg_ip = distances[0];
    int64_t most_similar_id = ids[0];
    for (size_t i = 1; i < ny; i++) {
        if (distances[i] < min_neg_ip) {
            min_neg_ip = distances[i];
            most_similar_id = ids[i];
        }
    }
    
    printf("ID of the most similar vector: %ld\n", most_similar_id);
    printf("Negative inner product value: %f (original inner product: %f)\n", min_neg_ip, -min_neg_ip);

cleanup:
    free(query_vec_fp16);
    free(base_vectors_fp16);
    free(ids);
    free(distances);

    return ret;
}
```

### krl\_inner\_product\_by\_idx\_s8f32

**Interface Definition<a name="section172317194488"></a>**

int krl\_inner\_product\_by\_idx\_s8f32\(float\* dis, const int8\_t\* x, const int8\_t\* y, const int64\_t\* ids, size\_t d, size\_t ny, size\_t dis\_size\);

**Function<a name="section1153124784912"></a>**

Performs one-to-many distance computation using inner product on vectors represented as 8-bit signed integers (int8).

**Parameters<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="14.601460146014599%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row92301478154"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p223015479158"><a name="p223015479158"></a><a name="p223015479158"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p11230154710156"><a name="p11230154710156"></a><a name="p11230154710156"></a>float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p184912496525"><a name="p184912496525"></a><a name="p184912496525"></a>Stores the distance computation result.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p923018478155"><a name="p923018478155"></a><a name="p923018478155"></a>The size is specified by <code>dis_size</code>. The memory needs to be allocated in advance.</p>
</td>
</tr>
<tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p953215815518"><a name="p953215815518"></a><a name="p953215815518"></a>const int8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p18661136253"><a name="p18661136253"></a><a name="p18661136253"></a>Query vector for distance computation.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>The vector has a dimension of <code>d</code>.</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4982142445414"><a name="p4982142445414"></a><a name="p4982142445414"></a>y</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p154911116102813"><a name="p154911116102813"></a><a name="p154911116102813"></a>const int8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p36611261054"><a name="p36611261054"></a><a name="p36611261054"></a>Base vector for distance computation.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>The size is specified by <code>d</code> × <code>ny</code>.</p>
</td>
</tr>
<tr id="row103951453161513"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p1395185361518"><a name="p1395185361518"></a><a name="p1395185361518"></a>ids</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p93958532154"><a name="p93958532154"></a><a name="p93958532154"></a>const int64_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p2039510531150"><a name="p2039510531150"></a><a name="p2039510531150"></a>IDs of base vectors.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p6395135351511"><a name="p6395135351511"></a><a name="p6395135351511"></a>The ID value is greater than or equal to 0  and less than the total number of base vectors.</p>
</td>
</tr>
<tr id="row106882715416"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p46812710547"><a name="p46812710547"></a><a name="p46812710547"></a>d</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p45311183519"><a name="p45311183519"></a><a name="p45311183519"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p17661261256"><a name="p17661261256"></a><a name="p17661261256"></a>Vector dimension.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p46952755416"><a name="p46952755416"></a><a name="p46952755416"></a>[1, 65535]</p>
</td>
</tr>
<tr id="row37151957141516"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p171515741513"><a name="p171515741513"></a><a name="p171515741513"></a>ny</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p3715105741513"><a name="p3715105741513"></a><a name="p3715105741513"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p197153572157"><a name="p197153572157"></a><a name="p197153572157"></a>Number of base vectors for distance computation.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1071517573156"><a name="p1071517573156"></a><a name="p1071517573156"></a>[1, 2^30-1]</p>
</td>
</tr>
<tr id="row5987191044118"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p39628388417"><a name="p39628388417"></a><a name="p39628388417"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p10722125214"><a name="p10722125214"></a><a name="p10722125214"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p1762116529"><a name="p1762116529"></a><a name="p1762116529"></a>Size of the distance result array.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p154517391451"><a name="p154517391451"></a><a name="p154517391451"></a>The value is specified by <code>ny</code>.</p>
</td>
</tr>
</tbody>
</table>

**Return Values<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a><code>0</code> is returned on successful execution. In case of failure, an error code is returned to indicate the specific issue.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

int main() {
    size_t dim = 128;
    size_t total_base_vectors = 10000;
    size_t ny = 100;

    // Prepare query vectors of the int8 type.
    int8_t* query_vec = (int8_t*)malloc(dim * sizeof(int8_t));
    for (size_t i = 0; i < dim; i++) {
        query_vec[i] = (int8_t)(rand() % 256 - 128);
    }

    // Prepare base vectors of the int8 type.
    int8_t* base_vectors = (int8_t*)malloc(total_base_vectors * dim * sizeof(int8_t));
    for (size_t i = 0; i < total_base_vectors * dim; i++) {
        base_vectors[i] = (int8_t)(rand() % 256 - 128);
    }

    // Specify IDs of vectors for distance computation.
    int64_t* ids = (int64_t*)malloc(ny * sizeof(int64_t));
    for (size_t i = 0; i < ny; i++) {
        ids[i] = rand() % total_base_vectors;
    }

    // Allocate the distance result array (the output type is still float).
    float* distances = (float*)malloc(ny * sizeof(float));

    // Perform one-to-many inner product distance computation on vectors represented as 8-bit signed integers (int8).
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
        printf("Failed to compute the one-to-many inner product distance for vectors represented as int8. Error code: %d\n", ret);
        goto cleanup;
    }

    printf("Successfully computed the one-to-many inner product distance for vectors represented as int8\n");
    printf("First 5 results:\n");
    for (size_t i = 0; i < 5 && i < ny; i++) {
        printf("  Vector ID [%ld]: inner product = %f\n", ids[i], distances[i]);
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

**Interface Definition<a name="section172317194488"></a>**

int krl\_L2sqr\_ny\(float\* dis, const float\* x, const float\* y, size\_t ny, size\_t d, size\_t dis\_size\);

**Function<a name="section1153124784912"></a>**

Performs one-to-many Euclidean distance computation on vectors represented in float precision.

**Parameters<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="14.601460146014599%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row92301478154"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p223015479158"><a name="p223015479158"></a><a name="p223015479158"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p11230154710156"><a name="p11230154710156"></a><a name="p11230154710156"></a>float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p184912496525"><a name="p184912496525"></a><a name="p184912496525"></a>Stores the distance computation result.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p923018478155"><a name="p923018478155"></a><a name="p923018478155"></a>The size is specified by <code>dis_size</code>. The memory needs to be allocated in advance.</p>
</td>
</tr>
<tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p953215815518"><a name="p953215815518"></a><a name="p953215815518"></a>const float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p18661136253"><a name="p18661136253"></a><a name="p18661136253"></a>Query vector for distance computation.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>The vector has a dimension of <code>d</code>.</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4982142445414"><a name="p4982142445414"></a><a name="p4982142445414"></a>y</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7532158856"><a name="p7532158856"></a><a name="p7532158856"></a>const float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p36611261054"><a name="p36611261054"></a><a name="p36611261054"></a>Base vector for distance computation.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>The size is specified by <code>d</code> × <code>ny</code>.</p>
</td>
</tr>
<tr id="row103951453161513"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p14723141215409"><a name="p14723141215409"></a><a name="p14723141215409"></a>ny</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p4723181210404"><a name="p4723181210404"></a><a name="p4723181210404"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p672341218403"><a name="p672341218403"></a><a name="p672341218403"></a>Number of base vectors for distance computation.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p6723181274010"><a name="p6723181274010"></a><a name="p6723181274010"></a>[1, 2^30-1]</p>
</td>
</tr>
<tr id="row106882715416"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p46812710547"><a name="p46812710547"></a><a name="p46812710547"></a>d</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p45311183519"><a name="p45311183519"></a><a name="p45311183519"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p17661261256"><a name="p17661261256"></a><a name="p17661261256"></a>Vector dimension.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p46952755416"><a name="p46952755416"></a><a name="p46952755416"></a>[1, 65535]</p>
</td>
</tr>
<tr id="row161414323423"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p39628388417"><a name="p39628388417"></a><a name="p39628388417"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p10722125214"><a name="p10722125214"></a><a name="p10722125214"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p1762116529"><a name="p1762116529"></a><a name="p1762116529"></a>Size of the distance result array.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p154517391451"><a name="p154517391451"></a><a name="p154517391451"></a>The value is specified by <code>ny</code>.</p>
</td>
</tr>
</tbody>
</table>

**Return Values<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a><code>0</code> is returned on successful execution. In case of failure, an error code is returned to indicate the specific issue.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

int main() {
    size_t dim = 128;
    size_t ny = 1000;  // Number of base vectors

    // Prepare the query vector.
    float* query_vec = (float*)malloc(dim * sizeof(float));
    for (size_t i = 0; i < dim; i++) {
        query_vec[i] = (float)(rand() % 1000) / 1000.0f;
    }

    // Prepare the base vector (contiguous storage).
    float* base_vectors = (float*)malloc(ny * dim * sizeof(float));
    for (size_t i = 0; i < ny * dim; i++) {
        base_vectors[i] = (float)(rand() % 1000) / 1000.0f;
    }

    // Allocate the distance result array.
    float* distances = (float*)malloc(ny * sizeof(float));

    // Perform one-to-many Euclidean distance computation (to compute the distance between the query vector and all ny vectors).
    int ret = krl_L2sqr_ny(
        distances,      // Output
        query_vec, // Query vector
        base_vectors,   // Base vector (contiguous storage)
        ny,             // Number of base vectors
        dim,            // Dimension
        ny              // Length of the result array
    );

    if (ret != 0) {
        printf("Failed to compute the one-to-many Euclidean distance. Error code: %d\n", ret);
        goto cleanup;
    }

    // Find the nearest neighbor.
    float min_dist = distances[0];
    size_t min_idx = 0;
    for (size_t i = 1; i < ny; i++) {
        if (distances[i] < min_dist) {
            min_dist = distances[i];
            min_idx = i;
        }
    }

    printf("Nearest neighbor: vector index = %zu, distance = %f\n", min_idx, min_dist);

cleanup:
    free(query_vec);
    free(base_vectors);
    free(distances);

    return ret;
}
```

### krl\_L2sqr\_ny\_f16f32

**Interface Definition<a name="section172317194488"></a>**

in krl\_L2sqr\_ny\_f16f32\(float\* dis, const uint16\_t\* x, const uint16\_t\* y, size\_t ny, size\_t d, size\_t dis\_size\);

**Function<a name="section1153124784912"></a>**

Performs one-to-many Euclidean distance computation on vectors represented in fp16 precision.

**Parameters<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="14.601460146014599%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row92301478154"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p223015479158"><a name="p223015479158"></a><a name="p223015479158"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p11230154710156"><a name="p11230154710156"></a><a name="p11230154710156"></a>float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p184912496525"><a name="p184912496525"></a><a name="p184912496525"></a>Stores the distance computation result.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p923018478155"><a name="p923018478155"></a><a name="p923018478155"></a>The size is specified by <code>dis_size</code>. The memory needs to be allocated in advance.</p>
</td>
</tr>
<tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p953215815518"><a name="p953215815518"></a><a name="p953215815518"></a>const uint16_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p18661136253"><a name="p18661136253"></a><a name="p18661136253"></a>Query vector for distance computation.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>The vector has a dimension of <code>d</code>.</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4982142445414"><a name="p4982142445414"></a><a name="p4982142445414"></a>y</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7532158856"><a name="p7532158856"></a><a name="p7532158856"></a>const uint16_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p36611261054"><a name="p36611261054"></a><a name="p36611261054"></a>Base vector for distance computation.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>The size is specified by <code>d</code> × <code>ny</code>.</p>
</td>
</tr>
<tr id="row103951453161513"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p14723141215409"><a name="p14723141215409"></a><a name="p14723141215409"></a>ny</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p4723181210404"><a name="p4723181210404"></a><a name="p4723181210404"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p672341218403"><a name="p672341218403"></a><a name="p672341218403"></a>Number of base vectors for distance computation.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p6723181274010"><a name="p6723181274010"></a><a name="p6723181274010"></a>[1, 2^30-1]</p>
</td>
</tr>
<tr id="row106882715416"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p46812710547"><a name="p46812710547"></a><a name="p46812710547"></a>d</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p45311183519"><a name="p45311183519"></a><a name="p45311183519"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p17661261256"><a name="p17661261256"></a><a name="p17661261256"></a>Vector dimension.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p46952755416"><a name="p46952755416"></a><a name="p46952755416"></a>[1, 65535]</p>
</td>
</tr>
<tr id="row1922192114518"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p39628388417"><a name="p39628388417"></a><a name="p39628388417"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p10722125214"><a name="p10722125214"></a><a name="p10722125214"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p1762116529"><a name="p1762116529"></a><a name="p1762116529"></a>Size of the distance result array.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p154517391451"><a name="p154517391451"></a><a name="p154517391451"></a>The value is specified by <code>ny</code>.</p>
</td>
</tr>
</tbody>
</table>

**Return Values<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a><code>0</code> is returned on successful execution. In case of failure, an error code is returned to indicate the specific issue.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

// Auxiliary function: Convert float to fp16.
uint16_t float_to_fp16(float value);

int main() {
    size_t dim = 128;
    size_t ny = 500;

    // Prepare query vectors in fp16 format.
    uint16_t* query_vec_fp16 = (uint16_t*)malloc(dim * sizeof(uint16_t));
    for (size_t i = 0; i < dim; i++) {
        query_vec_fp16[i] = float_to_fp16((float)(rand() % 100) / 100.0f);
    }

    // Prepare base vectors in fp16 format.
    uint16_t* base_vectors_fp16 = (uint16_t*)malloc(ny * dim * sizeof(uint16_t));
    for (size_t i = 0; i < ny * dim; i++) {
        base_vectors_fp16[i] = float_to_fp16((float)(rand() % 100) / 100.0f);
    }

    // Allocate the distance result array.
    float* distances = (float*)malloc(ny * sizeof(float));

    // Perform one-to-many Euclidean distance computation on vectors represented in fp16 precision.
    int ret = krl_L2sqr_ny_f16f32(
        distances,
        query_vec_fp16,
        base_vectors_fp16,
        ny,
        dim,
        ny
    );

    if (ret != 0) {
        printf("Failed to compute the one-to-many Euclidean distance for vectors represented in fp16 precision. Error code: %d\n", ret);
        goto cleanup;
    }

    printf("Successfully computed the one-to-many Euclidean distance for vectors represented in fp16 precision. Total number of vectors: %zu\n", ny);

cleanup:
    free(query_vec_fp16);
    free(base_vectors_fp16);
    free(distances);

    return ret;
}
```

### krl\_L2sqr\_ny\_u8f32

**Interface Definition<a name="section172317194488"></a>**

void krl\_L2sqr\_ny\_u8f32\(float\* dis, const uint8\_t\* x, const uint8\_t\* y, size\_t ny, size\_t d, size\_t dis\_size\);

**Function<a name="section1153124784912"></a>**

Performs one-to-many Euclidean distance computation on vectors represented as 8-bit unsigned integers (uint8).

**Parameters<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="14.601460146014599%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row92301478154"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p223015479158"><a name="p223015479158"></a><a name="p223015479158"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p11230154710156"><a name="p11230154710156"></a><a name="p11230154710156"></a>float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p184912496525"><a name="p184912496525"></a><a name="p184912496525"></a>Stores the distance computation result.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p923018478155"><a name="p923018478155"></a><a name="p923018478155"></a>The size is specified by <code>dis_size</code>. The memory needs to be allocated in advance.</p>
</td>
</tr>
<tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p953215815518"><a name="p953215815518"></a><a name="p953215815518"></a>const uint8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p18661136253"><a name="p18661136253"></a><a name="p18661136253"></a>Query vector for distance computation.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>The vector has a dimension of <code>d</code>.</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4982142445414"><a name="p4982142445414"></a><a name="p4982142445414"></a>y</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7532158856"><a name="p7532158856"></a><a name="p7532158856"></a>const uint8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p36611261054"><a name="p36611261054"></a><a name="p36611261054"></a>Base vector for distance computation.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>The size is specified by <code>d</code> × <code>ny</code>.</p>
</td>
</tr>
<tr id="row103951453161513"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p14723141215409"><a name="p14723141215409"></a><a name="p14723141215409"></a>ny</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p4723181210404"><a name="p4723181210404"></a><a name="p4723181210404"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p672341218403"><a name="p672341218403"></a><a name="p672341218403"></a>Number of base vectors for distance computation.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p6723181274010"><a name="p6723181274010"></a><a name="p6723181274010"></a>[1, 2^30-1]</p>
</td>
</tr>
<tr id="row106882715416"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p46812710547"><a name="p46812710547"></a><a name="p46812710547"></a>d</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p45311183519"><a name="p45311183519"></a><a name="p45311183519"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p17661261256"><a name="p17661261256"></a><a name="p17661261256"></a>Vector dimension.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p46952755416"><a name="p46952755416"></a><a name="p46952755416"></a>[1, 65535]</p>
</td>
</tr>
<tr id="row882011193585"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p39628388417"><a name="p39628388417"></a><a name="p39628388417"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p10722125214"><a name="p10722125214"></a><a name="p10722125214"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p1762116529"><a name="p1762116529"></a><a name="p1762116529"></a>Size of the distance result array.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p154517391451"><a name="p154517391451"></a><a name="p154517391451"></a>The value is specified by <code>ny</code>.</p>
</td>
</tr>
</tbody>
</table>

**Return Values<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a><code>0</code> is returned on successful execution. In case of failure, an error code is returned to indicate the specific issue.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

int main() {
    size_t dim = 128;
    size_t ny = 1000;

    // Prepare query vectors of the uint8 type.
    uint8_t* query_vec = (uint8_t*)malloc(dim * sizeof(uint8_t));
    for (size_t i = 0; i < dim; i++) {
        query_vec[i] = (uint8_t)(rand() % 256);
    }

    // Prepare base vectors of the uint8 type.
    uint8_t* base_vectors = (uint8_t*)malloc(ny * dim * sizeof(uint8_t));
    for (size_t i = 0; i < ny * dim; i++) {
        base_vectors[i] = (uint8_t)(rand() % 256);
    }

    // Allocate the distance result array.
    float* distances = (float*)malloc(ny * sizeof(float));

    // Perform one-to-many Euclidean distance computation on vectors represented as 8-bit unsigned integers (uint8).
    krl_L2sqr_ny_u8f32(
        distances,
        query_vec,
        base_vectors,
        ny,
        dim,
        ny
    );

    printf ("uint8 one-to-many Euclidean distance computation completed\n");

    // Summarize results.
    float sum = 0.0f;
    for (size_t i = 0; i < ny; i++) {
        sum += distances[i];
    }
    printf ("Average distance: %f\n", sum / ny);

    free(query_vec);
    free(base_vectors);
    free(distances);

    return 0;
}
```

### krl\_L2sqr\_ny\_with\_handle

**Interface Definition<a name="section172317194488"></a>**

int krl\_L2sqr\_ny\_with\_handle\(const KRLDistanceHandle\* kdh, float\* dis, const float\* x, size\_t dis\_size, size\_t x\_size\);

**Function<a name="section1153124784912"></a>**

Performs one-to-many Euclidean distance computation on vectors represented in float precision. The base vectors and dimensions are stored in the handle.

**Parameters<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="14.601460146014599%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row92301478154"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p223015479158"><a name="p223015479158"></a><a name="p223015479158"></a>kdh</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p11230154710156"><a name="p11230154710156"></a><a name="p11230154710156"></a>const KRLDistanceHandle*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p82303471154"><a name="p82303471154"></a><a name="p82303471154"></a>Pointer to a KRLDistanceHandle instance.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p923018478155"><a name="p923018478155"></a><a name="p923018478155"></a>It cannot be null, and is initialized using krl_create_distance_handle.</p>
</td>
</tr>
<tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p953215815518"><a name="p953215815518"></a><a name="p953215815518"></a>float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p23437551435"><a name="p23437551435"></a><a name="p23437551435"></a>Stores the distance computation result.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1334317552314"><a name="p1334317552314"></a><a name="p1334317552314"></a>The size is specified by <code>dis_size</code>. The memory needs to be allocated in advance.</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p1089412431931"><a name="p1089412431931"></a><a name="p1089412431931"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p1389417431933"><a name="p1389417431933"></a><a name="p1389417431933"></a>const uint8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p28941943039"><a name="p28941943039"></a><a name="p28941943039"></a>Query vector for distance computation.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p389414311314"><a name="p389414311314"></a><a name="p389414311314"></a>The size is specified by <code>x_size</code>.</p>
</td>
</tr>
<tr id="row204111454114013"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p741115416407"><a name="p741115416407"></a><a name="p741115416407"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p11411185494014"><a name="p11411185494014"></a><a name="p11411185494014"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p54111354134020"><a name="p54111354134020"></a><a name="p54111354134020"></a>Size of the distance result array.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p64114540409"><a name="p64114540409"></a><a name="p64114540409"></a>The size is specified by <code>num_base</code> x <code>codes_num</code>, where <code>num_base</code> is the number of query vectors processed in a single batch, and <code>codes_num</code> is the number of base vectors each query vector is compared against.</p>
</td>
</tr>
<tr id="row203061171413"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p63061672410"><a name="p63061672410"></a><a name="p63061672410"></a>x_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p1306147134110"><a name="p1306147134110"></a><a name="p1306147134110"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p330613718414"><a name="p330613718414"></a><a name="p330613718414"></a>Size of the query vector array for distance computation.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1730614764116"><a name="p1730614764116"></a><a name="p1730614764116"></a>The size is specified by <code>d</code> x <code>num_base</code>, where <code>d</code> is the vector dimension.</p>
</td>
</tr>
</tbody>
</table>

**Return Values<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a><code>0</code> is returned on successful execution. In case of failure, an error code is returned to indicate the specific issue.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

int main() {
    // Parameter configuration
    size_t dim = 128;
    size_t num_base = 1;        // Number of query vectors processed in a single batch
    size_t codes_num = 1000;    // Number of base vectors each query vector is compared against.
    size_t accu_level = 3;      // fp32 precision
    size_t blocksize = 32;
    int metric_type = 1;        // Euclidean distance

    // Prepare base vectors.
    size_t codes_size = num_base * codes_num * dim * sizeof(float);
    float* base_vectors = (float*)malloc(codes_size);
    for (size_t i = 0; i < num_base * codes_num * dim; i++) {
        base_vectors[i] = (float)(rand() % 1000) / 1000.0f;
    }

    // Handle creation
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
        printf("Failed to create the handle: %d\n", ret);
        free(base_vectors);
        return -1;
    }

    // Prepare the query vector.
    size_t x_size = dim * num_base * sizeof(float);
    float* query_vec = (float*)malloc(x_size);
    for (size_t i = 0; i < dim * num_base; i++) {
        query_vec[i] = (float)(rand() % 1000) / 1000.0f;
    }

    // Allocate the result array.
    size_t dis_size = num_base * codes_num;
    float* distances = (float*)malloc(dis_size * sizeof(float));

    // Use the handle to compute the distance.
    ret = krl_L2sqr_ny_with_handle(
        kdh,
        distances,
        query_vec,
        dis_size,
        x_size / sizeof(float)
    );

    if (ret != 0) {
        printf("Distance computation failed: %d\n", ret);
        goto cleanup;
    }

    printf("Successfully computed the one-to-many Euclidean distance using the handle\n");
    printf("First 5 distance results:\n");
    for (size_t i = 0; i < 5 && i < dis_size; i++) {
        printf ("  Distance [%zu] = %f\n", i, distances[i]);
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

**Interface Definition<a name="section172317194488"></a>**

int krl\_inner\_product\_ny\(float\* dis, const float\* x, const float\* y, size\_t ny, size\_t d, size\_t dis\_size\);

**Function<a name="section1153124784912"></a>**

Performs one-to-many distance computation using inner product on vectors represented in float precision.

**Parameters<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515553%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="14.601460146014603%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="34.043404340434044%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="35.80358035803581%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row92301478154"><td class="cellrowborder" valign="top" width="15.551555155515553%" headers="mcps1.1.5.1.1 "><p id="p223015479158"><a name="p223015479158"></a><a name="p223015479158"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014603%" headers="mcps1.1.5.1.2 "><p id="p11230154710156"><a name="p11230154710156"></a><a name="p11230154710156"></a>float*</p>
</td>
<td class="cellrowborder" valign="top" width="34.043404340434044%" headers="mcps1.1.5.1.3 "><p id="p82303471154"><a name="p82303471154"></a><a name="p82303471154"></a>Stores the distance computation result.</p>
</td>
<td class="cellrowborder" valign="top" width="35.80358035803581%" headers="mcps1.1.5.1.4 "><p id="p923018478155"><a name="p923018478155"></a><a name="p923018478155"></a>The size is specified by <code>dis_size</code>. The memory needs to be allocated in advance.</p>
</td>
</tr>
<tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515553%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014603%" headers="mcps1.1.5.1.2 "><p id="p953215815518"><a name="p953215815518"></a><a name="p953215815518"></a>const float*</p>
</td>
<td class="cellrowborder" valign="top" width="34.043404340434044%" headers="mcps1.1.5.1.3 "><p id="p18661136253"><a name="p18661136253"></a><a name="p18661136253"></a>Query vector for distance computation.</p>
</td>
<td class="cellrowborder" valign="top" width="35.80358035803581%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>The vector has a dimension of <code>d</code>.</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515553%" headers="mcps1.1.5.1.1 "><p id="p4982142445414"><a name="p4982142445414"></a><a name="p4982142445414"></a>y</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014603%" headers="mcps1.1.5.1.2 "><p id="p7532158856"><a name="p7532158856"></a><a name="p7532158856"></a>const float*</p>
</td>
<td class="cellrowborder" valign="top" width="34.043404340434044%" headers="mcps1.1.5.1.3 "><p id="p36611261054"><a name="p36611261054"></a><a name="p36611261054"></a>Base vector for distance computation.</p>
</td>
<td class="cellrowborder" valign="top" width="35.80358035803581%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>The size is specified by <code>d</code> × <code>ny</code>.</p>
</td>
</tr>
<tr id="row103951453161513"><td class="cellrowborder" valign="top" width="15.551555155515553%" headers="mcps1.1.5.1.1 "><p id="p14723141215409"><a name="p14723141215409"></a><a name="p14723141215409"></a>ny</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014603%" headers="mcps1.1.5.1.2 "><p id="p4723181210404"><a name="p4723181210404"></a><a name="p4723181210404"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="34.043404340434044%" headers="mcps1.1.5.1.3 "><p id="p672341218403"><a name="p672341218403"></a><a name="p672341218403"></a>Number of base vectors for distance computation.</p>
</td>
<td class="cellrowborder" valign="top" width="35.80358035803581%" headers="mcps1.1.5.1.4 "><p id="p6723181274010"><a name="p6723181274010"></a><a name="p6723181274010"></a>[1, 2^30-1]</p>
</td>
</tr>
<tr id="row106882715416"><td class="cellrowborder" valign="top" width="15.551555155515553%" headers="mcps1.1.5.1.1 "><p id="p46812710547"><a name="p46812710547"></a><a name="p46812710547"></a>d</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014603%" headers="mcps1.1.5.1.2 "><p id="p45311183519"><a name="p45311183519"></a><a name="p45311183519"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="34.043404340434044%" headers="mcps1.1.5.1.3 "><p id="p17661261256"><a name="p17661261256"></a><a name="p17661261256"></a>Vector dimension.</p>
</td>
<td class="cellrowborder" valign="top" width="35.80358035803581%" headers="mcps1.1.5.1.4 "><p id="p46952755416"><a name="p46952755416"></a><a name="p46952755416"></a>[1, 65535]</p>
</td>
</tr>
<tr id="row1069011157013"><td class="cellrowborder" valign="top" width="15.551555155515553%" headers="mcps1.1.5.1.1 "><p id="p39628388417"><a name="p39628388417"></a><a name="p39628388417"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014603%" headers="mcps1.1.5.1.2 "><p id="p10722125214"><a name="p10722125214"></a><a name="p10722125214"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="34.043404340434044%" headers="mcps1.1.5.1.3 "><p id="p1762116529"><a name="p1762116529"></a><a name="p1762116529"></a>Size of the distance result array.</p>
</td>
<td class="cellrowborder" valign="top" width="35.80358035803581%" headers="mcps1.1.5.1.4 "><p id="p154517391451"><a name="p154517391451"></a><a name="p154517391451"></a>The value is specified by <code>ny</code>.</p>
</td>
</tr>
</tbody>
</table>

**Return Values<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a><code>0</code> is returned on successful execution. In case of failure, an error code is returned to indicate the specific issue.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c
#include <stdio.h>
#include <stdlib.h>
#include <math.h>
#include "krl.h"

int main() {
    size_t dim = 128;
    size_t ny = 1000;

    // Prepare the query vector.
    float* query_vec = (float*)malloc(dim * sizeof(float));
    for (size_t i = 0; i < dim; i++) {
        query_vec[i] = (float)(rand() % 100) / 100.0f;
    }

    // Prepare the base vector.
    float* base_vectors = (float*)malloc(ny * dim * sizeof(float));
    for (size_t i = 0; i < ny * dim; i++) {
        base_vectors[i] = (float)(rand() % 100) / 100.0f;
    }

    // Allocate the distance result array.
    float* distances = (float*)malloc(ny * sizeof(float));

    // Perform one-to-many inner product distance computation.
    int ret = krl_inner_product_ny(
        distances,
        query_vec,
        base_vectors,
        ny,
        dim,
        ny
    );

    if (ret != 0) {
        printf("Failed to compute the one-to-many inner product distance. Error code: %d\n", ret);
        goto cleanup;
    }

    // Determine the maximum inner product (most similar).
    float max_ip = distances[0];
    size_t max_idx = 0;
    for (size_t i = 1; i < ny; i++) {
        if (distances[i] > max_ip) {
            max_ip = distances[i];
            max_idx = i;
        }
    }

    printf("Most similar vector: index = %zu, inner product = %f\n", max_idx, max_ip);

cleanup:
    free(query_vec);
    free(base_vectors);
    free(distances);

    return ret;
}
```

### krl\_inner\_product\_ny\_f16f32

**Interface Definition<a name="section172317194488"></a>**

int krl\_inner\_product\_ny\_f16f32\(float\* dis, const uint16\_t\* x, const uint16\_t\* y, size\_t ny, size\_t d, size\_t dis\_size\);

**Function<a name="section1153124784912"></a>**

Performs one-to-many distance computation using inner product on vectors represented in fp16 precision.

**Parameters<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="14.601460146014599%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="33.97339733973397%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="35.873587358735875%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row92301478154"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p223015479158"><a name="p223015479158"></a><a name="p223015479158"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p11230154710156"><a name="p11230154710156"></a><a name="p11230154710156"></a>float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.97339733973397%" headers="mcps1.1.5.1.3 "><p id="p82303471154"><a name="p82303471154"></a><a name="p82303471154"></a>Stores the distance computation result.</p>
</td>
<td class="cellrowborder" valign="top" width="35.873587358735875%" headers="mcps1.1.5.1.4 "><p id="p923018478155"><a name="p923018478155"></a><a name="p923018478155"></a>The size is specified by <code>dis_size</code>. The memory needs to be allocated in advance.</p>
</td>
</tr>
<tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p953215815518"><a name="p953215815518"></a><a name="p953215815518"></a>const uint16_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.97339733973397%" headers="mcps1.1.5.1.3 "><p id="p18661136253"><a name="p18661136253"></a><a name="p18661136253"></a>Query vector for distance computation.</p>
</td>
<td class="cellrowborder" valign="top" width="35.873587358735875%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>The vector has a dimension of <code>d</code>.</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4982142445414"><a name="p4982142445414"></a><a name="p4982142445414"></a>y</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7532158856"><a name="p7532158856"></a><a name="p7532158856"></a>const uint16_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.97339733973397%" headers="mcps1.1.5.1.3 "><p id="p36611261054"><a name="p36611261054"></a><a name="p36611261054"></a>Base vector for distance computation.</p>
</td>
<td class="cellrowborder" valign="top" width="35.873587358735875%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>The size is specified by <code>d</code> × <code>ny</code>.</p>
</td>
</tr>
<tr id="row103951453161513"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p14723141215409"><a name="p14723141215409"></a><a name="p14723141215409"></a>ny</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p4723181210404"><a name="p4723181210404"></a><a name="p4723181210404"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.97339733973397%" headers="mcps1.1.5.1.3 "><p id="p672341218403"><a name="p672341218403"></a><a name="p672341218403"></a>Number of base vectors for distance computation.</p>
</td>
<td class="cellrowborder" valign="top" width="35.873587358735875%" headers="mcps1.1.5.1.4 "><p id="p6723181274010"><a name="p6723181274010"></a><a name="p6723181274010"></a>[1, 2^30-1]</p>
</td>
</tr>
<tr id="row106882715416"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p46812710547"><a name="p46812710547"></a><a name="p46812710547"></a>d</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p45311183519"><a name="p45311183519"></a><a name="p45311183519"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.97339733973397%" headers="mcps1.1.5.1.3 "><p id="p17661261256"><a name="p17661261256"></a><a name="p17661261256"></a>Vector dimension.</p>
</td>
<td class="cellrowborder" valign="top" width="35.873587358735875%" headers="mcps1.1.5.1.4 "><p id="p46952755416"><a name="p46952755416"></a><a name="p46952755416"></a>[1, 65535]</p>
</td>
</tr>
<tr id="row536922710219"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p39628388417"><a name="p39628388417"></a><a name="p39628388417"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p10722125214"><a name="p10722125214"></a><a name="p10722125214"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.97339733973397%" headers="mcps1.1.5.1.3 "><p id="p1762116529"><a name="p1762116529"></a><a name="p1762116529"></a>Size of the distance result array.</p>
</td>
<td class="cellrowborder" valign="top" width="35.873587358735875%" headers="mcps1.1.5.1.4 "><p id="p154517391451"><a name="p154517391451"></a><a name="p154517391451"></a>The value is specified by <code>ny</code>.</p>
</td>
</tr>
</tbody>
</table>

**Return Values<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a><code>0</code> is returned on successful execution. In case of failure, an error code is returned to indicate the specific issue.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

// Auxiliary function: Convert float to fp16.
uint16_t float_to_fp16(float value);

int main() {
    size_t dim = 256;
    size_t ny = 500;

    // Prepare query vectors in fp16 format.
    uint16_t* query_vec_fp16 = (uint16_t*)malloc(dim * sizeof(uint16_t));
    for (size_t i = 0; i < dim; i++) {
        query_vec_fp16[i] = float_to_fp16(0.5f);
    }

    // Prepare base vectors in fp16 format.
    uint16_t* base_vectors_fp16 = (uint16_t*)malloc(ny * dim * sizeof(uint16_t));
    for (size_t i = 0; i < ny * dim; i++) {
        base_vectors_fp16[i] = float_to_fp16((float)(rand() % 100) / 100.0f);
    }

    // Allocate the distance result array.
    float* distances = (float*)malloc(ny * sizeof(float));

    // Perform one-to-many inner product distance computation on vectors represented in fp16 precision..
    int ret = krl_inner_product_ny_f16f32(
        distances,
        query_vec_fp16,
        base_vectors_fp16,
        ny,
        dim,
        ny
    );

    if (ret != 0) {
        printf("Failed to compute the one-to-many inner product distance on vectors represented in fp16 precision. Error code: %d\n", ret);
        goto cleanup;
    }

    printf("Successfully computed the one-to-many inner product distance for vectors represented in fp16 precision.\n");

cleanup:
    free(query_vec_fp16);
    free(base_vectors_fp16);
    free(distances);

    return ret;
}
```

### krl\_inner\_product\_ny\_s8f32

**Interface Definition <a name="section172317194488"></a>**

int krl\_inner\_product\_ny\_s8f32\(float\* dis, const int8\_t\* x, const int8\_t\* y, size\_t ny, size\_t d, size\_t dis\_size\);

**Function<a name="section1153124784912"></a>**

Performs one-to-many distance computation using inner product on vectors represented as 8-bit signed integers (int8).

**Parameters<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="14.601460146014599%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row92301478154"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p223015479158"><a name="p223015479158"></a><a name="p223015479158"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p11230154710156"><a name="p11230154710156"></a><a name="p11230154710156"></a>float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p184912496525"><a name="p184912496525"></a><a name="p184912496525"></a>Stores the distance computation result.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p923018478155"><a name="p923018478155"></a><a name="p923018478155"></a>The size is specified by <code>dis_size</code>. The memory needs to be allocated in advance.</p>
</td>
</tr>
<tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p953215815518"><a name="p953215815518"></a><a name="p953215815518"></a>const int8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p18661136253"><a name="p18661136253"></a><a name="p18661136253"></a>Query vector for distance computation.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>The vector has a dimension of <code>d</code>.</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4982142445414"><a name="p4982142445414"></a><a name="p4982142445414"></a>y</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7532158856"><a name="p7532158856"></a><a name="p7532158856"></a>const int8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p36611261054"><a name="p36611261054"></a><a name="p36611261054"></a>Base vector for distance computation.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>The size is specified by <code>d</code> × <code>ny</code>.</p>
</td>
</tr>
<tr id="row103951453161513"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p14723141215409"><a name="p14723141215409"></a><a name="p14723141215409"></a>ny</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p4723181210404"><a name="p4723181210404"></a><a name="p4723181210404"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p672341218403"><a name="p672341218403"></a><a name="p672341218403"></a>Number of base vectors for distance computation.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p6723181274010"><a name="p6723181274010"></a><a name="p6723181274010"></a>[1, 2^30-1]</p>
</td>
</tr>
<tr id="row106882715416"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p46812710547"><a name="p46812710547"></a><a name="p46812710547"></a>d</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p45311183519"><a name="p45311183519"></a><a name="p45311183519"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p17661261256"><a name="p17661261256"></a><a name="p17661261256"></a>Vector dimension.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p46952755416"><a name="p46952755416"></a><a name="p46952755416"></a>[1, 65535]</p>
</td>
</tr>
<tr id="row1491157243"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p39628388417"><a name="p39628388417"></a><a name="p39628388417"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p10722125214"><a name="p10722125214"></a><a name="p10722125214"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p1762116529"><a name="p1762116529"></a><a name="p1762116529"></a>Size of the distance result array.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p154517391451"><a name="p154517391451"></a><a name="p154517391451"></a>The value is specified by <code>ny</code>.</p>
</td>
</tr>
</tbody>
</table>

**Return Values<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a><code>0</code> is returned on successful execution. In case of failure, an error code is returned to indicate the specific issue.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

int main() {
    size_t dim = 128;
    size_t ny = 1000;

    // Prepare query vectors of the int8 type.
    int8_t* query_vec = (int8_t*)malloc(dim * sizeof(int8_t));
    for (size_t i = 0; i < dim; i++) {
        query_vec[i] = (int8_t)(rand() % 256 - 128);
    }

    // Prepare base vectors of the int8 type.
    int8_t* base_vectors = (int8_t*)malloc(ny * dim * sizeof(int8_t));
    for (size_t i = 0; i < ny * dim; i++) {
        base_vectors[i] = (int8_t)(rand() % 256 - 128);
    }

    // Allocate the distance result array.
    float* distances = (float*)malloc(ny * sizeof(float));

    // Perform one-to-many inner product distance computation on vectors represented as int8.
    int ret = krl_inner_product_ny_s8f32(
        distances,
        query_vec,
        base_vectors,
        ny,
        dim,
        ny
    );

    if (ret != 0) {
        printf("Failed to compute the one-to-many inner product distance for vectors represented as int8. Error code: %d\n", ret);
        goto cleanup;
    }

    printf("Successfully computed the one-to-many inner product distance for vectors represented as int8\n");

    // Determine the top 3.
    printf("Top-3 maximum inner product values:\n");
    for (int k = 0; k < 3; k++) {
        float max_val = -1e30f;
        size_t max_idx = 0;
        for (size_t i = 0; i < ny; i++) {
            if (distances[i] > max_val) {
                max_val = distances[i];
                max_idx = i;
            }
        }
        printf("Rank %d: index = %zu, inner product = %f\n", k + 1, max_idx, max_val);
        distances[max_idx] = -1e30f; // Mark as selected.
    }

cleanup:
    free(query_vec);
    free(base_vectors);
    free(distances);

    return ret;
}
```

### krl\_inner\_product\_ny\_with\_handle

**Interface Definition <a name="section172317194488"></a>**

int krl\_inner\_product\_ny\_with\_handle\(const KRLDistanceHandle\* krl\_distance\_handle, float\* dis, const float\* x, size\_t dis\_size, size\_t x\_size\);

**Function<a name="section1153124784912"></a>**

Performs one-to-many distance computation using inner product on vectors represented in float precision. The base vectors and dimensions are stored in the handle.

**Parameters<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="14.601460146014599%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row92301478154"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p223015479158"><a name="p223015479158"></a><a name="p223015479158"></a>kdh</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p11230154710156"><a name="p11230154710156"></a><a name="p11230154710156"></a>const KRLDistanceHandle*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p82303471154"><a name="p82303471154"></a><a name="p82303471154"></a>Pointer to a KRLDistanceHandle instance.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p923018478155"><a name="p923018478155"></a><a name="p923018478155"></a>It cannot be null, and is initialized using krl_create_distance_handle.</p>
</td>
</tr>
<tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p953215815518"><a name="p953215815518"></a><a name="p953215815518"></a>float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p23437551435"><a name="p23437551435"></a><a name="p23437551435"></a>Stores the distance computation result.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1334317552314"><a name="p1334317552314"></a><a name="p1334317552314"></a>The size is specified by <code>dis_size</code>. The memory needs to be allocated in advance.</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p1089412431931"><a name="p1089412431931"></a><a name="p1089412431931"></a>x</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p1389417431933"><a name="p1389417431933"></a><a name="p1389417431933"></a>const uint8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p28941943039"><a name="p28941943039"></a><a name="p28941943039"></a>Query vector for distance computation.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p389414311314"><a name="p389414311314"></a><a name="p389414311314"></a>The size is specified by <code>x_size</code>.</p>
</td>
</tr>
<tr id="row416975034615"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p741115416407"><a name="p741115416407"></a><a name="p741115416407"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p11411185494014"><a name="p11411185494014"></a><a name="p11411185494014"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p54111354134020"><a name="p54111354134020"></a><a name="p54111354134020"></a>Size of the distance result array.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p116975012466"><a name="p116975012466"></a><a name="p116975012466"></a>The size is specified by <code>num_base</code> x <code>codes_num</code>, where <code>num_base</code> is the number of query vectors processed in a single batch, and <code>codes_num</code> is the number of base vectors each query vector is compared against.</p>
</td>
</tr>
<tr id="row17378115284614"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p63061672410"><a name="p63061672410"></a><a name="p63061672410"></a>x_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p1306147134110"><a name="p1306147134110"></a><a name="p1306147134110"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p330613718414"><a name="p330613718414"></a><a name="p330613718414"></a>Size of the query vector array for distance computation.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p10378252194615"><a name="p10378252194615"></a><a name="p10378252194615"></a>The size is specified by <code>d</code> x <code>num_base</code>, where <code>d</code> is the vector dimension.</p>
</td>
</tr>
</tbody>
</table>

**Return Values<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a><code>0</code> is returned on successful execution. In case of failure, an error code is returned to indicate the specific issue.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

int main() {
    // Parameter configuration
    size_t dim = 128;
    size_t num_base = 1;
    size_t codes_num = 1000;
    size_t accu_level = 3;
    size_t blocksize = 32;
    int metric_type = 0;  // Inner product distance

    // Prepare the base vectors.
    size_t codes_size = num_base * codes_num * dim * sizeof(float);
    float* base_vectors = (float*)malloc(codes_size);
    for (size_t i = 0; i < num_base * codes_num * dim; i++) {
        base_vectors[i] = (float)(rand() % 100) / 100.0f;
    }

    // Create a handle (using the inner product distance).
    KRLDistanceHandle* kdh = NULL;
    int ret = krl_create_distance_handle(
        &kdh,
        accu_level,
        blocksize,
        codes_num,
        dim,
        num_base,
        metric_type,  // 0 indicates the inner product distance.
        (const uint8_t*)base_vectors,
        codes_size
    );

    if (ret != 0) {
        printf("Failed to create the handle: %d\n", ret);
        free(base_vectors);
        return -1;
    }

    // Prepare the query vectors.
    size_t x_size = dim * num_base;
    float* query_vec = (float*)malloc(x_size * sizeof(float));
    for (size_t i = 0; i < x_size; i++) {
        query_vec[i] = (float)(rand() % 100) / 100.0f;
    }

    // Allocate the result array.
    size_t dis_size = num_base * codes_num;
    float* distances = (float*)malloc(dis_size * sizeof(float));

    // Use the handle to compute the inner product distance.
    ret = krl_inner_product_ny_with_handle(
        kdh,
        distances,
        query_vec,
        dis_size,
        x_size
    );

    if (ret != 0) {
        printf("Failed to compute the inner product distance: %d\n", ret);
        goto cleanup;
    }

    printf("Successfully computed the one-to-many inner product distance using the handle\n");

    // Determine the maximum inner product value.
    float max_ip = distances[0];
    size_t max_idx = 0;
    for (size_t i = 1; i < dis_size; i++) {
        if (distances[i] > max_ip) {
            max_ip = distances[i];
            max_idx = i;
        }
    }
    printf("Most similar vector: index = %zu, inner product = %f\n", max_idx, max_ip);

cleanup:
    krl_clean_distance_handle(&kdh);
    free(base_vectors);
    free(query_vec);
    free(distances);

    return ret;
}
```

## 8-bit Table Lookup-based Accumulation Interfaces

### krl\_table\_lookup\_8b\_f32

**Interface Definition<a name="section172317194488"></a>**

int krl\_table\_lookup\_8b\_f32\(size\_t nsq, size\_t ncode, const uint8\_t\* codes, const float\* sim\_table, float\* distance, float dis0, size\_t codes\_size, size\_t sim\_table\_size, size\_t dis\_size\);

**Function<a name="section1153124784912"></a>**

Obtains distance values from the float-type LUT using 8-bit indexes, accumulates the distance values, adds `dis0` to the result after accumulation, and stores the final result in `distance`.

**Parameters<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="14.601460146014599%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row92301478154"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p223015479158"><a name="p223015479158"></a><a name="p223015479158"></a>nsq</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p11230154710156"><a name="p11230154710156"></a><a name="p11230154710156"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p82303471154"><a name="p82303471154"></a><a name="p82303471154"></a>Number of subspaces.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p923018478155"><a name="p923018478155"></a><a name="p923018478155"></a>[1, 65535]</p>
</td>
</tr>
<tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>ncode</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p953215815518"><a name="p953215815518"></a><a name="p953215815518"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p18661136253"><a name="p18661136253"></a><a name="p18661136253"></a>Total number of base vectors.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>[1, 2^30-1]</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4982142445414"><a name="p4982142445414"></a><a name="p4982142445414"></a>codes</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7532158856"><a name="p7532158856"></a><a name="p7532158856"></a>const uint8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p36611261054"><a name="p36611261054"></a><a name="p36611261054"></a>Codebook, which stores indexes of base vectors.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>The size is specified by <code>codes_size</code>.</p>
</td>
</tr>
<tr id="row103951453161513"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p14723141215409"><a name="p14723141215409"></a><a name="p14723141215409"></a>sim_table</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p4723181210404"><a name="p4723181210404"></a><a name="p4723181210404"></a>const float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p718413012396"><a name="p718413012396"></a><a name="p718413012396"></a>Similarity LUT, which stores the distance between per-dimension query vector and all centroids.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p6723181274010"><a name="p6723181274010"></a><a name="p6723181274010"></a>The size is specified by <code>sim_table_size</code>.</p>
</td>
</tr>
<tr id="row106882715416"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p46812710547"><a name="p46812710547"></a><a name="p46812710547"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p45311183519"><a name="p45311183519"></a><a name="p45311183519"></a>float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p17661261256"><a name="p17661261256"></a><a name="p17661261256"></a>Stores the distance computation result.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p57801052141013"><a name="p57801052141013"></a><a name="p57801052141013"></a>The size is specified by <code>dis_size</code>. The memory needs to be allocated in advance.</p>
</td>
</tr>
<tr id="row1875218456372"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p275311453374"><a name="p275311453374"></a><a name="p275311453374"></a>dis0</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7753045173714"><a name="p7753045173714"></a><a name="p7753045173714"></a>float</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p17531445103716"><a name="p17531445103716"></a><a name="p17531445103716"></a>Initial distance.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p69179904614"><a name="p69179904614"></a><a name="p69179904614"></a>Floating point number.</p>
</td>
</tr>
<tr id="row9742043764"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p137414311617"><a name="p137414311617"></a><a name="p137414311617"></a>codes_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p06662231878"><a name="p06662231878"></a><a name="p06662231878"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p16744431269"><a name="p16744431269"></a><a name="p16744431269"></a>Length of the codebook array.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p127494317611"><a name="p127494317611"></a><a name="p127494317611"></a><code>nsq</code> x <code>ncode</code></p>
</td>
</tr>
<tr id="row411920559612"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p7119655861"><a name="p7119655861"></a><a name="p7119655861"></a>sim_table_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p6403112617719"><a name="p6403112617719"></a><a name="p6403112617719"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p311925516613"><a name="p311925516613"></a><a name="p311925516613"></a>Length of the similarity LUT array.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p81191255064"><a name="p81191255064"></a><a name="p81191255064"></a><code>nsq</code> x 256</p>
</td>
</tr>
<tr id="row2533196472"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p1753316619720"><a name="p1753316619720"></a><a name="p1753316619720"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p64039264714"><a name="p64039264714"></a><a name="p64039264714"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p54111354134020"><a name="p54111354134020"></a><a name="p54111354134020"></a>Size of the distance result array.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p175331661478"><a name="p175331661478"></a><a name="p175331661478"></a>The size is specified by <code>ncode</code>.</p>
</td>
</tr>
</tbody>
</table>

**Return Values<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a><code>0</code> is returned on successful execution. In case of failure, an error code is returned to indicate the specific issue.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

int main() {
    // Product quantization (PQ) parameter configuration
    size_t nsq = 32;        // Number of subspaces (a vector is divided into 32 subspaces)
    size_t ncode = 10000; // Total number of base vectors
    size_t ksub = 256; // Number of centroids per subspace (8-bit index, up to 256 centroids)

    // Prepare the codebook (codes).
    // Each base vector has nsq indexes, and each index points to a centroid in the corresponding subspace.
    size_t codes_size = nsq * ncode;
    uint8_t* codes = (uint8_t*)malloc(codes_size * sizeof(uint8_t));
    
    // Simulated codebook data (obtained through PQ training in actual use)
    for (size_t i = 0; i < codes_size; i++) {
        codes[i] = (uint8_t)(rand() % ksub);
    }

    // Prepare the similarity LUT (sim_table).
    // Stores the distances between the query vector and all centroids in each subspace.
    // Dimensions: nsq x ksub
    size_t sim_table_size = nsq * ksub;
    float* sim_table = (float*)malloc(sim_table_size * sizeof(float));
    
    // Simulated similarity LUT data (In actual use, distances between the query vector and centroids must be computed.)
    for (size_t i = 0; i < sim_table_size; i++) {
        sim_table[i] = (float)(rand() % 1000) / 100.0f;
    }

    // Allocate the distance result array.
    float* distances = (float*)malloc(ncode * sizeof(float));

    // Perform accumulation based on 8-bit table lookup.
    float dis0 = 0.0f;  // Initial distance
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
        printf("Failed to perform accumulation based on 8-bit table lookup. Error code: %d\n", ret);
        goto cleanup;
    }

    printf("Successfully performed accumulation based on 8-bit table lookup\n");

    // Determine the nearest neighbor.
    float min_dist = distances[0];
    size_t min_idx = 0;
    for (size_t i = 1; i < ncode; i++) {
        if (distances[i] < min_dist) {
            min_dist = distances[i];
            min_idx = i;
        }
    }
    printf("Nearest neighbor: index = %zu, PQ distance = %f\n", min_idx, min_dist);

cleanup:
    free(codes);
    free(sim_table);
    free(distances);

    return ret;
}
```

### krl\_table\_lookup\_8b\_f32\_by\_idx

**Interface Definition<a name="section172317194488"></a>**

int krl\_table\_lookup\_8b\_f32\_by\_idx\(size\_t nsq, size\_t ncode, const uint8\_t\* codes, const float\* sim\_table, float\* dis, float dis0, const size\_t\* idx, size\_t codes\_size, size\_t sim\_table\_size, size\_t dis\_size\);

**Function<a name="section1153124784912"></a>**

Obtains distance values from the float-type LUT using 8-bit indexes, accumulates the distance values, adds `dis0` to the result after accumulation, and stores the final result in `distance`. Only the base vectors whose IDs are in the <code>idx</code> array are used for computation.

**Parameters<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="14.601460146014599%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row92301478154"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p223015479158"><a name="p223015479158"></a><a name="p223015479158"></a>nsq</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p11230154710156"><a name="p11230154710156"></a><a name="p11230154710156"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p82303471154"><a name="p82303471154"></a><a name="p82303471154"></a>Number of subspaces.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p923018478155"><a name="p923018478155"></a><a name="p923018478155"></a>[1, 65535]</p>
</td>
</tr>
<tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>ncode</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p953215815518"><a name="p953215815518"></a><a name="p953215815518"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p18661136253"><a name="p18661136253"></a><a name="p18661136253"></a>Total number of base vectors.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>[1, 2^30-1]</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4982142445414"><a name="p4982142445414"></a><a name="p4982142445414"></a>codes</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7532158856"><a name="p7532158856"></a><a name="p7532158856"></a>const uint8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p992551816390"><a name="p992551816390"></a><a name="p992551816390"></a>Codebook, which stores indexes of base vectors.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>The size is specified by <code>codes_size</code>.</p>
</td>
</tr>
<tr id="row103951453161513"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p14723141215409"><a name="p14723141215409"></a><a name="p14723141215409"></a>sim_table</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p4723181210404"><a name="p4723181210404"></a><a name="p4723181210404"></a>const float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p710155233915"><a name="p710155233915"></a><a name="p710155233915"></a>Similarity LUT, which stores the distance between per-dimension query vector and all centroids.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p6723181274010"><a name="p6723181274010"></a><a name="p6723181274010"></a>The size is specified by <code>sim_table_size</code>.</p>
</td>
</tr>
<tr id="row106882715416"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p46812710547"><a name="p46812710547"></a><a name="p46812710547"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p45311183519"><a name="p45311183519"></a><a name="p45311183519"></a>float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p17661261256"><a name="p17661261256"></a><a name="p17661261256"></a>Stores the distance computation result.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p57801052141013"><a name="p57801052141013"></a><a name="p57801052141013"></a>The size is specified by <code>dis_size</code>. The memory needs to be allocated in advance.</p>
</td>
</tr>
<tr id="row1875218456372"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p275311453374"><a name="p275311453374"></a><a name="p275311453374"></a>dis0</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7753045173714"><a name="p7753045173714"></a><a name="p7753045173714"></a>float</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p17531445103716"><a name="p17531445103716"></a><a name="p17531445103716"></a>Initial distance.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p69179904614"><a name="p69179904614"></a><a name="p69179904614"></a>Floating point number.</p>
</td>
</tr>
<tr id="row575095414710"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p075085444712"><a name="p075085444712"></a><a name="p075085444712"></a>idx</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p19750155420479"><a name="p19750155420479"></a><a name="p19750155420479"></a>const size_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p875015418477"><a name="p875015418477"></a><a name="p875015418477"></a>Array of IDs of base vectors used for computation.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p375065415472"><a name="p375065415472"></a><a name="p375065415472"></a>The size is specified by <code>ncode</code>. The IDs need to be arranged in ascending order.</p>
</td>
</tr>
<tr id="row14701171851717"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p137414311617"><a name="p137414311617"></a><a name="p137414311617"></a>codes_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p06662231878"><a name="p06662231878"></a><a name="p06662231878"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p16744431269"><a name="p16744431269"></a><a name="p16744431269"></a>Length of the codebook array.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p127494317611"><a name="p127494317611"></a><a name="p127494317611"></a><code>nsq</code> x <code>ncode</code></p>
</td>
</tr>
<tr id="row37001918161712"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p7119655861"><a name="p7119655861"></a><a name="p7119655861"></a>sim_table_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p6403112617719"><a name="p6403112617719"></a><a name="p6403112617719"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p311925516613"><a name="p311925516613"></a><a name="p311925516613"></a>Length of the similarity LUT array.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p81191255064"><a name="p81191255064"></a><a name="p81191255064"></a><code>nsq</code> x 256</p>
</td>
</tr>
<tr id="row370081812173"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p1753316619720"><a name="p1753316619720"></a><a name="p1753316619720"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p64039264714"><a name="p64039264714"></a><a name="p64039264714"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p54111354134020"><a name="p54111354134020"></a><a name="p54111354134020"></a>Size of the distance result array.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p175331661478"><a name="p175331661478"></a><a name="p175331661478"></a>The size is specified by <code>ncode</code>.</p>
</td>
</tr>
</tbody>
</table>

**Return Values<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a><code>0</code> is returned on successful execution. In case of failure, an error code is returned to indicate the specific issue.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

int main() {
    // PQ parameter configuration
    size_t nsq = 32;
    size_t total_vectors = 100000;  // Total number of base vectors
    size_t ncode = 1000;            // Number of vectors used for computation (after filtering)
    size_t ksub = 256;

    // Prepare the codebook.
    size_t full_codes_size = nsq * total_vectors;
    uint8_t* codes = (uint8_t*)malloc(full_codes_size * sizeof(uint8_t));
    for (size_t i = 0; i < full_codes_size; i++) {
        codes[i] = (uint8_t)(rand() % ksub);
    }

    // Prepare the similarity LUT.
    size_t sim_table_size = nsq * ksub;
    float* sim_table = (float*)malloc(sim_table_size * sizeof(float));
    for (size_t i = 0; i < sim_table_size; i++) {
        sim_table[i] = (float)(rand() % 1000) / 100.0f;
    }

    // Prepare the filtered ID array (must be in ascending order).
    size_t* idx = (size_t*)malloc(ncode * sizeof(size_t));
    for (size_t i = 0; i < ncode; i++) {
        idx[i] = i * 100; // Select IDs: 0, 100, 200, ... (in ascending order)
    }

    // Allocate the distance result array.
    float* distances = (float*)malloc(ncode * sizeof(float));

    // Perform accumulation based on 8-bit table lookup with indexes.
    float dis0 = 0.0f;
    int ret = krl_table_lookup_8b_f32_by_idx(
        nsq,
        ncode,
        codes,
        sim_table,
        distances,
        dis0,
        idx,
        nsq * ncode, // Compute only the selected vectors.
        sim_table_size,
        ncode
    );

    if (ret != 0) {
        printf("Failed to perform accumulation based on 8-bit table lookup with indexes. Error code: %d\n", ret);
        goto cleanup;
    }

    printf("Successfully performed accumulation based on 8-bit table lookup with indexes\n");
    printf("PQ distance computed for %zu vectors\n", ncode);

    // Output the first five results.
    printf("First 5 results:\n");
    for (size_t i = 0; i < 5 && i < ncode; i++) {
        printf ("  Vector ID[%zu]: PQ distance = %f\n", idx[i], distances[i]);
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

**Interface Definition<a name="section172317194488"></a>**

int krl\_table\_lookup\_8b\_f32\_with\_handle\(KRLLUT8bHandle\* klh, size\_t dim, size\_t ncode, const uint8\_t\* codes, const float\* sim\_table, float dis0, size\_t codes\_size, size\_t sim\_table\_size\);

**Function<a name="section1153124784912"></a>**

Obtains distance values from the float-type LUT using 8-bit indexes, accumulates the distance values, adds `dis0` to the result after accumulation, and stores the final result in `distance`. The <code>idx</code> and <code>distance</code> arrays are contained in the KRLLUT8bHandle instance. Only the base vectors whose IDs are in the <code>idx</code> array are used for computation.

**Parameters<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="14.601460146014599%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="33.953395339533955%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="35.873587358735875%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row92301478154"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p223015479158"><a name="p223015479158"></a><a name="p223015479158"></a>klh</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p11230154710156"><a name="p11230154710156"></a><a name="p11230154710156"></a>KRLLUT8bHandle*</p>
</td>
<td class="cellrowborder" valign="top" width="33.953395339533955%" headers="mcps1.1.5.1.3 "><p id="p82303471154"><a name="p82303471154"></a><a name="p82303471154"></a>Pointer to a KRLLUT8bHandle instance.</p>
</td>
<td class="cellrowborder" valign="top" width="35.8935893589359%" headers="mcps1.1.5.1.4 "><p id="p923018478155"><a name="p923018478155"></a><a name="p923018478155"></a>It cannot be null, and is initialized using krl_create_LUT8b_handle.</p>
</td>
</tr>
<tr id="row166241441532"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p262494414531"><a name="p262494414531"></a><a name="p262494414531"></a>dim</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p126241544125310"><a name="p126241544125310"></a><a name="p126241544125310"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.953395339533955%" headers="mcps1.1.5.1.3 "><p id="p1562414447536"><a name="p1562414447536"></a><a name="p1562414447536"></a>Vector dimension.</p>
</td>
<td class="cellrowborder" valign="top" width="35.8935893589359%" headers="mcps1.1.5.1.4 "><p id="p19624744195313"><a name="p19624744195313"></a><a name="p19624744195313"></a>[1, 65535]</p>
</td>
</tr>
<tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p11230033165015"><a name="p11230033165015"></a><a name="p11230033165015"></a>ncode</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p953215815518"><a name="p953215815518"></a><a name="p953215815518"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.953395339533955%" headers="mcps1.1.5.1.3 "><p id="p18661136253"><a name="p18661136253"></a><a name="p18661136253"></a>Total number of base vectors.</p>
</td>
<td class="cellrowborder" valign="top" width="35.8935893589359%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>[1, 2^30-1]</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4982142445414"><a name="p4982142445414"></a><a name="p4982142445414"></a>codes</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7532158856"><a name="p7532158856"></a><a name="p7532158856"></a>const uint8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.953395339533955%" headers="mcps1.1.5.1.3 "><p id="p992551816390"><a name="p992551816390"></a><a name="p992551816390"></a>Codebook, which stores indexes of base vectors.</p>
</td>
<td class="cellrowborder" valign="top" width="35.8935893589359%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>The size is specified by <code>codes_size</code>.</p>
</td>
</tr>
<tr id="row103951453161513"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p14723141215409"><a name="p14723141215409"></a><a name="p14723141215409"></a>sim_table</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p4723181210404"><a name="p4723181210404"></a><a name="p4723181210404"></a>const float*</p>
</td>
<td class="cellrowborder" valign="top" width="35.8935893589359%" headers="mcps1.1.5.1.3 "><p id="p710155233915"><a name="p710155233915"></a><a name="p710155233915"></a>Similarity LUT, which stores the distance between per-dimension query vector and all centroids.</p>
</td>
<td class="cellrowborder" valign="top" width="35.8935893589359%" headers="mcps1.1.5.1.4 "><p id="p6723181274010"><a name="p6723181274010"></a><a name="p6723181274010"></a>The size is specified by <code>sim_table_size</code>.</p>
</td>
</tr>
<tr id="row1875218456372"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p275311453374"><a name="p275311453374"></a><a name="p275311453374"></a>dis0</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7753045173714"><a name="p7753045173714"></a><a name="p7753045173714"></a>float</p>
</td>
<td class="cellrowborder" valign="top" width="33.953395339533955%" headers="mcps1.1.5.1.3 "><p id="p17531445103716"><a name="p17531445103716"></a><a name="p17531445103716"></a>Initial distance.</p>
</td>
<td class="cellrowborder" valign="top" width="35.8935893589359%" headers="mcps1.1.5.1.4 "><p id="p69179904614"><a name="p69179904614"></a><a name="p69179904614"></a>Floating point number.</p>
</td>
</tr>
<tr id="row10770205351915"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p137414311617"><a name="p137414311617"></a><a name="p137414311617"></a>codes_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p06662231878"><a name="p06662231878"></a><a name="p06662231878"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.953395339533955%" headers="mcps1.1.5.1.3 "><p id="p16744431269"><a name="p16744431269"></a><a name="p16744431269"></a>Length of the codebook array.</p>
</td>
<td class="cellrowborder" valign="top" width="35.8935893589359%" headers="mcps1.1.5.1.4 "><p id="p127494317611"><a name="p127494317611"></a><a name="p127494317611"></a><code>dim</code> x <code>ncode</code></p>
</td>
</tr>
<tr id="row15300105641919"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p7119655861"><a name="p7119655861"></a><a name="p7119655861"></a>sim_table_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p6403112617719"><a name="p6403112617719"></a><a name="p6403112617719"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.953395339533955%" headers="mcps1.1.5.1.3 "><p id="p311925516613"><a name="p311925516613"></a><a name="p311925516613"></a>Length of the similarity LUT array.</p>
</td>
<td class="cellrowborder" valign="top" width="35.8935893589359%" headers="mcps1.1.5.1.4 "><p id="p1350143882216"><a name="p1350143882216"></a><a name="p1350143882216"></a><code>dim</code> x 256</p>
</td>
</tr>
</tbody>
</table>

**Return Values<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a><code>0</code> is returned on successful execution. In case of failure, an error code is returned to indicate the specific issue.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

int main() {
    // Parameter configuration
    size_t dim = 128; // Vector dimensions (i.e., the number of subspaces)
    size_t ncode = 10000; // Total number of base vectors
    size_t ksub = 256;
    int use_idx = 1; // Enable index filtering.
    size_t capacity = ncode;

    // LUT8b handle creation
    KRLLUT8bHandle* klh = NULL;
    int ret = krl_create_LUT8b_handle(&klh, use_idx, capacity);
    if (ret != 0) {
        printf("Failed to create the LUT8b handle: %d\n", ret);
        return -1;
    }

    // Set IDs of vectors to be used for computation.
    size_t* idx_ptr = krl_get_idx_pointer(klh);
    size_t selected_count = 500; // Compute only 500 vectors.
    for (size_t i = 0; i < selected_count; i++) {
        idx_ptr[i] = i * 20; // Select IDs 0, 20, 40, ...
    }

    // Prepare the codebook.
    size_t codes_size = dim * ncode;
    uint8_t* codes = (uint8_t*)malloc(codes_size * sizeof(uint8_t));
    for (size_t i = 0; i < codes_size; i++) {
        codes[i] = (uint8_t)(rand() % ksub);
    }

    // Prepare the similarity LUT.
    size_t sim_table_size = dim * ksub;
    float* sim_table = (float*)malloc(sim_table_size * sizeof(float));
    for (size_t i = 0; i < sim_table_size; i++) {
        sim_table[i] = (float)(rand() % 1000) / 100.0f;
    }

    // Perform accumulation based on 8-bit table lookup using the handle.
    float dis0 = 0.0f;
    ret = krl_table_lookup_8b_f32_with_handle(
        klh,
        dim,
        selected_count,  // Actual number of vectors for computation
        codes,
        sim_table,
        dis0,
        codes_size,
        sim_table_size
    );

    if (ret != 0) {
        printf("Failed to perform accumulation based on 8-bit table lookup using the handle: %d\n", ret);
        goto cleanup;
    }

    // Obtain the distance result.
    float* dist_ptr = krl_get_dist_pointer(klh);

    printf("Successfully perform accumulation based on 8-bit table lookup using the handle\n");
    printf("First 5 results:\n");
    for (size_t i = 0; i < 5 && i < selected_count; i++) {
        printf ("  Vector ID[%zu]: PQ distance = %f\n", idx_ptr[i], dist_ptr[i]);
    }

cleanup:
    krl_clean_LUT8b_handle(&klh);
    free(codes);
    free(sim_table);

    return ret;
}
```

## 4-bit Table Lookup-based Accumulation Interfaces

### krl\_fast\_table\_lookup\_step

**Interface Definition<a name="section172317194488"></a>**

int krl\_fast\_table\_lookup\_step\(int nq, int nsq, const uint8\_t\* codes, const uint8\_t\* LUT, uint16\_t\* dis, const uint16\_t\* threshold, uint32\_t\* lt\_mask, int keep\_min, size\_t codes\_size, size\_t LUT\_size, size\_t dis\_size, size\_t threshold\_size, size\_t lt\_mask\_size\);

**Function<a name="section1153124784912"></a>**

An operator designed for 4-bit table lookup, accumulation, filtering, and compression. It is used for batch processing of float-type query vectors. This operator is used to compute distances between a maximum of 16 query vectors and 32 base vectors. After the distance computation, each result is compared against a threshold. If a distance value is less than the threshold, the bit in <code>lt\_mask</code> of the corresponding base vector is set to <code>1</code>. Otherwise, it is set to <code>0</code>.

**Parameters<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="14.601460146014599%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row92301478154"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p223015479158"><a name="p223015479158"></a><a name="p223015479158"></a>nq</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p11230154710156"><a name="p11230154710156"></a><a name="p11230154710156"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p82303471154"><a name="p82303471154"></a><a name="p82303471154"></a>Total number of query vectors.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p923018478155"><a name="p923018478155"></a><a name="p923018478155"></a>[1, 16]</p>
</td>
</tr>
<tr id="row166241441532"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p262494414531"><a name="p262494414531"></a><a name="p262494414531"></a>nsq</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p126241544125310"><a name="p126241544125310"></a><a name="p126241544125310"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p1562414447536"><a name="p1562414447536"></a><a name="p1562414447536"></a>Number of subspaces.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p19624744195313"><a name="p19624744195313"></a><a name="p19624744195313"></a>An even number in [1, 256].</p>
</td>
</tr>
<tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p14381721205612"><a name="p14381721205612"></a><a name="p14381721205612"></a>codes</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7438122115569"><a name="p7438122115569"></a><a name="p7438122115569"></a>const uint8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p570319812427"><a name="p570319812427"></a><a name="p570319812427"></a>Codebook, which stores indexes of base vectors after krl_pack_codes_4b (blocksize=32) processing.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p51251625162911"><a name="p51251625162911"></a><a name="p51251625162911"></a>The size is specified by <code>codes_size</code>.</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4982142445414"><a name="p4982142445414"></a><a name="p4982142445414"></a>LUT</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7532158856"><a name="p7532158856"></a><a name="p7532158856"></a>const uint8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p36611261054"><a name="p36611261054"></a><a name="p36611261054"></a>Distance LUT, which stores the uint8 distances between product quantization (PQ) centroids and query vectors in each subspace.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>The size is specified by <code>LUT_size</code>.</p>
</td>
</tr>
<tr id="row103951453161513"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p14723141215409"><a name="p14723141215409"></a><a name="p14723141215409"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p4723181210404"><a name="p4723181210404"></a><a name="p4723181210404"></a>uint16_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p672341218403"><a name="p672341218403"></a><a name="p672341218403"></a>Stores the distance computation result.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p57801052141013"><a name="p57801052141013"></a><a name="p57801052141013"></a>The size is specified by <code>dis_size</code>. The memory needs to be allocated in advance.</p>
</td>
</tr>
<tr id="row1875218456372"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p275311453374"><a name="p275311453374"></a><a name="p275311453374"></a>threshold</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7753045173714"><a name="p7753045173714"></a><a name="p7753045173714"></a>const uint16_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p17531445103716"><a name="p17531445103716"></a><a name="p17531445103716"></a>Distance threshold.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p748810273302"><a name="p748810273302"></a><a name="p748810273302"></a>The size is specified by <code>threshold_size</code>. The threshold is <code>65535</code>.</p>
</td>
</tr>
<tr id="row143744955610"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p34370492563"><a name="p34370492563"></a><a name="p34370492563"></a>lt_mask</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p3437549145616"><a name="p3437549145616"></a><a name="p3437549145616"></a>uint32_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p143715495569"><a name="p143715495569"></a><a name="p143715495569"></a>Filtered and compressed results.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p77615321231"><a name="p77615321231"></a><a name="p77615321231"></a>The size is specified by <code>lt_mask_size</code>. The memory needs to be allocated in advance.</p>
</td>
</tr>
<tr id="row12299105712"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p22931165713"><a name="p22931165713"></a><a name="p22931165713"></a>keep_min</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p192916117571"><a name="p192916117571"></a><a name="p192916117571"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p8731759124214"><a name="p8731759124214"></a><a name="p8731759124214"></a>Indicates whether to retain the distance results less than the threshold.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p329412578"><a name="p329412578"></a><a name="p329412578"></a>[0, 1]</p>
<a name="ul164886121012"></a><a name="ul164886121012"></a><ul id="ul164886121012"><li><code>0</code>: Retain the distance results greater than the threshold. </li><li><code>1</code>: Retain the distance results less than the threshold.</li></ul>
</td>
</tr>
<tr id="row1167140172619"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p11681640172619"><a name="p11681640172619"></a><a name="p11681640172619"></a>codes_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p06662231878"><a name="p06662231878"></a><a name="p06662231878"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p16681940142616"><a name="p16681940142616"></a><a name="p16681940142616"></a>Length of the codebook array.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p568184012612"><a name="p568184012612"></a><a name="p568184012612"></a><code>nsq</code>/2 × 32</p>
</td>
</tr>
<tr id="row1758312172712"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p1258316232715"><a name="p1258316232715"></a><a name="p1258316232715"></a>LUT_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p6403112617719"><a name="p6403112617719"></a><a name="p6403112617719"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p1258316212714"><a name="p1258316212714"></a><a name="p1258316212714"></a>Length of the distance LUT array.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1658311212279"><a name="p1658311212279"></a><a name="p1658311212279"></a><code>nq</code> x <code>nsq</code> x 16</p>
</td>
</tr>
<tr id="row613215113273"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p1613312110277"><a name="p1613312110277"></a><a name="p1613312110277"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p1699263912712"><a name="p1699263912712"></a><a name="p1699263912712"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p21335117279"><a name="p21335117279"></a><a name="p21335117279"></a>Size of the distance result array.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p41335118277"><a name="p41335118277"></a><a name="p41335118277"></a><code>nq</code> x 32</p>
</td>
</tr>
<tr id="row9243174820292"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4243154811296"><a name="p4243154811296"></a><a name="p4243154811296"></a>threshold_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p1524318483294"><a name="p1524318483294"></a><a name="p1524318483294"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p8243184812293"><a name="p8243184812293"></a><a name="p8243184812293"></a>Length of the distance threshold array.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1824374814291"><a name="p1824374814291"></a><a name="p1824374814291"></a>The size is specified by <code>nq</code>.</p>
</td>
</tr>
<tr id="row721827152717"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p172182719273"><a name="p172182719273"></a><a name="p172182719273"></a>lt_mask_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p119923399274"><a name="p119923399274"></a><a name="p119923399274"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p92127202712"><a name="p92127202712"></a><a name="p92127202712"></a>Length of the array storing filtered and compressed results.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1421327132714"><a name="p1421327132714"></a><a name="p1421327132714"></a><code>nq</code>/32</p>
</td>
</tr>
</tbody>
</table>

**Return Values<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a><code>0</code> is returned on successful execution. In case of failure, an error code is returned to indicate the specific issue.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c
#include <stdio.h>
#include <stdlib.h>
#include <string.h>
#include "krl.h"

int main() {
    // 4-bit PQ parameter configuration
    int nq = 8;             // Number of query vectors (up to 16)
    int nsq = 64;           // Number of subspaces (must be an even number)
    int ncode = 32; // Number of base vectors (must be 32)
    int ksub = 16; // 4-bit index, with 16 centroids per subspace

    // Prepare the codebook (after 4-bit packing).
    // 4-bit packing: Every two 4-bit indexes are combined into one uint8.
    size_t codes_size = (nsq / 2) * ncode;
    uint8_t* codes = (uint8_t*)malloc(codes_size * sizeof(uint8_t));
    
    // Simulated 4-bit packed codebook data
    for (size_t i = 0; i < codes_size; i++) {
        uint8_t low = rand() % ksub;   // Lower 4 bits
        uint8_t high = rand() % ksub;  // Hiher 4 bits
        codes[i] = (high << 4) | low;
    }

    // Prepare the distance LUT.
    // Dimensions: nq × nsq × ksub
    size_t LUT_size = nq * nsq * ksub;
    uint8_t* LUT = (uint8_t*)malloc(LUT_size * sizeof(uint8_t));
    for (size_t i = 0; i < LUT_size; i++) {
        LUT[i] = (uint8_t)(rand() % 256);
    }

    // Prepare the distance result array.
    size_t dis_size = nq * ncode;
    uint16_t* distances = (uint16_t*)malloc(dis_size * sizeof(uint16_t));

    // Prepare the threshold array (one threshold per query vector).
    uint16_t* threshold = (uint16_t*)malloc(nq * sizeof(uint16_t));
    for (int i = 0; i < nq; i++) {
        threshold[i] = 5000;  // Set the distance threshold.
    }

    // Prepare the filter mask array.
    size_t lt_mask_size = (nq + 31) / 32;  // Round up.
    uint32_t* lt_mask = (uint32_t*)malloc(lt_mask_size * sizeof(uint32_t));
    memset(lt_mask, 0, lt_mask_size * sizeof(uint32_t));

    // Perform accumulation and filtering based on 4-bit table lookup.
    int keep_min = 1;  // Retain the results that are less than the threshold.
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
        printf("Failed to perform accumulation and filtering based on 4-bit table lookup. Error code: %d\n", ret);
        goto cleanup;
    }

    printf("Successfully performed accumulation and filtering based on 4-bit table lookup\n");

    // Count the number of vectors that meet the conditions.
    int passed_count = 0;
    for (size_t i = 0; i < lt_mask_size; i++) {
        for (int bit = 0; bit < 32; bit++) {
            if (lt_mask[i] & (1u << bit)) {
                passed_count++;
            }
        }
    }
    printf("Number of vectors that meet the threshold condition: %d\n", passed_count);

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

**Interface Definition <a name="section172317194488"></a>**

int krl\_L2\_table\_lookup\_fast\_scan\_bs64\(int nsq, const uint8\_t\* codes, const uint8\_t\* LUT, uint16\_t\* dis, uint16\_t threshold, uint32\_t\* lt\_mask, size\_t codes\_size, size\_t LUT\_size, size\_t dis\_size, size\_t lt\_mask\_size\);

**Function<a name="section1153124784912"></a>**

An operator designed for 4-bit table lookup, accumulation, filtering, and compression. It is used for processing float-type query vectors individually. Computes Euclidean distances between a query vector and 64 base vectors. Based on the distance comparison rule, if a distance value meets the comparison rule, the bit in <code>lt\_mask</code> of the corresponding base vector is set to <code>1</code>. Otherwise, it is set to <code>0</code>.

**Parameters<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="14.601460146014599%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="33.97339733973397%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="35.873587358735875%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row166241441532"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p262494414531"><a name="p262494414531"></a><a name="p262494414531"></a>nsq</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p126241544125310"><a name="p126241544125310"></a><a name="p126241544125310"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="33.97339733973397%" headers="mcps1.1.5.1.3 "><p id="p1562414447536"><a name="p1562414447536"></a><a name="p1562414447536"></a>Number of subspaces.</p>
</td>
<td class="cellrowborder" valign="top" width="35.873587358735875%" headers="mcps1.1.5.1.4 "><p id="p19624744195313"><a name="p19624744195313"></a><a name="p19624744195313"></a>An even number in [1, 256].</p>
</td>
</tr>
<tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p14381721205612"><a name="p14381721205612"></a><a name="p14381721205612"></a>codes</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7438122115569"><a name="p7438122115569"></a><a name="p7438122115569"></a>const uint8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.97339733973397%" headers="mcps1.1.5.1.3 "><p id="p18618921124518"><a name="p18618921124518"></a><a name="p18618921124518"></a>Codebook, which stores indexes of base vectors after krl_pack_codes_4b (blocksize=64) processing.</p>
</td>
<td class="cellrowborder" valign="top" width="35.873587358735875%" headers="mcps1.1.5.1.4 "><p id="p51251625162911"><a name="p51251625162911"></a><a name="p51251625162911"></a>The size is specified by <code>codes_size</code>.</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4982142445414"><a name="p4982142445414"></a><a name="p4982142445414"></a>LUT</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7532158856"><a name="p7532158856"></a><a name="p7532158856"></a>const uint8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.97339733973397%" headers="mcps1.1.5.1.3 "><p id="p36611261054"><a name="p36611261054"></a><a name="p36611261054"></a>Distance LUT, which stores the uint8 distances between PQ centroids and query vectors in each subspace.</p>
</td>
<td class="cellrowborder" valign="top" width="35.873587358735875%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>The size is specified by <code>LUT_size</code>.</p>
</td>
</tr>
<tr id="row103951453161513"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p14723141215409"><a name="p14723141215409"></a><a name="p14723141215409"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p4723181210404"><a name="p4723181210404"></a><a name="p4723181210404"></a>uint16_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.97339733973397%" headers="mcps1.1.5.1.3 "><p id="p672341218403"><a name="p672341218403"></a><a name="p672341218403"></a>Stores the distance computation result.</p>
</td>
<td class="cellrowborder" valign="top" width="35.873587358735875%" headers="mcps1.1.5.1.4 "><p id="p57801052141013"><a name="p57801052141013"></a><a name="p57801052141013"></a>The size is specified by <code>dis_size</code>. The memory needs to be allocated in advance.</p>
</td>
</tr>
<tr id="row1875218456372"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p275311453374"><a name="p275311453374"></a><a name="p275311453374"></a>threshold</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7753045173714"><a name="p7753045173714"></a><a name="p7753045173714"></a>const uint16_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.97339733973397%" headers="mcps1.1.5.1.3 "><p id="p17531445103716"><a name="p17531445103716"></a><a name="p17531445103716"></a>Distance threshold.</p>
</td>
<td class="cellrowborder" valign="top" width="35.873587358735875%" headers="mcps1.1.5.1.4 "><p id="p748810273302"><a name="p748810273302"></a><a name="p748810273302"></a>The value is <code>65535</code>.</p>
</td>
</tr>
<tr id="row143744955610"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p34370492563"><a name="p34370492563"></a><a name="p34370492563"></a>lt_mask</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p3437549145616"><a name="p3437549145616"></a><a name="p3437549145616"></a>uint32_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.97339733973397%" headers="mcps1.1.5.1.3 "><p id="p143715495569"><a name="p143715495569"></a><a name="p143715495569"></a>Filtered and compressed results.</p>
</td>
<td class="cellrowborder" valign="top" width="35.873587358735875%" headers="mcps1.1.5.1.4 "><p id="p77615321231"><a name="p77615321231"></a><a name="p77615321231"></a>The size is specified by <code>lt_mask_size</code>. The memory needs to be allocated in advance.</p>
</td>
</tr>
<tr id="row1695419558379"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p11681640172619"><a name="p11681640172619"></a><a name="p11681640172619"></a>codes_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p06662231878"><a name="p06662231878"></a><a name="p06662231878"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.97339733973397%" headers="mcps1.1.5.1.3 "><p id="p16681940142616"><a name="p16681940142616"></a><a name="p16681940142616"></a>Length of the codebook array.</p>
</td>
<td class="cellrowborder" valign="top" width="35.873587358735875%" headers="mcps1.1.5.1.4 "><p id="p568184012612"><a name="p568184012612"></a><a name="p568184012612"></a><code>nsq</code>/2 × 64</p>
</td>
</tr>
<tr id="row15954175511376"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p1258316232715"><a name="p1258316232715"></a><a name="p1258316232715"></a>LUT_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p6403112617719"><a name="p6403112617719"></a><a name="p6403112617719"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.97339733973397%" headers="mcps1.1.5.1.3 "><p id="p1258316212714"><a name="p1258316212714"></a><a name="p1258316212714"></a>Length of the distance LUT array.</p>
</td>
<td class="cellrowborder" valign="top" width="35.873587358735875%" headers="mcps1.1.5.1.4 "><p id="p1658311212279"><a name="p1658311212279"></a><a name="p1658311212279"></a><code>nsq</code> × 16</p>
</td>
</tr>
<tr id="row109541655133713"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p1613312110277"><a name="p1613312110277"></a><a name="p1613312110277"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p1699263912712"><a name="p1699263912712"></a><a name="p1699263912712"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.97339733973397%" headers="mcps1.1.5.1.3 "><p id="p21335117279"><a name="p21335117279"></a><a name="p21335117279"></a>Size of the distance result array.</p>
</td>
<td class="cellrowborder" valign="top" width="35.873587358735875%" headers="mcps1.1.5.1.4 "><p id="p41335118277"><a name="p41335118277"></a><a name="p41335118277"></a>The value is <code>64</code>.</p>
</td>
</tr>
<tr id="row4954455153717"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p172182719273"><a name="p172182719273"></a><a name="p172182719273"></a>lt_mask_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p119923399274"><a name="p119923399274"></a><a name="p119923399274"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.97339733973397%" headers="mcps1.1.5.1.3 "><p id="p92127202712"><a name="p92127202712"></a><a name="p92127202712"></a>Length of the array storing filtered and compressed results.</p>
</td>
<td class="cellrowborder" valign="top" width="35.873587358735875%" headers="mcps1.1.5.1.4 "><p id="p1421327132714"><a name="p1421327132714"></a><a name="p1421327132714"></a>The value is <code>2</code>.</p>
</td>
</tr>
</tbody>
</table>

**Return Values<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a><code>0</code> is returned on successful execution. In case of failure, an error code is returned to indicate the specific issue.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c
#include <stdio.h>
#include <stdlib.h>
#include <string.h>
#include "krl.h"

int main() {
    // 4-bit PQ parameter configuration (blocksize = 64)
    int nsq = 64;           // Number of subspaces (must be an even number)
    int ncode = 64; // Number of base vectors (must be 64)
    int ksub = 16; // 4-bit index

    // Prepare the codebook (4-bit packing, blocksize = 64).
    size_t codes_size = (nsq / 2) * ncode;
    uint8_t* codes = (uint8_t*)malloc(codes_size * sizeof(uint8_t));
    
    for (size_t i = 0; i < codes_size; i++) {
        uint8_t low = rand() % ksub;
        uint8_t high = rand() % ksub;
        codes[i] = (high << 4) | low;
    }

    // Prepare the distance LUT.
    size_t LUT_size = nsq * ksub;
    uint8_t* LUT = (uint8_t*)malloc(LUT_size * sizeof(uint8_t));
    for (size_t i = 0; i < LUT_size; i++) {
        LUT[i] = (uint8_t)(rand() % 256);
    }

    // Prepare the distance result array.
    uint16_t* distances = (uint16_t*)malloc(ncode * sizeof(uint16_t));

    // Prepare the filter mask array.
    size_t lt_mask_size = 2; // 64 vectors require two uint32 values.
    uint32_t* lt_mask = (uint32_t*)malloc(lt_mask_size * sizeof(uint32_t));
    memset(lt_mask, 0, lt_mask_size * sizeof(uint32_t));

    // Perform accumulation and filtering based on 4-bit table lookup for the L2 distance (block size = 64).
    uint16_t threshold = 8000;  // Distance threshold
    int ret = krl_L2_table_lookup_fast_scan_bs64(
        nsq,
        codes,
        LUT,
        distances,
        threshold,
        lt_mask,
        codes_size,
        LUT_size,
        ncode, // dis_size must be 64.
        lt_mask_size
    );

    if (ret != 0) {
        printf("Failed to perform accumulation and filtering based on 4-bit table lookup for the L2 distance. Error code: %d\n", ret);
        goto cleanup;
    }

    printf("Successfully performed accumulation and filtering based on 4-bit table lookup (bs64) for L2 distance\n");

    // Determine vectors that meet the conditions.
    printf("Number of vectors that meet the condition (distance < %u): \n", threshold);
    int count = 0;
    for (int i = 0; i < ncode; i++) {
        int mask_idx = i / 32;
        int bit_idx = i % 32;
        if (lt_mask[mask_idx] & (1u << bit_idx)) {
            if (count < 10) { // Display only the first 10 vectors.
                printf("  Vector [%d]: distance = %u\n", i, distances[i]);
            }
            count++;
        }
    }
    printf("A total of %d vectors meet the condition.\n", count);

cleanup:
    free(codes);
    free(LUT);
    free(distances);
    free(lt_mask);

    return ret;
}
```

### krl\_IP\_table\_lookup\_fast\_scan\_bs64

**Interface Definition <a name="section172317194488"></a>**

int krl\_IP\_table\_lookup\_fast\_scan\_bs64\(int nsq, const uint8\_t\* codes, const uint8\_t\* LUT, uint16\_t\* dis, uint16\_t threshold, uint32\_t\* lt\_mask, size\_t codes\_size, size\_t LUT\_size, size\_t dis\_size, size\_t lt\_mask\_size\);

**Function<a name="section1153124784912"></a>**

An operator designed for 4-bit table lookup, accumulation, filtering, and compression. It is used for processing float-type query vectors individually. It computes distances between a query vector and 64 base vectors using inner product. Based on the distance comparison rule, if a distance value meets the comparison rule, the bit in <code>lt\_mask</code> of the corresponding base vector is set to <code>1</code>. Otherwise, it is set to <code>0</code>.

**Parameters<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="14.601460146014599%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row166241441532"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p262494414531"><a name="p262494414531"></a><a name="p262494414531"></a>nsq</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p126241544125310"><a name="p126241544125310"></a><a name="p126241544125310"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p1562414447536"><a name="p1562414447536"></a><a name="p1562414447536"></a>Number of subspaces.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p19624744195313"><a name="p19624744195313"></a><a name="p19624744195313"></a>An even number in [1, 256].</p>
</td>
</tr>
<tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p14381721205612"><a name="p14381721205612"></a><a name="p14381721205612"></a>codes</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7438122115569"><a name="p7438122115569"></a><a name="p7438122115569"></a>const uint8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p18618921124518"><a name="p18618921124518"></a><a name="p18618921124518"></a>Codebook, which stores indexes of base vectors after krl_pack_codes_4b (blocksize=64) processing.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p51251625162911"><a name="p51251625162911"></a><a name="p51251625162911"></a>The size is specified by <code>codes_size</code>.</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4982142445414"><a name="p4982142445414"></a><a name="p4982142445414"></a>LUT</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7532158856"><a name="p7532158856"></a><a name="p7532158856"></a>const uint8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p36611261054"><a name="p36611261054"></a><a name="p36611261054"></a>Distance LUT, which stores the uint8 distances between product quantization (PQ) centroids and query vectors in each subspace.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>The size is specified by <code>LUT_size</code>.</p>
</td>
</tr>
<tr id="row103951453161513"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p14723141215409"><a name="p14723141215409"></a><a name="p14723141215409"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p4723181210404"><a name="p4723181210404"></a><a name="p4723181210404"></a>uint16_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p672341218403"><a name="p672341218403"></a><a name="p672341218403"></a>Stores the distance computation result.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p57801052141013"><a name="p57801052141013"></a><a name="p57801052141013"></a>The size is specified by <code>dis_size</code>. The memory needs to be allocated in advance.</p>
</td>
</tr>
<tr id="row1875218456372"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p275311453374"><a name="p275311453374"></a><a name="p275311453374"></a>threshold</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7753045173714"><a name="p7753045173714"></a><a name="p7753045173714"></a>const uint16_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p17531445103716"><a name="p17531445103716"></a><a name="p17531445103716"></a>Distance threshold.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p748810273302"><a name="p748810273302"></a><a name="p748810273302"></a>The value is <code>65535</code>.</p>
</td>
</tr>
<tr id="row143744955610"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p34370492563"><a name="p34370492563"></a><a name="p34370492563"></a>lt_mask</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p3437549145616"><a name="p3437549145616"></a><a name="p3437549145616"></a>uint32_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p143715495569"><a name="p143715495569"></a><a name="p143715495569"></a>Filtered and compressed results.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p77615321231"><a name="p77615321231"></a><a name="p77615321231"></a>The size is specified by <code>lt_mask_size</code>. The memory needs to be allocated in advance.</p>
</td>
</tr>
<tr id="row177615011429"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p11681640172619"><a name="p11681640172619"></a><a name="p11681640172619"></a>codes_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p06662231878"><a name="p06662231878"></a><a name="p06662231878"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p16681940142616"><a name="p16681940142616"></a><a name="p16681940142616"></a>Length of the codebook array.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p568184012612"><a name="p568184012612"></a><a name="p568184012612"></a><code>nsq</code>/2 × 64</p>
</td>
</tr>
<tr id="row9760006427"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p1258316232715"><a name="p1258316232715"></a><a name="p1258316232715"></a>LUT_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p6403112617719"><a name="p6403112617719"></a><a name="p6403112617719"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p1258316212714"><a name="p1258316212714"></a><a name="p1258316212714"></a>Length of the distance LUT array.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1658311212279"><a name="p1658311212279"></a><a name="p1658311212279"></a><code>nsq</code> × 16</p>
</td>
</tr>
<tr id="row1276017012420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p1613312110277"><a name="p1613312110277"></a><a name="p1613312110277"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p1699263912712"><a name="p1699263912712"></a><a name="p1699263912712"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p21335117279"><a name="p21335117279"></a><a name="p21335117279"></a>Size of the distance result array.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p41335118277"><a name="p41335118277"></a><a name="p41335118277"></a>The value is <code>64</code>.</p>
</td>
</tr>
<tr id="row157604034212"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p172182719273"><a name="p172182719273"></a><a name="p172182719273"></a>lt_mask_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p119923399274"><a name="p119923399274"></a><a name="p119923399274"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p92127202712"><a name="p92127202712"></a><a name="p92127202712"></a>Length of the array storing filtered and compressed results.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1421327132714"><a name="p1421327132714"></a><a name="p1421327132714"></a>The value is <code>2</code>.</p>
</td>
</tr>
</tbody>
</table>

**Return Values<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a><code>0</code> is returned on successful execution. In case of failure, an error code is returned to indicate the specific issue.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c
#include <stdio.h>
#include <stdlib.h>
#include <string.h>
#include "krl.h"

int main() {
    // 4-bit PQ parameter configuration (inner product distance, blocksize = 64)
    int nsq = 64;           // Number of subspaces (must be an even number)
    int ncode = 64; // Number of base vectors (must be 64)
    int ksub = 16; // 4-bit index, with 16 centroids per subspace

    // Prepare the codebook (4-bit packing, blocksize = 64).
    size_t codes_size = (nsq / 2) * ncode;
    uint8_t* codes = (uint8_t*)malloc(codes_size * sizeof(uint8_t));
    
    for (size_t i = 0; i < codes_size; i++) {
        uint8_t low = rand() % ksub;
        uint8_t high = rand() % ksub;
        codes[i] = (high << 4) | low;
    }

    // Prepare the inner product distance LUT.
    // Note: The distance value computed using inner product usually needs to be negated or specially processed for comparison.
    size_t LUT_size = nsq * ksub;
    uint8_t* LUT = (uint8_t*)malloc(LUT_size * sizeof(uint8_t));
    for (size_t i = 0; i < LUT_size; i++) {
        LUT[i] = (uint8_t)(rand() % 256);
    }

    // Prepare the distance result array.
    uint16_t* distances = (uint16_t*)malloc(ncode * sizeof(uint16_t));

    // Prepare the filter mask array.
    size_t lt_mask_size = 2; // 64 vectors require two uint32 values.
    uint32_t* lt_mask = (uint32_t*)malloc(lt_mask_size * sizeof(uint32_t));
    memset(lt_mask, 0, lt_mask_size * sizeof(uint32_t));

    // Perform accumulation and filtering based on 4-bit table lookup for the inner product distance.
    // Note: For the inner product distance, the threshold comparison rule is different from that for the L2 distance.
    // A larger inner product indicates higher similarity. Therefore, results greater than the threshold are usually retained.
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
        printf("Failed to perform accumulation and filtering based on 4-bit table lookup for the inner product (IP) distance. Error code: %d\n", ret);
        goto cleanup;
    }

    printf("Successfully performed accumulation and filtering based on 4-bit table lookup (bs64) for the IP distance\n");

    // Determine vectors that meet the condition (inner product > threshold).
    int count = 0;
    printf("Number of vectors that meet the condition (inner product > %u): \n", threshold);
    for (int i = 0; i < ncode; i++) {
        int mask_idx = i / 32;
        int bit_idx = i % 32;
        if (lt_mask[mask_idx] & (1u << bit_idx)) {
            if (count < 5) {
                printf("  Vector [%d]: inner product = %u\n", i, distances[i]);
            }
            count++;
        }
    }
    printf("A total of %d vectors meet the condition.\n", count);

cleanup:
    free(codes);
    free(LUT);
    free(distances);
    free(lt_mask);

    return ret;
}
```

### krl\_L2\_table\_lookup\_fast\_scan\_bs96

**Interface Definition <a name="section172317194488"></a>**

int krl\_L2\_table\_lookup\_fast\_scan\_bs96\(int nsq, const uint8\_t\* codes, const uint8\_t\* LUT, uint16\_t\* dis, uint16\_t threshold, uint32\_t\* lt\_mask, size\_t codes\_size, size\_t LUT\_size, size\_t dis\_size, size\_t lt\_mask\_size\);

**Function<a name="section1153124784912"></a>**

An operator designed for 4-bit table lookup, accumulation, filtering, and compression. It is used for processing float-type query vectors individually. It computes Euclidean distances between a query vector and 96 base vectors. Based on the distance comparison rule, if a distance value meets the comparison rule, the bit in <code>lt\_mask</code> of the corresponding base vector is set to <code>1</code>. Otherwise, it is set to <code>0</code>.

**Parameters<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="14.601460146014599%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row166241441532"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p262494414531"><a name="p262494414531"></a><a name="p262494414531"></a>nsq</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p126241544125310"><a name="p126241544125310"></a><a name="p126241544125310"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p1562414447536"><a name="p1562414447536"></a><a name="p1562414447536"></a>Number of subspaces.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p19624744195313"><a name="p19624744195313"></a><a name="p19624744195313"></a>An even number in [1, 256].</p>
</td>
</tr>
<tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p14381721205612"><a name="p14381721205612"></a><a name="p14381721205612"></a>codes</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7438122115569"><a name="p7438122115569"></a><a name="p7438122115569"></a>const uint8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p18438121155616"><a name="p18438121155616"></a><a name="p18438121155616"></a>Codebook, which stores indexes of base vectors after krl_pack_codes_4b (blocksize=96) processing.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p51251625162911"><a name="p51251625162911"></a><a name="p51251625162911"></a>The size is specified by <code>codes_size</code>.</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4982142445414"><a name="p4982142445414"></a><a name="p4982142445414"></a>LUT</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7532158856"><a name="p7532158856"></a><a name="p7532158856"></a>const uint8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p36611261054"><a name="p36611261054"></a><a name="p36611261054"></a>Distance LUT, which stores the uint8 distances between product quantization (PQ) centroids and query vectors in each subspace.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>The size is specified by <code>LUT_size</code>.</p>
</td>
</tr>
<tr id="row103951453161513"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p14723141215409"><a name="p14723141215409"></a><a name="p14723141215409"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p4723181210404"><a name="p4723181210404"></a><a name="p4723181210404"></a>uint16_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p672341218403"><a name="p672341218403"></a><a name="p672341218403"></a>Stores the distance computation result.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p57801052141013"><a name="p57801052141013"></a><a name="p57801052141013"></a>The size is specified by <code>dis_size</code>. The memory needs to be allocated in advance.</p>
</td>
</tr>
<tr id="row1875218456372"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p275311453374"><a name="p275311453374"></a><a name="p275311453374"></a>threshold</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7753045173714"><a name="p7753045173714"></a><a name="p7753045173714"></a>const uint16_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p17531445103716"><a name="p17531445103716"></a><a name="p17531445103716"></a>Distance threshold.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p748810273302"><a name="p748810273302"></a><a name="p748810273302"></a>The value is <code>65535</code>.</p>
</td>
</tr>
<tr id="row143744955610"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p34370492563"><a name="p34370492563"></a><a name="p34370492563"></a>lt_mask</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p3437549145616"><a name="p3437549145616"></a><a name="p3437549145616"></a>uint32_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p143715495569"><a name="p143715495569"></a><a name="p143715495569"></a>Filtered and compressed results.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p77615321231"><a name="p77615321231"></a><a name="p77615321231"></a>The size is specified by <code>lt_mask_size</code>. The memory needs to be allocated in advance.</p>
</td>
</tr>
<tr id="row02162634718"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p11681640172619"><a name="p11681640172619"></a><a name="p11681640172619"></a>codes_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p06662231878"><a name="p06662231878"></a><a name="p06662231878"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p16681940142616"><a name="p16681940142616"></a><a name="p16681940142616"></a>Length of the codebook array.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p568184012612"><a name="p568184012612"></a><a name="p568184012612"></a><code>nsq</code>/2 × 96</p>
</td>
</tr>
<tr id="row11211726184714"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p1258316232715"><a name="p1258316232715"></a><a name="p1258316232715"></a>LUT_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p6403112617719"><a name="p6403112617719"></a><a name="p6403112617719"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p1258316212714"><a name="p1258316212714"></a><a name="p1258316212714"></a>Length of the distance LUT array.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1658311212279"><a name="p1658311212279"></a><a name="p1658311212279"></a><code>nsq</code> × 16</p>
</td>
</tr>
<tr id="row172114262476"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p1613312110277"><a name="p1613312110277"></a><a name="p1613312110277"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p1699263912712"><a name="p1699263912712"></a><a name="p1699263912712"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p21335117279"><a name="p21335117279"></a><a name="p21335117279"></a>Size of the distance result array.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p41335118277"><a name="p41335118277"></a><a name="p41335118277"></a>The value is <code>96</code>.</p>
</td>
</tr>
<tr id="row11201326164720"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p172182719273"><a name="p172182719273"></a><a name="p172182719273"></a>lt_mask_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p119923399274"><a name="p119923399274"></a><a name="p119923399274"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p92127202712"><a name="p92127202712"></a><a name="p92127202712"></a>Length of the array storing filtered and compressed results.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1421327132714"><a name="p1421327132714"></a><a name="p1421327132714"></a>The value is <code>3</code>.</p>
</td>
</tr>
</tbody>
</table>

**Return Values<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a><code>0</code> is returned on successful execution. In case of failure, an error code is returned to indicate the specific issue.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c
#include <stdio.h>
#include <stdlib.h>
#include <string.h>
#include "krl.h"

int main() {
    // 4-bit PQ parameter configuration (L2 distance, blocksize = 96)
    int nsq = 64;           // Number of subspaces (must be an even number)
    int ncode = 96; // Number of base vectors (must be 96)
    int ksub = 16; // 4-bit index

    // Prepare the codebook (4-bit packing, blocksize = 96).
    size_t codes_size = (nsq / 2) * ncode;
    uint8_t* codes = (uint8_t*)malloc(codes_size * sizeof(uint8_t));
    
    for (size_t i = 0; i < codes_size; i++) {
        uint8_t low = rand() % ksub;
        uint8_t high = rand() % ksub;
        codes[i] = (high << 4) | low;
    }

    // Prepare the L2 distance LUT.
    size_t LUT_size = nsq * ksub;
    uint8_t* LUT = (uint8_t*)malloc(LUT_size * sizeof(uint8_t));
    for (size_t i = 0; i < LUT_size; i++) {
        LUT[i] = (uint8_t)(rand() % 256);
    }

    // Prepare the distance result array.
    uint16_t* distances = (uint16_t*)malloc(ncode * sizeof(uint16_t));

    // Prepare the filter mask array.
    // 96 vectors require 3 uint32 values (96/32 = 3).
    size_t lt_mask_size = 3;
    uint32_t* lt_mask = (uint32_t*)malloc(lt_mask_size * sizeof(uint32_t));
    memset(lt_mask, 0, lt_mask_size * sizeof(uint32_t));

    // Perform accumulation and filtering based on 4-bit table lookup for the L2 distance (block size = 96).
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
        ncode, // dis_size must be 96.
        lt_mask_size
    );

    if (ret != 0) {
        printf("Failed to perform accumulation and filtering based on 4-bit table lookup (bs96) for the L2 distance. Error code: %d\n", ret);
        goto cleanup;
    }

    printf("Successfully performed accumulation and filtering based on 4-bit table lookup (bs96) for L2 distance\n");

    // Determine vectors that meet the conditions.
    int count = 0;
    for (int i = 0; i < ncode; i++) {
        int mask_idx = i / 32;
        int bit_idx = i % 32;
        if (lt_mask[mask_idx] & (1u << bit_idx)) {
            count++;
        }
    }
    printf("A total of %d vectors meet the condition (L2 distance < %u).\n", count, threshold);

cleanup:
    free(codes);
    free(LUT);
    free(distances);
    free(lt_mask);

    return ret;
}
```

### krl\_IP\_table\_lookup\_fast\_scan\_bs96

**Interface Definition <a name="section172317194488"></a>**

int krl\_IP\_table\_lookup\_fast\_scan\_bs96\(int nsq, const uint8\_t\* codes, const uint8\_t\* LUT, uint16\_t\* dis, uint16\_t threshold, uint32\_t\* lt\_mask, size\_t codes\_size, size\_t LUT\_size, size\_t dis\_size, size\_t lt\_mask\_size\);

**Function<a name="section1153124784912"></a>**

An operator designed for 4-bit table lookup, accumulation, filtering, and compression. It is used for processing float-type query vectors individually. Computes distances between a query vector and 96 base vectors using inner product. Based on the distance comparison rule, if a distance value meets the comparison rule, the bit in <code>lt\_mask</code> of the corresponding base vector is set to <code>1</code>. Otherwise, it is set to <code>0</code>.

**Parameters<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="14.601460146014599%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="33.903390339033905%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="35.94359435943594%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row166241441532"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p262494414531"><a name="p262494414531"></a><a name="p262494414531"></a>nsq</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p126241544125310"><a name="p126241544125310"></a><a name="p126241544125310"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="33.903390339033905%" headers="mcps1.1.5.1.3 "><p id="p1562414447536"><a name="p1562414447536"></a><a name="p1562414447536"></a>Number of subspaces.</p>
</td>
<td class="cellrowborder" valign="top" width="35.94359435943594%" headers="mcps1.1.5.1.4 "><p id="p19624744195313"><a name="p19624744195313"></a><a name="p19624744195313"></a>An even number in [1, 256].</p>
</td>
</tr>
<tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p14381721205612"><a name="p14381721205612"></a><a name="p14381721205612"></a>codes</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7438122115569"><a name="p7438122115569"></a><a name="p7438122115569"></a>const uint8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.903390339033905%" headers="mcps1.1.5.1.3 "><p id="p18438121155616"><a name="p18438121155616"></a><a name="p18438121155616"></a>Codebook, which stores indexes of base vectors after krl_pack_codes_4b (blocksize=96) processing.</p>
</td>
<td class="cellrowborder" valign="top" width="35.94359435943594%" headers="mcps1.1.5.1.4 "><p id="p51251625162911"><a name="p51251625162911"></a><a name="p51251625162911"></a>The size is specified by <code>codes_size</code>.</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p4982142445414"><a name="p4982142445414"></a><a name="p4982142445414"></a>LUT</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7532158856"><a name="p7532158856"></a><a name="p7532158856"></a>const uint8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.903390339033905%" headers="mcps1.1.5.1.3 "><p id="p36611261054"><a name="p36611261054"></a><a name="p36611261054"></a>Distance LUT, which stores the uint8 distances between product quantization (PQ) centroids and query vectors in each subspace.</p>
</td>
<td class="cellrowborder" valign="top" width="35.94359435943594%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>The size is specified by <code>LUT_size</code>.</p>
</td>
</tr>
<tr id="row103951453161513"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p14723141215409"><a name="p14723141215409"></a><a name="p14723141215409"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p4723181210404"><a name="p4723181210404"></a><a name="p4723181210404"></a>uint16_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.903390339033905%" headers="mcps1.1.5.1.3 "><p id="p672341218403"><a name="p672341218403"></a><a name="p672341218403"></a>Stores the distance computation result.</p>
</td>
<td class="cellrowborder" valign="top" width="35.94359435943594%" headers="mcps1.1.5.1.4 "><p id="p57801052141013"><a name="p57801052141013"></a><a name="p57801052141013"></a>The size is specified by <code>dis_size</code>. The memory needs to be allocated in advance.</p>
</td>
</tr>
<tr id="row1875218456372"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p275311453374"><a name="p275311453374"></a><a name="p275311453374"></a>threshold</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7753045173714"><a name="p7753045173714"></a><a name="p7753045173714"></a>const uint16_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.903390339033905%" headers="mcps1.1.5.1.3 "><p id="p17531445103716"><a name="p17531445103716"></a><a name="p17531445103716"></a>Distance threshold.</p>
</td>
<td class="cellrowborder" valign="top" width="35.94359435943594%" headers="mcps1.1.5.1.4 "><p id="p748810273302"><a name="p748810273302"></a><a name="p748810273302"></a>The value is <code>65535</code>.</p>
</td>
</tr>
<tr id="row143744955610"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p34370492563"><a name="p34370492563"></a><a name="p34370492563"></a>lt_mask</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p3437549145616"><a name="p3437549145616"></a><a name="p3437549145616"></a>uint32_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.903390339033905%" headers="mcps1.1.5.1.3 "><p id="p143715495569"><a name="p143715495569"></a><a name="p143715495569"></a>Filtered and compressed results.</p>
</td>
<td class="cellrowborder" valign="top" width="35.94359435943594%" headers="mcps1.1.5.1.4 "><p id="p77615321231"><a name="p77615321231"></a><a name="p77615321231"></a>The size is specified by <code>lt_mask_size</code>. The memory needs to be allocated in advance.</p>
</td>
</tr>
<tr id="row3115131755217"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p11681640172619"><a name="p11681640172619"></a><a name="p11681640172619"></a>codes_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p06662231878"><a name="p06662231878"></a><a name="p06662231878"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="35.94359435943594%" headers="mcps1.1.5.1.3 "><p id="p16681940142616"><a name="p16681940142616"></a><a name="p16681940142616"></a>Length of the codebook array.</p>
</td>
<td class="cellrowborder" valign="top" width="35.94359435943594%" headers="mcps1.1.5.1.4 "><p id="p568184012612"><a name="p568184012612"></a><a name="p568184012612"></a><code>nsq</code>/2 × 96</p>
</td>
</tr>
<tr id="row511551717527"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p1258316232715"><a name="p1258316232715"></a><a name="p1258316232715"></a>LUT_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p6403112617719"><a name="p6403112617719"></a><a name="p6403112617719"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.903390339033905%" headers="mcps1.1.5.1.3 "><p id="p1258316212714"><a name="p1258316212714"></a><a name="p1258316212714"></a>Length of the distance LUT array.</p>
</td>
<td class="cellrowborder" valign="top" width="35.94359435943594%" headers="mcps1.1.5.1.4 "><p id="p1658311212279"><a name="p1658311212279"></a><a name="p1658311212279"></a><code>nsq</code> × 16</p>
</td>
</tr>
<tr id="row11115201711529"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p1613312110277"><a name="p1613312110277"></a><a name="p1613312110277"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p1699263912712"><a name="p1699263912712"></a><a name="p1699263912712"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.903390339033905%" headers="mcps1.1.5.1.3 "><p id="p21335117279"><a name="p21335117279"></a><a name="p21335117279"></a>Size of the distance result array.</p>
</td>
<td class="cellrowborder" valign="top" width="35.94359435943594%" headers="mcps1.1.5.1.4 "><p id="p41335118277"><a name="p41335118277"></a><a name="p41335118277"></a>The value is <code>96</code>.</p>
</td>
</tr>
<tr id="row111141217155212"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p172182719273"><a name="p172182719273"></a><a name="p172182719273"></a>lt_mask_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p119923399274"><a name="p119923399274"></a><a name="p119923399274"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.903390339033905%" headers="mcps1.1.5.1.3 "><p id="p92127202712"><a name="p92127202712"></a><a name="p92127202712"></a>Length of the array storing filtered and compressed results.</p>
</td>
<td class="cellrowborder" valign="top" width="35.94359435943594%" headers="mcps1.1.5.1.4 "><p id="p1421327132714"><a name="p1421327132714"></a><a name="p1421327132714"></a>The value is <code>3</code>.</p>
</td>
</tr>
</tbody>
</table>

**Return Values<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a><code>0</code> is returned on successful execution. In case of failure, an error code is returned to indicate the specific issue.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c
#include <stdio.h>
#include <stdlib.h>
#include <string.h>
#include "krl.h"

int main() {
    // 4-bit PQ parameter configuration (inner product distance, blocksize = 96)
    int nsq = 64;
    int ncode = 96;
    int ksub = 16;

    // Prepare the codebook.
    size_t codes_size = (nsq / 2) * ncode;
    uint8_t* codes = (uint8_t*)malloc(codes_size * sizeof(uint8_t));
    for (size_t i = 0; i < codes_size; i++) {
        uint8_t low = rand() % ksub;
        uint8_t high = rand() % ksub;
        codes[i] = (high << 4) | low;
    }

    // Prepare the inner product distance LUT.
    size_t LUT_size = nsq * ksub;
    uint8_t* LUT = (uint8_t*)malloc(LUT_size * sizeof(uint8_t));
    for (size_t i = 0; i < LUT_size; i++) {
        LUT[i] = (uint8_t)(rand() % 256);
    }

    // Prepare the result array.
    uint16_t* distances = (uint16_t*)malloc(ncode * sizeof(uint16_t));
    size_t lt_mask_size = 3;
    uint32_t* lt_mask = (uint32_t*)malloc(lt_mask_size * sizeof(uint32_t));
    memset(lt_mask, 0, lt_mask_size * sizeof(uint32_t));

    // Perform accumulation and filtering based on 4-bit table lookup (bs96) for the inner product distance.
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
        printf("Failed to perform accumulation and filtering based on 4-bit table lookup (bs96) for the IP distance. Error code: %d\n", ret);
        goto cleanup;
    }

    printf("Successfully performed accumulation and filtering based on 4-bit table lookup (bs96) for the IP distance\n");

    // Output the top-5 maximum inner product values.
    printf("Top-5 maximum inner product values:\n");
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
            printf("  Rank %d: vector [%d], inner product = %u\n", k + 1, max_idx, max_val);
            distances[max_idx] = 0; // Mark as selected.
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

**Interface Definition <a name="section172317194488"></a>**

int krl\_table\_lookup\_4b\_f16\(size\_t nsq, size\_t ncode, const uint8\_t\* codes, const uint16\_t\* LUT, float\* dis, uint16\_t dis0, size\_t codes\_size, size\_t LUT\_size, size\_t dis\_size\);

**Function<a name="section1153124784912"></a>**

An operator designed for 4-bit table lookup, accumulation, filtering, and compression. It is used for processing fp16 query vectors individually. It computes distances between a query vector and multiple base vectors using inner product. The initial distance is <code>dis0</code>. This interface does not perform filtering or compression (that is, comparison with the threshold).

**Parameters<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.551555155515551%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="14.601460146014599%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row166241441532"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p262494414531"><a name="p262494414531"></a><a name="p262494414531"></a>nsq</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p126241544125310"><a name="p126241544125310"></a><a name="p126241544125310"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p1562414447536"><a name="p1562414447536"></a><a name="p1562414447536"></a>Number of subspaces.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p19624744195313"><a name="p19624744195313"></a><a name="p19624744195313"></a>An even number in [1, 65535].</p>
</td>
</tr>
<tr id="row8437621111217"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p943722161218"><a name="p943722161218"></a><a name="p943722161218"></a>ncode</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p19437152117123"><a name="p19437152117123"></a><a name="p19437152117123"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p543720213125"><a name="p543720213125"></a><a name="p543720213125"></a>Total number of base vectors.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p743792191219"><a name="p743792191219"></a><a name="p743792191219"></a>[1, 2^30-1]</p>
</td>
</tr>
<tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p14381721205612"><a name="p14381721205612"></a><a name="p14381721205612"></a>codes</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7438122115569"><a name="p7438122115569"></a><a name="p7438122115569"></a>const uint8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p18438121155616"><a name="p18438121155616"></a><a name="p18438121155616"></a>Codebook, which stores indexes of base vectors after krl_pack_codes_4b (blocksize=64) processing.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p51251625162911"><a name="p51251625162911"></a><a name="p51251625162911"></a>The size is specified by <code>codes_size</code>.</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p734604031220"><a name="p734604031220"></a><a name="p734604031220"></a>LUT</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7532158856"><a name="p7532158856"></a><a name="p7532158856"></a>const uint16_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p36611261054"><a name="p36611261054"></a><a name="p36611261054"></a>Distance LUT, which stores the fp16 distances between PQ centroids and query vectors in each subspace.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>The size is specified by <code>LUT_size</code>.</p>
</td>
</tr>
<tr id="row103951453161513"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p14723141215409"><a name="p14723141215409"></a><a name="p14723141215409"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p4723181210404"><a name="p4723181210404"></a><a name="p4723181210404"></a>float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p672341218403"><a name="p672341218403"></a><a name="p672341218403"></a>Stores the distance computation result.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p57801052141013"><a name="p57801052141013"></a><a name="p57801052141013"></a>The size is specified by <code>dis_size</code>. The memory needs to be allocated in advance.</p>
</td>
</tr>
<tr id="row1875218456372"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p564545281211"><a name="p564545281211"></a><a name="p564545281211"></a>dis0</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p7753045173714"><a name="p7753045173714"></a><a name="p7753045173714"></a>uint16_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p17531445103716"><a name="p17531445103716"></a><a name="p17531445103716"></a>Initial distance.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p69179904614"><a name="p69179904614"></a><a name="p69179904614"></a>Floating point number.</p>
</td>
</tr>
<tr id="row5701164775910"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p137414311617"><a name="p137414311617"></a><a name="p137414311617"></a>codes_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p06662231878"><a name="p06662231878"></a><a name="p06662231878"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p16744431269"><a name="p16744431269"></a><a name="p16744431269"></a>Length of the codebook array.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p127494317611"><a name="p127494317611"></a><a name="p127494317611"></a><code>nsq</code>/2 × <code>ncode</code></p>
</td>
</tr>
<tr id="row97004477597"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p1258316232715"><a name="p1258316232715"></a><a name="p1258316232715"></a>LUT_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p6403112617719"><a name="p6403112617719"></a><a name="p6403112617719"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p1258316212714"><a name="p1258316212714"></a><a name="p1258316212714"></a>Length of the distance LUT array.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1658311212279"><a name="p1658311212279"></a><a name="p1658311212279"></a><code>nsq</code> × 16</p>
</td>
</tr>
<tr id="row67009473597"><td class="cellrowborder" valign="top" width="15.551555155515551%" headers="mcps1.1.5.1.1 "><p id="p1753316619720"><a name="p1753316619720"></a><a name="p1753316619720"></a>dis_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.601460146014599%" headers="mcps1.1.5.1.2 "><p id="p64039264714"><a name="p64039264714"></a><a name="p64039264714"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p54111354134020"><a name="p54111354134020"></a><a name="p54111354134020"></a>Size of the distance result array.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p175331661478"><a name="p175331661478"></a><a name="p175331661478"></a>The size is specified by <code>ncode</code>.</p>
</td>
</tr>
</tbody>
</table>

**Return Values<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a><code>0</code> is returned on successful execution. In case of failure, an error code is returned to indicate the specific issue.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

// Auxiliary function: Convert float to fp16.
uint16_t float_to_fp16(float value);

int main() {
    // 4-bit PQ parameter configuration (fp16 distance LUT)
    size_t nsq = 64;        // Number of subspaces (must be an even number)
    size_t ncode = 1000;    // Total number of base vectors
    size_t ksub = 16;       // 4-bit index

    // Prepare the codebook (4-bit packing).
    size_t codes_size = (nsq / 2) * ncode;
    uint8_t* codes = (uint8_t*)malloc(codes_size * sizeof(uint8_t));
    for (size_t i = 0; i < codes_size; i++) {
        uint8_t low = rand() % ksub;
        uint8_t high = rand() % ksub;
        codes[i] = (high << 4) | low;
    }

    // Prepare the fp16 distance LUT.
    size_t LUT_size = nsq * ksub;
    uint16_t* LUT = (uint16_t*)malloc(LUT_size * sizeof(uint16_t));
    for (size_t i = 0; i < LUT_size; i++) {
        // Convert the distance value to the fp16 format.
        float dist = (float)(rand() % 1000) / 100.0f;
        LUT[i] = float_to_fp16(dist);
    }

    // Prepare the distance result array (output is in the float format).
    float* distances = (float*)malloc(ncode * sizeof(float));

    // Perform accumulation based on 4-bit table lookup for fp16 vectors.
    uint16_t dis0 = float_to_fp16(0.0f); // The initial distance is 0.
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
        printf("Failed to perform accumulation based on 4-bit table lookup for fp16 vectors. Error code: %d\n", ret);
        goto cleanup;
    }

    printf("Successfully performed accumulation based on 4-bit table lookup for fp16 vectors\n");

    // Determine the minimum distance (nearest neighbor).
    float min_dist = distances[0];
    size_t min_idx = 0;
    for (size_t i = 1; i < ncode; i++) {
        if (distances[i] < min_dist) {
            min_dist = distances[i];
            min_idx = i;
        }
    }
    printf("Nearest neighbor: index = %zu, PQ distance = %f\n", min_idx, min_dist);

cleanup:
    free(codes);
    free(LUT);
    free(distances);

    return ret;
}
```

### krl\_pack\_codes\_4b

**Interface Definition <a name="section172317194488"></a>**

int krl\_pack\_codes\_4b\(const uint8\_t\* codes, size\_t ncode, size\_t nsq, uint8\_t\* blocks, size\_t batchsize, int dim\_cross, size\_t codes\_size, size\_t blocks\_size\);

**Function<a name="section1153124784912"></a>**

An operator designed for 4-bit table lookup, accumulation, filtering, and compression. It is used for processing fp16 query vectors individually. It computes distances between a query vector and multiple base vectors using inner product. The initial distance is <code>dis\_f16</code>. This interface does not perform filtering or compression (that is, comparison with the threshold).

**Parameters<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.541554155415543%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="14.611461146114612%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p14381721205612"><a name="p14381721205612"></a><a name="p14381721205612"></a>codes</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p7438122115569"><a name="p7438122115569"></a><a name="p7438122115569"></a>const uint8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p18438121155616"><a name="p18438121155616"></a><a name="p18438121155616"></a>Base vector data.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p13438102185617"><a name="p13438102185617"></a><a name="p13438102185617"></a>The size is specified by <code>codes_size</code>.</p>
</td>
</tr>
<tr id="row587315210197"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p14873021151914"><a name="p14873021151914"></a><a name="p14873021151914"></a>ncode</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p887382119197"><a name="p887382119197"></a><a name="p887382119197"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p287382118190"><a name="p287382118190"></a><a name="p287382118190"></a>Total number of base vectors.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p79885872519"><a name="p79885872519"></a><a name="p79885872519"></a>[1, 2^30-1]</p>
</td>
</tr>
<tr id="row18840143271918"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p4840832111916"><a name="p4840832111916"></a><a name="p4840832111916"></a>nsq</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p68401332181920"><a name="p68401332181920"></a><a name="p68401332181920"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p08401632111917"><a name="p08401632111917"></a><a name="p08401632111917"></a>Number of subspaces.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p20840123241914"><a name="p20840123241914"></a><a name="p20840123241914"></a>[1, 65535]</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p734604031220"><a name="p734604031220"></a><a name="p734604031220"></a>blocks</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p7532158856"><a name="p7532158856"></a><a name="p7532158856"></a>uint8_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p36611261054"><a name="p36611261054"></a><a name="p36611261054"></a>Packed base vector data.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>The size is specified by <code>blocks_size</code>. The memory needs to be allocated in advance.</p>
</td>
</tr>
<tr id="row103951453161513"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p14723141215409"><a name="p14723141215409"></a><a name="p14723141215409"></a>batchsize</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p4723181210404"><a name="p4723181210404"></a><a name="p4723181210404"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p672341218403"><a name="p672341218403"></a><a name="p672341218403"></a>Base vector block size.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p6723181274010"><a name="p6723181274010"></a><a name="p6723181274010"></a>The value is greater than 0 and is a multiple of 16. The value must match table lookup accumulation operators.</p>
<a name="ul1810376145316"></a><a name="ul1810376145316"></a><ul id="ul1810376145316"><li><code>32:</code></li></ul>
<p id="p2989163595213"><a name="p2989163595213"></a><a name="p2989163595213"></a>krl_table_lookup_step</p>
<a name="ul342518815320"></a><a name="ul342518815320"></a><ul id="ul342518815320"><li><code>64:</code></li></ul>
<p id="p19989135155218"><a name="p19989135155218"></a><a name="p19989135155218"></a>krl_L2_table_lookup_fast_scan_bs64</p>
<p id="p398933517522"><a name="p398933517522"></a><a name="p398933517522"></a>krl_IP_table_lookup_fast_scan_bs64</p>
<p id="p1998973515521"><a name="p1998973515521"></a><a name="p1998973515521"></a>krl_table_lookup_4b_f16</p>
<a name="ul13296171112536"></a><a name="ul13296171112536"></a><ul id="ul13296171112536"><li><code>96:</code></li></ul>
<p id="p3989203517528"><a name="p3989203517528"></a><a name="p3989203517528"></a>krl_L2_table_lookup_fast_scan_bs96</p>
<p id="p16989173512524"><a name="p16989173512524"></a><a name="p16989173512524"></a>krl_IP_table_lookup_fast_scan_bs96</p>
</td>
</tr>
<tr id="row1875218456372"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p564545281211"><a name="p564545281211"></a><a name="p564545281211"></a>dim_cross</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p7753045173714"><a name="p7753045173714"></a><a name="p7753045173714"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p17531445103716"><a name="p17531445103716"></a><a name="p17531445103716"></a>Indicates whether the distance data is 8-bit.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p69179904614"><a name="p69179904614"></a><a name="p69179904614"></a>[0, 1]</p>
<a name="ul164886121012"></a><a name="ul164886121012"></a><ul id="ul164886121012"><li><code>0</code>: The distance data is 8-bit. </li><li><code>1</code>: The distance data is 16-bit.</li></ul>
</td>
</tr>
<tr id="row67711025367"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p137414311617"><a name="p137414311617"></a><a name="p137414311617"></a>codes_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p06662231878"><a name="p06662231878"></a><a name="p06662231878"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p16744431269"><a name="p16744431269"></a><a name="p16744431269"></a>Size of the base vector array.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p127494317611"><a name="p127494317611"></a><a name="p127494317611"></a><code>ncode</code> x <code>nsq</code>/2</p>
</td>
</tr>
<tr id="row4903281565"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p292753515619"><a name="p292753515619"></a><a name="p292753515619"></a>blocks_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p15927335864"><a name="p15927335864"></a><a name="p15927335864"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p2927183515614"><a name="p2927183515614"></a><a name="p2927183515614"></a>Size of the packed base vector array.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p99271635566"><a name="p99271635566"></a><a name="p99271635566"></a>ceil(<code>ncode</code>/<code>batchsize</code>) x <code>batchsize</code> x ceil(<code>nsq</code>/2)</p>
</td>
</tr>
</tbody>
</table>

**Return Values<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a><code>0</code> is returned on successful execution. In case of failure, an error code is returned to indicate the specific issue.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c
#include <stdio.h>
#include <stdlib.h>
#include <math.h>
#include "krl.h"

int main() {
    // Parameter configuration
    size_t ncode = 10000; // Total number of base vectors
    size_t nsq = 64;        // Number of subspaces
    size_t batchsize = 64; // Block size (corresponding to the bs64 API)
    int dim_cross = 0; // Use the 8-bit distance.

    // Prepare the original 4-bit codebook.
    // Original format: Each vector has nsq 4-bit indexes.
    // During storage, every two 4-bit indexes are packed into one uint8.
    size_t codes_size = ncode * nsq / 2;
    uint8_t* codes = (uint8_t*)malloc(codes_size * sizeof(uint8_t));
    
    // Simulated original codebook data
    for (size_t i = 0; i < codes_size; i++) {
        uint8_t low = rand() % 16;   // Lower 4 bits: 0–15
        uint8_t high = rand() % 16;   // Higher 4 bits: 0–15
        codes[i] = (high << 4) | low;
    }

    // Calculate the size of the packed array.
    size_t num_blocks = (ncode + batchsize - 1) / batchsize;  // Round up.
    size_t blocks_size = num_blocks * batchsize * ((nsq + 1) / 2);
    uint8_t* blocks = (uint8_t*)malloc(blocks_size * sizeof(uint8_t));

    // Pack the codebook.
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
        printf("Failed to pack the codebook. Error code: %d\n", ret);
        goto cleanup;
    }

    printf("4-bit codebook packing succeeded\n");
    printf("  Original codebook size: %zu bytes\n", codes_size);
    printf("  Size after packing: %zu bytes\n", blocks_size);
    printf("  Block size: %zu\n", batchsize);
    printf("  Number of blocks: %zu\n", num_blocks);

    // Blocks are now available for fast table lookup.
    // Example: krl_L2_table_lookup_fast_scan_bs64 (...)

cleanup:
    free(codes);
    free(blocks);

    return ret;
}
```

## Reranking Interfaces

### krl\_reorder\_2\_vector

**Interface Definition <a name="section172317194488"></a>**

int krl\_reorder\_2\_vector\(const KRLDistanceHandle\* kdh, int64\_t base\_k, float\* base\_dis, int64\_t\* base\_idx, const float\* query\_vector, int64\_t k, float\* dis, int64\_t\* idx, size\_t query\_vector\_size\);

**Function<a name="section1153124784912"></a>**

Computes high-accuracy distances between a single query vector and multiple non-contiguous base vectors, and returns the results sorted by distance.

**Parameters<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.541554155415543%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="14.611461146114612%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="29.532953295329534%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="40.31403140314032%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p14381721205612"><a name="p14381721205612"></a><a name="p14381721205612"></a>kdh</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p7438122115569"><a name="p7438122115569"></a><a name="p7438122115569"></a>const KRLDistanceHandle*</p>
</td>
<td class="cellrowborder" valign="top" width="29.532953295329534%" headers="mcps1.1.5.1.3 "><p id="p18438121155616"><a name="p18438121155616"></a><a name="p18438121155616"></a>Pointer to a KRLDistanceHandle instance.</p>
</td>
<td class="cellrowborder" valign="top" width="40.31403140314032%" headers="mcps1.1.5.1.4 "><p id="p13438102185617"><a name="p13438102185617"></a><a name="p13438102185617"></a>The value cannot be null. This instance is initialized by krl_create_reorder_handle.</p>
</td>
</tr>
<tr id="row587315210197"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p14873021151914"><a name="p14873021151914"></a><a name="p14873021151914"></a>base_k</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p887382119197"><a name="p887382119197"></a><a name="p887382119197"></a>int64_t</p>
</td>
<td class="cellrowborder" valign="top" width="29.532953295329534%" headers="mcps1.1.5.1.3 "><p id="p287382118190"><a name="p287382118190"></a><a name="p287382118190"></a>The number of candidate points selected by a low-accuracy retrieval algorithm.</p>
</td>
<td class="cellrowborder" valign="top" width="40.31403140314032%" headers="mcps1.1.5.1.4 "><p id="p1487318214195"><a name="p1487318214195"></a><a name="p1487318214195"></a>It falls within [<code>k</code>, <code>codes_num</code>], where <code>codes_num</code> is the number of base vectors.</p>
</td>
</tr>
<tr id="row18840143271918"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p4840832111916"><a name="p4840832111916"></a><a name="p4840832111916"></a>base_dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p68401332181920"><a name="p68401332181920"></a><a name="p68401332181920"></a>float*</p>
</td>
<td class="cellrowborder" valign="top" width="29.532953295329534%" headers="mcps1.1.5.1.3 "><p id="p08401632111917"><a name="p08401632111917"></a><a name="p08401632111917"></a>Low-accuracy distance obtained using the low-accuracy retrieval algorithm.</p>
</td>
<td class="cellrowborder" valign="top" width="40.31403140314032%" headers="mcps1.1.5.1.4 "><p id="p20840123241914"><a name="p20840123241914"></a><a name="p20840123241914"></a>The size is specified by <code>base_k</code>.</p>
</td>
</tr>
<tr id="row10982132445420"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p734604031220"><a name="p734604031220"></a><a name="p734604031220"></a>base_idx</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p7532158856"><a name="p7532158856"></a><a name="p7532158856"></a>int64_t*</p>
</td>
<td class="cellrowborder" valign="top" width="29.532953295329534%" headers="mcps1.1.5.1.3 "><p id="p36611261054"><a name="p36611261054"></a><a name="p36611261054"></a>ID of the candidate point obtained using the low-accuracy retrieval algorithm.</p>
</td>
<td class="cellrowborder" valign="top" width="40.31403140314032%" headers="mcps1.1.5.1.4 "><p id="p85127581355"><a name="p85127581355"></a><a name="p85127581355"></a>The size is specified by <code>base_k</code>. It falls within [<code>-1</code>, <code>codes_num</code>]. The IDs increase monotonically. If a placeholder value of <code>-1</code> is used to indicate positions that should not be computed, those entries must be placed at the end of the vector array.</p>
</td>
</tr>
<tr id="row103951453161513"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p14723141215409"><a name="p14723141215409"></a><a name="p14723141215409"></a>query_vector</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p4723181210404"><a name="p4723181210404"></a><a name="p4723181210404"></a>const float*</p>
</td>
<td class="cellrowborder" valign="top" width="29.532953295329534%" headers="mcps1.1.5.1.3 "><p id="p672341218403"><a name="p672341218403"></a><a name="p672341218403"></a>Query vector data.</p>
</td>
<td class="cellrowborder" valign="top" width="40.31403140314032%" headers="mcps1.1.5.1.4 "><p id="p6723181274010"><a name="p6723181274010"></a><a name="p6723181274010"></a>The size is specified by <code>query_vector_size</code>.</p>
</td>
</tr>
<tr id="row1875218456372"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p564545281211"><a name="p564545281211"></a><a name="p564545281211"></a>k</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p7753045173714"><a name="p7753045173714"></a><a name="p7753045173714"></a>int64_t</p>
</td>
<td class="cellrowborder" valign="top" width="29.532953295329534%" headers="mcps1.1.5.1.3 "><p id="p164563717334"><a name="p164563717334"></a><a name="p164563717334"></a>Number of the nearest neighbors to return after computation.</p>
</td>
<td class="cellrowborder" valign="top" width="40.31403140314032%" headers="mcps1.1.5.1.4 "><p id="p10984160193814"><a name="p10984160193814"></a><a name="p10984160193814"></a>It falls within [<code>1</code>, <code>base_k</code>].</p>
</td>
</tr>
<tr id="row1959261153015"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p159201112305"><a name="p159201112305"></a><a name="p159201112305"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p95921611183016"><a name="p95921611183016"></a><a name="p95921611183016"></a>float*</p>
</td>
<td class="cellrowborder" valign="top" width="29.532953295329534%" headers="mcps1.1.5.1.3 "><p id="p5592171115307"><a name="p5592171115307"></a><a name="p5592171115307"></a>Stores the computed distances between the query vector and its nearest neighbors.</p>
</td>
<td class="cellrowborder" valign="top" width="40.31403140314032%" headers="mcps1.1.5.1.4 "><p id="p5592141183018"><a name="p5592141183018"></a><a name="p5592141183018"></a>The value is specified by <code>k</code>. The memory needs to be allocated in advance.</p>
</td>
</tr>
<tr id="row8439920305"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p1243209163013"><a name="p1243209163013"></a><a name="p1243209163013"></a>idx</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p174410973020"><a name="p174410973020"></a><a name="p174410973020"></a>int64_t*</p>
</td>
<td class="cellrowborder" valign="top" width="29.532953295329534%" headers="mcps1.1.5.1.3 "><p id="p344169173011"><a name="p344169173011"></a><a name="p344169173011"></a>Stores IDs of the nearest neighbors.</p>
</td>
<td class="cellrowborder" valign="top" width="40.31403140314032%" headers="mcps1.1.5.1.4 "><p id="p14445915305"><a name="p14445915305"></a><a name="p14445915305"></a>The value is specified by <code>k</code>. The memory needs to be allocated in advance.</p>
</td>
</tr>
<tr id="row76471455191816"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p16648125510182"><a name="p16648125510182"></a><a name="p16648125510182"></a>query_vector_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p11648125510182"><a name="p11648125510182"></a><a name="p11648125510182"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="29.532953295329534%" headers="mcps1.1.5.1.3 "><p id="p06484557186"><a name="p06484557186"></a><a name="p06484557186"></a>Size of the query vector array.</p>
</td>
<td class="cellrowborder" valign="top" width="40.31403140314032%" headers="mcps1.1.5.1.4 "><p id="p176481955171818"><a name="p176481955171818"></a><a name="p176481955171818"></a>The value is specified by <code>dim</code>, the vector dimension.</p>
</td>
</tr>
</tbody>
</table>

**Return Values<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a><code>0</code> is returned on successful execution. In case of failure, an error code is returned to indicate the specific issue.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

int main() {
    // Parameter configuration
    size_t dim = 128; // Vector dimension
    size_t codes_num = 100000;  // Total number of base vectors
    int64_t base_k = 100;       // Number of candidate points returned in low-accuracy retrieval
    int64_t k = 10;             // Final top-K result
    int metric_type = 0;        // 0: L2 distance

    // Prepare base vector data.
    float* base_vectors = (float*)malloc(codes_num * dim * sizeof(float));
    for (size_t i = 0; i < codes_num * dim; i++) {
        base_vectors[i] = (float)(rand() % 1000) / 100.0f;
    }

    // Reranking handle creation
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
        printf("Failed to create the reranking handle: %d\n", ret);
        free(base_vectors);
        return -1;
    }

    // Prepare the query vector.
    float* query_vector = (float*)malloc(dim * sizeof(float));
    for (size_t i = 0; i < dim; i++) {
        query_vector[i] = (float)(rand() % 1000) / 100.0f;
    }

    // Simulated low-accuracy retrieval results.
    // In actual use, these results are obtained using PQ or other approximate retrieval algorithms.
    float* base_dis = (float*)malloc(base_k * sizeof(float));
    int64_t* base_idx = (int64_t*)malloc(base_k * sizeof(int64_t));
    
    // Simulated candidate point IDs (which must increase monotonically).
    for (int64_t i = 0; i < base_k; i++) {
        base_idx[i] = i * 100;  // ID: 0, 100, 200, ...
        base_dis[i] = (float)(rand() % 10000) / 10.0f;  // Low-accuracy distance
    }

    // Allocate the result array.
    float* result_dis = (float*)malloc(k * sizeof(float));
    int64_t* result_idx = (int64_t*)malloc(k * sizeof(int64_t));

    // Perform high-accuracy reranking
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
        printf("Reranking computation failed. Error code: %d\n", ret);
        goto cleanup;
    }

    // Output the results.
    printf("High-accuracy reranking completed. Top-%lld results:\n", (long long)k);
    for (int64_t i = 0; i < k; i++) {
        printf("  Rank %lld: ID = %lld, high-accuracy distance = %f\n",
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

**Interface Definition <a name="section172317194488"></a>**

int krl\_reorder\_2\_vector\_continuous\(const KRLDistanceHandle\* kdh, int64\_t base\_k, int64\_t begin\_id, const float\* query\_vector, int64\_t k, float\* dis, int64\_t\* idx, size\_t query\_vector\_size\);

**Function<a name="section1153124784912"></a>**

Computes high-accuracy distances between a single query vector and multiple contiguous base vectors, and returns the results sorted by distance.

**Parameters<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.541554155415543%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="14.611461146114612%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p14381721205612"><a name="p14381721205612"></a><a name="p14381721205612"></a>kdh</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p7438122115569"><a name="p7438122115569"></a><a name="p7438122115569"></a>const KRLDistanceHandle*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p18438121155616"><a name="p18438121155616"></a><a name="p18438121155616"></a>Pointer to a KRLDistanceHandle instance.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p13438102185617"><a name="p13438102185617"></a><a name="p13438102185617"></a>It cannot be null, and is initialized using krl_create_reorder_handle.</p>
</td>
</tr>
<tr id="row587315210197"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p14873021151914"><a name="p14873021151914"></a><a name="p14873021151914"></a>base_k</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p887382119197"><a name="p887382119197"></a><a name="p887382119197"></a>int64_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p287382118190"><a name="p287382118190"></a><a name="p287382118190"></a>The number of candidate points selected by a low-accuracy retrieval algorithm.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1487318214195"><a name="p1487318214195"></a><a name="p1487318214195"></a>It falls within [<code>k</code>, <code>codes_num</code>], where <code>codes_num</code> is the number of base vectors.</p>
</td>
</tr>
<tr id="row18840143271918"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p4840832111916"><a name="p4840832111916"></a><a name="p4840832111916"></a>begin_id</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p68401332181920"><a name="p68401332181920"></a><a name="p68401332181920"></a>int64_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p08401632111917"><a name="p08401632111917"></a><a name="p08401632111917"></a>ID of the first base vector to be included in the computation.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p20840123241914"><a name="p20840123241914"></a><a name="p20840123241914"></a>[<code>0</code>, <code>codes_num-base_k</code>]</p>
</td>
</tr>
<tr id="row103951453161513"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p14723141215409"><a name="p14723141215409"></a><a name="p14723141215409"></a>query_vector</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p4723181210404"><a name="p4723181210404"></a><a name="p4723181210404"></a>const float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p672341218403"><a name="p672341218403"></a><a name="p672341218403"></a>Query vector data.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p6723181274010"><a name="p6723181274010"></a><a name="p6723181274010"></a>The size is specified by <code>query_vector_size</code>.</p>
</td>
</tr>
<tr id="row1875218456372"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p564545281211"><a name="p564545281211"></a><a name="p564545281211"></a>k</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p7753045173714"><a name="p7753045173714"></a><a name="p7753045173714"></a>int64_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p164563717334"><a name="p164563717334"></a><a name="p164563717334"></a>Number of the nearest neighbors to return after computation.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p10984160193814"><a name="p10984160193814"></a><a name="p10984160193814"></a>It falls within [<code>1</code>, <code>base_k</code>].</p>
</td>
</tr>
<tr id="row1959261153015"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p159201112305"><a name="p159201112305"></a><a name="p159201112305"></a>dis</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p95921611183016"><a name="p95921611183016"></a><a name="p95921611183016"></a>float*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p5592171115307"><a name="p5592171115307"></a><a name="p5592171115307"></a>Stores the computed distances between the query vector and its nearest neighbors.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p5592141183018"><a name="p5592141183018"></a><a name="p5592141183018"></a>The value is specified by <code>k</code>. The memory needs to be allocated in advance.</p>
</td>
</tr>
<tr id="row8439920305"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p1243209163013"><a name="p1243209163013"></a><a name="p1243209163013"></a>idx</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p174410973020"><a name="p174410973020"></a><a name="p174410973020"></a>int64_t*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p344169173011"><a name="p344169173011"></a><a name="p344169173011"></a>Stores IDs of the nearest neighbors.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p14445915305"><a name="p14445915305"></a><a name="p14445915305"></a>The value is specified by <code>k</code>. The memory needs to be allocated in advance.</p>
</td>
</tr>
<tr id="row355263412118"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p16648125510182"><a name="p16648125510182"></a><a name="p16648125510182"></a>query_vector_size</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p11648125510182"><a name="p11648125510182"></a><a name="p11648125510182"></a>size_t</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p06484557186"><a name="p06484557186"></a><a name="p06484557186"></a>Size of the query vector array.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p176481955171818"><a name="p176481955171818"></a><a name="p176481955171818"></a>The value is specified by <code>dim</code>, the vector dimension.</p>
</td>
</tr>
</tbody>
</table>

**Return Values<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a><code>0</code> is returned on successful execution. In case of failure, an error code is returned to indicate the specific issue.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

int main() {
    // Parameter configuration
    size_t dim = 128;
    size_t codes_num = 100000;
    int64_t base_k = 1000;      // Number of consecutive candidate points
    int64_t begin_id = 5000;    // Start ID (for example, the start position of a cluster)
    int64_t k = 10;             // Final top-k results 
    int metric_type = 0;        // L2 distance

    // Prepare base vectors.
    float* base_vectors = (float*)malloc(codes_num * dim * sizeof(float));
    for (size_t i = 0; i < codes_num * dim; i++) {
        base_vectors[i] = (float)(rand() % 1000) / 100.0f;
    }

    // Reranking handle creation
    KRLDistanceHandle* kdh = NULL;
    int ret = krl_create_reorder_handle(
        &kdh, base_vectors, codes_num, dim, metric_type, codes_num * dim
    );
    if (ret != 0) {
        printf("Failed to create the reranking handle: %d\n", ret);
        free(base_vectors);
        return -1;
    }

    // Prepare the query vector.
    float* query_vector = (float*)malloc(dim * sizeof(float));
    for (size_t i = 0; i < dim; i++) {
        query_vector[i] = (float)(rand() % 1000) / 100.0f;
    }

    // Allocate the result array.
    float* result_dis = (float*)malloc(k * sizeof(float));
    int64_t* result_idx = (int64_t*)malloc(k * sizeof(int64_t));

    // Perform high-accuracy reranking of consecutive vectors.
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
        printf("Computation for consecutive vector reranking failed. Error code: %d\n", ret);
        goto cleanup;
    }

    // Output the results.
    printf("Consecutive vector reranking completed.\n");
    printf("Search range: ID [%lld, %lld)\n",
           (long long)begin_id,
           (long long)(begin_id + base_k));
    printf("Top-%lld results:\n", (long long)k);
    for (int64_t i = 0; i < k; i++) {
        printf("  Rank %lld: ID = %lld, distance = %f\n",
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

## Store/Load Interfaces

### krl\_store\_LUT8Handle

**Interface Definition <a name="section172317194488"></a>**

int krl\_store\_LUT8Handle\(FILE\* f, const KRLLUT8bHandle\* klh\);

**Function<a name="section1153124784912"></a>**

Stores the handle of an 8-bit lookup table into a file.

**Parameters<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.541554155415543%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="14.611461146114612%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p14381721205612"><a name="p14381721205612"></a><a name="p14381721205612"></a>f</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p7438122115569"><a name="p7438122115569"></a><a name="p7438122115569"></a>FILE*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p1018720320568"><a name="p1018720320568"></a><a name="p1018720320568"></a>Handle to a file opened for writing.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p4187123185620"><a name="p4187123185620"></a><a name="p4187123185620"></a>The value cannot be null.</p>
</td>
</tr>
<tr id="row587315210197"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p14873021151914"><a name="p14873021151914"></a><a name="p14873021151914"></a>klh</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p887382119197"><a name="p887382119197"></a><a name="p887382119197"></a>const KRLLUT8bHandle*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p287382118190"><a name="p287382118190"></a><a name="p287382118190"></a>Pointer to the KRLLUT8bHandle instance.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1487318214195"><a name="p1487318214195"></a><a name="p1487318214195"></a>The value cannot be null.</p>
</td>
</tr>
</tbody>
</table>

**Return Values<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a><code>0</code> is returned on successful execution. In case of failure, an error code is returned to indicate the specific issue.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

// Save the handle to a file.
int save_lut8_handle(const char* filename, KRLLUT8bHandle* klh) {
    FILE* f = fopen(filename, "wb");
    if (f == NULL) {
        printf("Failed to open the file for writing: %s\n", filename);
        return -1;
    }

    int ret = krl_store_LUT8Handle(f, klh);
    fclose(f);

    if (ret == 0) {
        printf("LUT8bHandle saved to: %s\n", filename);
    } else {
        printf("Failed to save the file. Error code: %d\n", ret);
    }
    return ret;
}

// Load the handle from a file.
int load_lut8_handle(const char* filename, KRLLUT8bHandle** klh) {
    FILE* f = fopen(filename, "rb");
    if (f == NULL) {
        printf("Failed to open the file for reading: %s\n", filename);
        return -1;
    }

    int ret = krl_build_LUT8Handle_fromfile(f, klh);
    fclose(f);

    if (ret == 0) {
        printf("LUT8bHandle has been loaded from the file: %s\n", filename);
    } else {
        printf("Loading failed. Error code: %d\n", ret);
    }
    return ret;
}

int main() {
    const char* filename = "lut8_handle.bin";
    
    // Create and initialize a handle.
    KRLLUT8bHandle* klh = NULL;
    int use_idx = 1;
    size_t capacity = 10000;
    
    int ret = krl_create_LUT8b_handle(&klh, use_idx, capacity);
    if (ret != 0) {
        printf("Failed to create the handle.\n");
        return -1;
    }

    // Set some data.
    size_t* idx_ptr = krl_get_idx_pointer(klh);
    for (size_t i = 0; i < 100; i++) {
        idx_ptr[i] = i * 10;
    }

    // Save the handle.
    ret = save_lut8_handle(filename, klh);
    if (ret != 0) {
        krl_clean_LUT8b_handle(&klh);
        return -1;
    }

    // Clean up the original handle.
    krl_clean_LUT8b_handle(&klh);
    klh = NULL;

    // Reload from the file.
    ret = load_lut8_handle(filename, &klh);
    if (ret != 0) {
        return -1;
    }

    // Verify the loaded data.
    size_t* loaded_idx = krl_get_idx_pointer(klh);
    printf ("Verify the loaded data:\n");
    for (size_t i = 0; i < 5; i++) {
        printf("  idx[%zu] = %zu\n", i, loaded_idx[i]);
    }

    // Cleanup
    krl_clean_LUT8b_handle(&klh);
    
    return 0;
}
```

### krl\_build\_LUT8Handle\_fromfile

**Interface Definition <a name="section172317194488"></a>**

int krl\_build\_LUT8Handle\_fromfile\(FILE\* f, KRLLUT8bHandle\*\* klh\);

**Function<a name="section1153124784912"></a>**

Reads data of an 8-bit lookup table from a file and rebuilds a handle.

**Parameters<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.541554155415543%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="14.611461146114612%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p14381721205612"><a name="p14381721205612"></a><a name="p14381721205612"></a>f</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p7438122115569"><a name="p7438122115569"></a><a name="p7438122115569"></a>FILE*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p6717120145712"><a name="p6717120145712"></a><a name="p6717120145712"></a>Handle to a file opened for reading.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p4187123185620"><a name="p4187123185620"></a><a name="p4187123185620"></a>The value cannot be null.</p>
</td>
</tr>
<tr id="row587315210197"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p14873021151914"><a name="p14873021151914"></a><a name="p14873021151914"></a>klh</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p887382119197"><a name="p887382119197"></a><a name="p887382119197"></a>KRLLUT8bHandle*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p287382118190"><a name="p287382118190"></a><a name="p287382118190"></a>Pointer to the KRLLUT8bHandle instance.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1487318214195"><a name="p1487318214195"></a><a name="p1487318214195"></a>The value cannot be null.</p>
</td>
</tr>
</tbody>
</table>

**Return Values<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a><code>0</code> is returned on successful execution. In case of failure, an error code is returned to indicate the specific issue.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

// Save the handle to a file.
int save_lut8_handle(const char* filename, KRLLUT8bHandle* klh) {
    FILE* f = fopen(filename, "wb");
    if (f == NULL) {
        printf("Failed to open the file for writing: %s\n", filename);
        return -1;
    }

    int ret = krl_store_LUT8Handle(f, klh);
    fclose(f);

    if (ret == 0) {
        printf("LUT8bHandle saved to: %s\n", filename);
    } else {
        printf("Failed to save the file. Error code: %d\n", ret);
    }
    return ret;
}

// Load the handle from a file.
int load_lut8_handle(const char* filename, KRLLUT8bHandle** klh) {
    FILE* f = fopen(filename, "rb");
    if (f == NULL) {
        printf("Failed to open the file for reading: %s\n", filename);
        return -1;
    }

    int ret = krl_build_LUT8Handle_fromfile(f, klh);
    fclose(f);

    if (ret == 0) {
        printf("LUT8bHandle has been loaded from the file: %s\n", filename);
    } else {
        printf("Loading failed. Error code: %d\n", ret);
    }
    return ret;
}

int main() {
    const char* filename = "lut8_handle.bin";
    
    // Create and initialize a handle.
    KRLLUT8bHandle* klh = NULL;
    int use_idx = 1;
    size_t capacity = 10000;
    
    int ret = krl_create_LUT8b_handle(&klh, use_idx, capacity);
    if (ret != 0) {
        printf("Failed to create the handle.\n");
        return -1;
    }

    // Set some data.
    size_t* idx_ptr = krl_get_idx_pointer(klh);
    for (size_t i = 0; i < 100; i++) {
        idx_ptr[i] = i * 10;
    }

    // Save the handle.
    ret = save_lut8_handle(filename, klh);
    if (ret != 0) {
        krl_clean_LUT8b_handle(&klh);
        return -1;
    }

    // Clean up the original handle.
    krl_clean_LUT8b_handle(&klh);
    klh = NULL;

    // Reload from the file.
    ret = load_lut8_handle(filename, &klh);
    if (ret != 0) {
        return -1;
    }

    // Verify the loaded data.
    size_t* loaded_idx = krl_get_idx_pointer(klh);
    printf ("Verify the loaded data:\n");
    for (size_t i = 0; i < 5; i++) {
        printf("  idx[%zu] = %zu\n", i, loaded_idx[i]);
    }

    // Clean up
    krl_clean_LUT8b_handle(&klh);
    
    return 0;
}
```

### krl\_store\_distanceHandle

**Interface Definition <a name="section172317194488"></a>**

int krl\_store\_distanceHandle\(FILE\* f, const KRLDistanceHandle\* kdh\);

**Function<a name="section1153124784912"></a>**

Stores the handle for distance computation into a file.

**Parameters<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.541554155415543%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="14.611461146114612%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p14381721205612"><a name="p14381721205612"></a><a name="p14381721205612"></a>f</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p7438122115569"><a name="p7438122115569"></a><a name="p7438122115569"></a>FILE*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p1018720320568"><a name="p1018720320568"></a><a name="p1018720320568"></a>Handle to a file opened for writing.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p4187123185620"><a name="p4187123185620"></a><a name="p4187123185620"></a>The value cannot be null.</p>
</td>
</tr>
<tr id="row587315210197"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p123371053104616"><a name="p123371053104616"></a><a name="p123371053104616"></a>kdh</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p9468096466"><a name="p9468096466"></a><a name="p9468096466"></a>const KRLDistanceHandle*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p287382118190"><a name="p287382118190"></a><a name="p287382118190"></a>Pointer to the KRLDistanceHandle instance.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1487318214195"><a name="p1487318214195"></a><a name="p1487318214195"></a>The value cannot be null.</p>
</td>
</tr>
</tbody>
</table>

**Return Values<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a><code>0</code> is returned on successful execution. In case of failure, an error code is returned to indicate the specific issue.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

int main() {
    const char* filename = "distance_handle.bin";
    
    // Parameter configuration
    size_t dim = 128;
    size_t ny = 10000;
    int metric_type = 0;  // L2 distance

    // Prepare base vectors.
    float* base_vectors = (float*)malloc(ny * dim * sizeof(float));
    for (size_t i = 0; i < ny * dim; i++) {
        base_vectors[i] = (float)(rand() % 1000) / 100.0f;
    }

    // Create a handle.
    KRLDistanceHandle* kdh = NULL;
    int ret = krl_create_distance_handle(
        &kdh, base_vectors, ny, dim, metric_type, ny * dim
    );
    if (ret != 0) {
        printf("Failed to create DistanceHandle.\n");
        free(base_vectors);
        return -1;
    }

    // Save the handle to a file.
    FILE* f_write = fopen(filename, "wb");
    if (f_write == NULL) {
        printf ("Failed to open the file for writing.\n");
        krl_clean_distance_handle(&kdh);
        free(base_vectors);
        return -1;
    }

    ret = krl_store_distanceHandle(f_write, kdh);
    fclose(f_write);
    
    if (ret != 0) {
        printf("Failed to save the DistanceHandle: %d\n", ret);
        krl_clean_distance_handle(&kdh);
        free(base_vectors);
        return -1;
    }
    printf("DistanceHandle saved to: %s\n", filename);

    // Clean up the original handle.
    krl_clean_distance_handle(&kdh);
    kdh = NULL;

    // Load a handle from the file.
    FILE* f_read = fopen(filename, "rb");
    if (f_read == NULL) {
        printf ("Failed to open the file for reading\n");
        free(base_vectors);
        return -1;
    }

    ret = krl_build_distanceHandle_fromfile(f_read, &kdh);
    fclose(f_read);

    if (ret != 0) {
        printf("Failed to load DistanceHandle: %d\n", ret);
        free(base_vectors);
        return -1;
    }
    printf ("DistanceHandle has been loaded from the file\n");

    // Use the loaded handle to compute the distance.
    float* query = (float*)malloc(dim * sizeof(float));
    for (size_t i = 0; i < dim; i++) {
        query[i] = (float)(rand() % 1000) / 100.0f;
    }

    float distance;
    ret = krl_L2sqr_with_handle(kdh, query, 0, &distance, dim);
    if (ret == 0) {
        printf("Successfully computed the distance using the loaded handle: %f\n", distance);
    }

    // Cleanup
    krl_clean_distance_handle(&kdh);
    free(base_vectors);
    free(query);

    return 0;
}
```

### krl\_build\_distanceHandle\_fromfile

**Interface Definition <a name="section172317194488"></a>**

int krl\_build\_distanceHandle\_fromfile\(FILE\* f, KRLDistanceHandle\*\* kdh\);

**Function<a name="section1153124784912"></a>**

Reads data of a distance computation handle from a file and rebuilds the handle.

**Parameters<a name="section157501312135019"></a>**

<a name="table1623016332509"></a>
<table><thead align="left"><tr id="row823063355012"><th class="cellrowborder" valign="top" width="15.541554155415543%" id="mcps1.1.5.1.1"><p id="p1230333125010"><a name="p1230333125010"></a><a name="p1230333125010"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="14.611461146114612%" id="mcps1.1.5.1.2"><p id="p089311158912"><a name="p089311158912"></a><a name="p089311158912"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="33.99339933993399%" id="mcps1.1.5.1.3"><p id="p4230193313507"><a name="p4230193313507"></a><a name="p4230193313507"></a>Description</p>
</th>
<th class="cellrowborder" valign="top" width="35.85358535853585%" id="mcps1.1.5.1.4"><p id="p19887819256"><a name="p19887819256"></a><a name="p19887819256"></a>Value Range</p>
</th>
</tr>
</thead>
<tbody><tr id="row1823023318504"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p14381721205612"><a name="p14381721205612"></a><a name="p14381721205612"></a>f</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p7438122115569"><a name="p7438122115569"></a><a name="p7438122115569"></a>FILE*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p6717120145712"><a name="p6717120145712"></a><a name="p6717120145712"></a>Handle to a file opened for reading.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p4187123185620"><a name="p4187123185620"></a><a name="p4187123185620"></a>The value cannot be null.</p>
</td>
</tr>
<tr id="row587315210197"><td class="cellrowborder" valign="top" width="15.541554155415543%" headers="mcps1.1.5.1.1 "><p id="p123371053104616"><a name="p123371053104616"></a><a name="p123371053104616"></a>kdh</p>
</td>
<td class="cellrowborder" valign="top" width="14.611461146114612%" headers="mcps1.1.5.1.2 "><p id="p9468096466"><a name="p9468096466"></a><a name="p9468096466"></a>const KRLDistanceHandle*</p>
</td>
<td class="cellrowborder" valign="top" width="33.99339933993399%" headers="mcps1.1.5.1.3 "><p id="p287382118190"><a name="p287382118190"></a><a name="p287382118190"></a>Pointer to the KRLDistanceHandle instance.</p>
</td>
<td class="cellrowborder" valign="top" width="35.85358535853585%" headers="mcps1.1.5.1.4 "><p id="p1487318214195"><a name="p1487318214195"></a><a name="p1487318214195"></a>The value cannot be null.</p>
</td>
</tr>
</tbody>
</table>

**Return Values<a name="section49971832106"></a>**

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>Data Type</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a><code>0</code> is returned on successful execution. In case of failure, an error code is returned to indicate the specific issue.</p>
</td>
</tr>
</tbody>
</table>

## Error Codes

<a name="table17997635100"></a>
<table><thead align="left"><tr id="row699763141018"><th class="cellrowborder" valign="top" width="40%" id="mcps1.1.3.1.1"><p id="p699793141012"><a name="p699793141012"></a><a name="p699793141012"></a>Error code</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.1.3.1.2"><p id="p1999763141020"><a name="p1999763141020"></a><a name="p1999763141020"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row1599716361015"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p39970319101"><a name="p39970319101"></a><a name="p39970319101"></a>0</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p53461032104518"><a name="p53461032104518"></a><a name="p53461032104518"></a><code>0</code> is returned on successful execution.</p>
</td>
</tr>
<tr id="row2932411194415"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p99338112449"><a name="p99338112449"></a><a name="p99338112449"></a>-1</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p8763115484411"><a name="p8763115484411"></a><a name="p8763115484411"></a>Invalid pointer.</p>
</td>
</tr>
<tr id="row1410418141442"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p810461414413"><a name="p810461414413"></a><a name="p810461414413"></a>-2</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p7104191418447"><a name="p7104191418447"></a><a name="p7104191418447"></a>Memory allocation failure.</p>
</td>
</tr>
<tr id="row628451718442"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p2028411717447"><a name="p2028411717447"></a><a name="p2028411717447"></a>-3</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p728431784411"><a name="p728431784411"></a><a name="p728431784411"></a>Invalid input parameter.</p>
</td>
</tr>
<tr id="row3524122294419"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p20524162216440"><a name="p20524162216440"></a><a name="p20524162216440"></a>-4</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p18524122210449"><a name="p18524122210449"></a><a name="p18524122210449"></a>Double free.</p>
</td>
</tr>
<tr id="row8864111915443"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p0864219184413"><a name="p0864219184413"></a><a name="p0864219184413"></a>-5</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p786412199445"><a name="p786412199445"></a><a name="p786412199445"></a>Insecure memory operation.</p>
</td>
</tr>
<tr id="row114641147134412"><td class="cellrowborder" valign="top" width="40%" headers="mcps1.1.3.1.1 "><p id="p746415479447"><a name="p746415479447"></a><a name="p746415479447"></a>-6</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.1.3.1.2 "><p id="p14640472441"><a name="p14640472441"></a><a name="p14640472441"></a>I/O failure.</p>
</td>
</tr>
</tbody>
</table>

**Example**

```c
#include <stdio.h>
#include <stdlib.h>
#include "krl.h"

int main() {
    const char* filename = "distance_handle.bin";
    
    // Parameter configuration
    size_t dim = 128;
    size_t ny = 10000;
    int metric_type = 0;  // L2 distance

    // Prepare base vectors.
    float* base_vectors = (float*)malloc(ny * dim * sizeof(float));
    for (size_t i = 0; i < ny * dim; i++) {
        base_vectors[i] = (float)(rand() % 1000) / 100.0f;
    }

    // Handle creation
    KRLDistanceHandle* kdh = NULL;
    int ret = krl_create_distance_handle(
        &kdh, base_vectors, ny, dim, metric_type, ny * dim
    );
    if (ret != 0) {
        printf("Failed to create DistanceHandle.\n");
        free(base_vectors);
        return -1;
    }

    // Save the handle to a file.
    FILE* f_write = fopen(filename, "wb");
    if (f_write == NULL) {
        printf ("Failed to open the file for writing.\n");
        krl_clean_distance_handle(&kdh);
        free(base_vectors);
        return -1;
    }

    ret = krl_store_distanceHandle(f_write, kdh);
    fclose(f_write);
    
    if (ret != 0) {
        printf("Failed to save the DistanceHandle: %d\n", ret);
        krl_clean_distance_handle(&kdh);
        free(base_vectors);
        return -1;
    }
    printf("DistanceHandle saved to: %s\n", filename);

    // Clean up the original handle.
    krl_clean_distance_handle(&kdh);
    kdh = NULL;

    // Load a handle from the file.
    FILE* f_read = fopen(filename, "rb");
    if (f_read == NULL) {
        printf ("Failed to open the file for reading\n");
        free(base_vectors);
        return -1;
    }

    ret = krl_build_distanceHandle_fromfile(f_read, &kdh);
    fclose(f_read);

    if (ret != 0) {
        printf("Failed to load DistanceHandle: %d\n", ret);
        free(base_vectors);
        return -1;
    }
    printf ("DistanceHandle has been loaded from the file\n");

    // Use the loaded handle to compute the distance.
    float* query = (float*)malloc(dim * sizeof(float));
    for (size_t i = 0; i < dim; i++) {
        query[i] = (float)(rand() % 1000) / 100.0f;
    }

    float distance;
    ret = krl_L2sqr_with_handle(kdh, query, 0, &distance, dim);
    if (ret == 0) {
        printf("Successfully computed the distance using the loaded handle: %f\n", distance);
    }

    // Cleanup
    krl_clean_distance_handle(&kdh);
    free(base_vectors);
    free(query);

    return 0;
}
```
