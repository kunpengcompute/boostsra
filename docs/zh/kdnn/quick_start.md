# 快速入门

## 前提条件

使用本指导运行功能验证和调用示例步骤时，请先参见《[安装指南](./installation_guide.md)》完成KDNN的安装。

## 功能验证

编译后进入`out/test/dnn/llt/scripts`目录，执行以下命令运行算子用例。

```bash
python run_daily_build.py  
```

如果用例全部passed，说明验证成功。

## 单算子接口调用示例

编译后的可执行程序是`out/test/dnn/oneDNN-3.4/build/tests/benchdnn/benchdnn`，可以使用benchdnn验证KDNN算子功能以及性能，以matmul算子为例。

```bash
./benchdnn --mode=P --matmul --perf-template=Gflops:%0Gflops% --stag=ab --wtag=ab --dtag=ab 128x2048:2048x1024_n"googlenet_v1:ip1*1"
```
