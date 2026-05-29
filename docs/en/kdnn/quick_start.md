# Quick Start

## Function Verification

After compilation, go to the <code>out/test/dnn/llt/scripts</code> directory and run the following command to run the operator test cases:

```bash
python run_daily_build.py  
```

If the execution results of all test cases are <code>passed</code>, the verification is successful.

## Single-Operator API Calling Example

The built executable program is <code>out/test/dnn/oneDNN-3.4/build/tests/benchdnn/benchdnn</code>. You can use <code>benchdnn</code> to verify the functionality and performance of the kdnn operators. The following uses the Matmul operator as an example.

```bash
./benchdnn --mode=P --matmul --perf-template=Gflops:%0Gflops% --stag=ab --wtag=ab --dtag=ab 128x2048:2048x1024_n"googlenet_v1:ip1*1"
```
