# Release Notes

## Version Mapping

### Product Version

<a name="table62675726"></a>
<table><tbody><tr id="row41561572"><th class="firstcol" valign="top" width="42.17%" id="mcps1.1.3.1.1"><p id="p11044137"><a name="p11044137"></a><a name="p11044137"></a>Product Name</p></th>
<td class="cellrowborder" valign="top" width="57.830000000000005%" headers="mcps1.1.3.1.1 "><p id="p1597721693713"><a name="p1597721693713"></a><a name="p1597721693713"></a>Kunpeng BoostKit</p></td>
</tr>
<tr id="row24726251"><th class="firstcol" valign="top" width="42.17%" id="mcps1.1.3.2.1"><p id="p56669300"><a name="p56669300"></a><a name="p56669300"></a>Product Version</p></th>
<td class="cellrowborder" valign="top" width="57.830000000000005%" headers="mcps1.1.3.2.1 "><p id="p13967181113316"><a name="p13967181113316"></a><a name="p13967181113316"></a><span id="text03501914183312"><a name="text03501914183312"></a><a name="text03501914183312"></a>26.2.RC1</span></p></td>
</tr>
<tr id="row1930811171892"><th class="firstcol" valign="top" width="42.17%" id="mcps1.1.3.3.1"><p id="p2030912172097"><a name="p2030912172097"></a><a name="p2030912172097"></a>Software Name</p></th>
<td class="cellrowborder" valign="top" width="57.830000000000005%" headers="mcps1.1.3.3.1 "><p id="p1730912179911"><a name="p1730912179911"></a><a name="p1730912179911"></a>Kunpeng AI Operator Library (Kunpeng AI<strong id="b166665341595"><a name="b166665341595"></a><a name="b166665341595"></a> </strong>Library)</p></td>
</tr>
<tr id="row5497143514612"><th class="firstcol" valign="top" width="42.17%" id="mcps1.1.3.4.1"><p id="p162251517551"><a name="p162251517551"></a><a name="p162251517551"></a>Software Version</p></th>
<td class="cellrowborder" valign="top" width="57.830000000000005%" headers="mcps1.1.3.4.1 "><p id="p6225131165519"><a name="p6225131165519"></a><a name="p6225131165519"></a>V3.2.0</p></td>
</tr>
</tbody>
</table>

### OS, Compiler, and CPU

**Table 1** Verified environments for KDNN<a id="verified-environments-for-kdnn"></a>

<a name="table59918346913"></a>

| Component | OS | CPU | Compiler | Build Tool | Python Interpreter |
|---|---|---|---|---|---|
| KDNN | openEuler 22.03 LTS SP3 | New Kunpeng 920 processor model | GCC 10.3.1 | CMake 3.22.0 | Python 3.9.21 |
| KDNN | openEuler 22.03 LTS SP4<br>(kernel version later than 5.10.0-228.0.0.127) | New Kunpeng 920 processor model | GCC 12.3.1/BiSheng 4.2.0 | CMake 3.22.0 | Python 3.9.21 |
| KDNN_EXT | openEuler 22.03 LTS SP3 | Kunpeng 920 processors | GCC 10.3.1 | CMake 3.22.0 | Python 3.9.20 |

### Virus Scan Results

The software packages, release documents, and product documents have been scanned by multiple antivirus software, and no virus is found. The virus scan results are as follows.

<a name="table1980419519233"></a>

| Antivirus Software | Antivirus Software Version | Virus Database Version | Scan Time | Scan Result |
|---|---|---|---|---|
| QiAnXin | 8.0.5.5260 | 2026-09-27 08:00:00.0 | 2026-09-28 16:02:00 | OK |
| Bitdefender | 7.5.1.200224 | 7.101487 | 2026-09-28 16:02:08 | OK |
| Kaspersky | 12.0.0.6672 | 2026-09-28 10:09:00 | 2026-09-28 16:02:02 | OK |

## V3.2.0

### Change Description

**New Features**

| Feature | Description |
|---|---|
| KDNN | <ul><li>Added thread pool parallelism support for SparseGemm.</li><li>Added a small-matrix GEMM optimization implementation.</li><li>Continuously optimized the performance of MatMul, convolution, and related operators on the Kunpeng platform.</li></ul> |

### Resolved Issues

None

### Known Issues

None

## V3.1.0

### Change Description

**New Features**

| Feature | Description |
|---|---|
| KDNN | <ul><li>Added MatMul implementation for s8/u8 data types based on MMLA instructions.</li><li>Added support for post-processing operation.</li><li>Added support for the FusedMatMul operator.</li></ul> |

### Resolved Issues

None

### Known Issues

None

## V3.0.0

### Change Description

**New Features<a name="section11862975"></a>**

<a name="table41916133"></a>

| Feature | Description |
|---|---|
| KDNN | <ul><li>Added NEON implementation for MatMul.</li><li>Added support for a custom thread pool mode in MatMul.</li><li>Added Kunpeng platform support for the deep neural network operators Group Normalization and SparseGemm.</li></ul> |

### Resolved Issues

None

### Known Issues

None

## V2.0.0

### Change Description

**New Features<a name="section11862975"></a>**

<a name="table41916133"></a>

| Feature | Description |
|---|---|
| KDNN | <ul><li>Added Kunpeng platform support for the Pool, Batch Normalization, Local Response Normalization, Reduction, PReLU, Binary, and RNN deep neural network operators.</li><li>Added support for the new Kunpeng 920 processor model.</li></ul> |

### Resolved Issues

None

### Known Issues

None

## V1.1.0

### Change Description

**New Features<a name="section11862975"></a>**

<a name="table41916133"></a>

| Feature | Description |
|---|---|
| KDNN | Added Kunpeng platform support for four deep neural network operators, including Reorder, Resampling, Concat, and Shuffle. |

### Resolved Issues

None

### Known Issues

None

## V1.0.0

### Change Description

**New Features<a name="section11862975"></a>**

<a name="table41916133"></a>

| Feature | Description |
|---|---|
| KDNN | Added Kunpeng platform support for seven deep neural network operators. |
| KDNN_EXT | Added Kunpeng platform support for the random_choice and softmax operators. |

### Resolved Issues

None

### Known Issues

None

## Related Documentation

### V3.2.0 Documentation

<a name="table41916133"></a>

| Document Name | Description | Delivery Method |
|---|---|---|
| [Release Notes](./release_notes.md) | Provides version release information of KDNN. | Open-source repository |
| [Quick Start](./quick_start.md) | Provides guidance for getting started with KDNN. | Open-source repository |
| [Installation Guide](./installation_guide.md) | Describes how to install and deploy KDNN. | Open-source repository |
| [API Reference](./api_reference.md) | Provides definitions, descriptions, and calling examples of KDNN APIs. | Open-source repository |
| [Best Practices](./best_practices.md) | Provides best practices of using KDNN. | Open-source repository |

### Obtaining Documentation

Visit the [open-source repository](./README_en.md) to view or download related documents.
