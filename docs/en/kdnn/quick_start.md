# Quick Start

## Prerequisites

When running the functional verification and example invocation steps using this guide, please first refer to the [Installation Guide](./installation_guide.md) to complete the KDNN installation.

## Function Verification

After compilation, go to the <code>out/test/dnn/llt/scripts</code> directory and run the following command to run the operator test cases:

```bash
python run_daily_build.py  
```

If the execution results of all test cases are passed, the verification is successful.

## Single-Operator API Calling Example

The built executable program is `out/test/dnn/oneDNN-3.4/build/tests/benchdnn/benchdnn`. You can use `benchdnn` to verify the functionality and performance of the KDNN operators. The following uses the Matmul operator as an example.

```bash
./benchdnn --mode=P --matmul --perf-template=Gflops:%0Gflops% --stag=ab --wtag=ab --dtag=ab 128x2048:2048x1024_n"googlenet_v1:ip1*1"
```
