# Quick Start

<!-- md-trans-meta sourceCommit=24bb37cb43d173905925eb7242ca1677ac105f2f translatedAt=2026-11-12T08:58:34.403Z pushedAt=2026-11-13T01:07:09.483Z -->

This document describes how to get started with KDNN, covering prerequisites for installation, functional verification, and a single-operator API calling example, for users who need a quick start.

## Prerequisites

Before running the functional verification and example invocation steps in this document, please first refer to [Installation Guide](./installation_guide.md) to complete KDNN installation.

## Function Verification

After compilation, go to the <code>out/test/dnn/llt/scripts</code> directory and run the following command to run the operator test cases:

```bash
python run_daily_build.py  
```

If all test cases pass, the verification is successful.

## Single-Operator API Calling Example

The built executable program is `out/test/dnn/oneDNN-3.4/build/tests/benchdnn/benchdnn`. You can use `benchdnn` to verify the functionality and performance of the KDNN operators. The following uses the Matmul operator as an example.

```bash
./benchdnn --mode=P --matmul --perf-template=Gflops:%0Gflops% --stag=ab --wtag=ab --dtag=ab 128x2048:2048x1024_n"googlenet_v1:ip1*1"
```
