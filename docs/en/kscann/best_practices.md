# Best Practices

## Python

This section provides details on how to call the KScaNN algorithm API in Python. In the example, the `sift-128-euclidean.hdf5` dataset is used. Before calling the APIs, ensure that KScaNN has been installed.

**Obtaining the Test Code<a name="section25419211384"></a>**

Obtain the test framework code from the source code downloaded from [GitCode](https://atomgit.com/openeuler/sra_scann_adapter.git). The tag is `v2.2.1`. Assume that the source code is stored in `/path/to/scann/sra_scann_adapter` and the test framework code is stored in `/path/to/scann/sra_scann_adapter/ann-benchmarks`. Obtain datasets.

```bash
cd /path/to/scann/sra_scann_adapter/ann-benchmarks
mkdir data && cd data
wget http://ann-benchmarks.com/sift-128-euclidean.hdf5 --no-check-certificate
```

The directory structure of the main files is as follows:

```text
├── data                                                    // Stores the datasets.
      └── sift-128-euclidean.hdf5
├── ann_benchmarks
      └── algorithms
            └── scann
                  └── config-sift-128-euclidean.yml         // Dataset configuration file
└── test.sh                                                 // Test script
```

**Test Procedure<a name="section25072475424"></a>**

1. Verify that `scann-1.2.10-cp39-cp39-linux_aarch64.whl` has been installed as described in [Installation Guide](./installation_guide.md).

2. Install the dependencies required by `ann-benchmarks`.

    ```bash
    cd /path/to/scann/sra_scann_adapter/ann-benchmarks
    pip install -r requirements.txt
    yum install numactl numactl-devel
    ```

3. Run the test script.

    ```bash
    sh test.sh 
    ```

The test result is as follows:

<img src="figures/best_practices-python.jpg" alt="best_practices-python" width="1000"/>

## C++

This section provides details on how to call the KScaNN algorithm API in C++. In the example, the `sift-128-euclidean.hdf5` dataset is used. Before calling the APIs, ensure that KScaNN has been installed.

**Obtaining Datasets and Test Code<a name="section155352047153818"></a>**

Obtain the test framework code from the source code downloaded from [GitCode](https://atomgit.com/openeuler/sra_scann_adapter.git). Assume that the source code is stored in `/path/to/scann/sra_scann_adapter` and the test framework code is stored in `/path/to/scann/sra_scann_adapter/ann-benchmarks`.

Obtain datasets.

```bash
cd /path/to/scann/sra_scann_adapter/ann-benchmarks
mkdir data && cd data
wget http://ann-benchmarks.com/sift-128-euclidean.hdf5 --no-check-certificate
```

The directory structure of the main files is as follows:

```text
├── ann-benchmarks
      ├── data                                                      // Stores the datasets.
            └── sift-128-euclidean.hdf5
      ├── ann_benchmarks
            └── algorithms
                  └── scann
                        └── cpp_test
                              └── config-sift-128-euclidean.config  // Dataset configuration file
            └── test_cpp.sh                                         // Test script
├── scann
            ├── CMakeLists.txt                                      // Compilation configuration file
            ├── eval.cpp                                            // Test code
            ├── cmdline.h                                            // Header file of the cmdline parameter parsing library
project.sh                                                          // Compilation script
```

**Procedure<a name="section080205934220"></a>**

1. Verify that `libscann_cc.so` has been compiled successfully as described in [Installation Guide](./installation_guide.md).

2. Install CMake.

    ```bash
    yum install cmake
    ```

3. Install the dependencies.

    ```bash
    yum install numactl numactl-devel hdf5 hdf5-devel gtest-devel gcc-toolset-12-libstdc++-static
    ```

4. Install the Python dependencies.

    ```bash
    cd /path/to/scann/sra_scann_adapter/ann-benchmarks
    pip install -r requirements.txt
    pip install treelite==4.2.1 tl2cgen
    ```

5. Install protobuf.

    ```bash
    wget https://github.com/protocolbuffers/protobuf/archive/refs/tags/v3.21.9.tar.gz --no-check-certificate
    tar -xzf v3.21.9.tar.gz
    cd protobuf-3.21.9
    mkdir build && cd build
    cmake .. -Dprotobuf_BUILD_TESTS=OFF -DCMAKE_INSTALL_PREFIX=/usr/local/protobuf-3.21.9
    make install
    export PATH=/usr/local/protobuf-3.21.9/bin:$PATH
    export LD_LIBRARY_PATH=/usr/local/protobuf-3.21.9/lib:$LD_LIBRARY_PATH
    ```

6. Install Abseil.

    ```bash
    wget https://storage.googleapis.com/mirror.tensorflow.org/github.com/abseil/abseil-cpp/archive/fb3621f4f897824c0dbe0615fa94543df6192f30.tar.gz --no-check-certificate
    tar -xvzf fb3621f4f897824c0dbe0615fa94543df6192f30.tar.gz
    cd abseil-cpp-fb3621f4f897824c0dbe0615fa94543df6192f30
    mkdir build && cd build
    cmake .. && make -j
    make install
    ```

7. Install Eigen.

    ```bash
    git clone https://gitlab.com/libeigen/eigen.git
    cd eigen
    git checkout 33d0937c6bdf5ec999939fb17f2a553183d14a74
    mkdir build && cd build
    cmake .. -DCMAKE_INSTALL_PREFIX=/usr/local/eigen-3.3.7
    make -j && make install
    ```

8. Build the executable file.

    ```bash
    cd /path/to/scann/sra_scann_adapter
    sh project.sh --build_eval_cmake_sve
    ```

    >![note](public_sys-resources/icon-note.gif) **NOTE:**
    >`project.sh` contains the following compilation options. You can select them as required:
    >- --`prepare`: installs Python dependencies.
    >- --`build_eval_cmake_sve`: builds the executable file of the SVE instruction version using `libscann_cc.so` through `cmake`.
    >- --`build_eval_cmake_neon`: builds the executable file of the NEON instruction version using `libscann_cc.so` through `cmake`.
    >- --`build_eval_bazel_sve`: builds the executable file of the SVE instruction version using the source code through `bazel`.
    >- --`build_eval_bazel_neon`: builds the executable file of the NEON instruction version using the source code through `bazel`.

9. Run the test script.

    ```bash
    sh test_cpp.sh 
    ```

    >![note](public_sys-resources/icon-note.gif) **NOTE:**
    >During the test, dataset-related parameters (such as index construction and search policy) are controlled by the configuration file. The configuration file path is as follows:
    >`./algorithms/scann/cpp_test/config-*.config` ("\*" is a wildcard, covering all configuration files that start with `config-` and end with `.config`, such as `config-deep-image-96-angular.config`.)
    >You can adjust the `index_save_or_load` parameter in the configuration file to control index processing mode during the test. The details are as follows:
    >- `save`: builds the search index from scratch and saves it to a specified path, enabling direct loading in subsequent runs.
    >- `load`: skips the index-building step and reads the saved index file from the specified path for search. This option is applicable to the index reuse verification.
    >- Values other than `save` or `load`: build the search index from scratch but does not save it. The index is only effective for this process.

The test result is as follows:

<img src="figures/best_practices-c++.jpg" alt="best_practices-c++" width="1000"/>

## Integrating KScaNN into Milvus

The KScaNN algorithm can be integrated into the Milvus database (version 2.4.5) to accelerate the query efficiency while ensuring a high recall rate.

KScaNN optimizes the open-source ScaNN algorithm by using dynamic library inline, low-bit quantization, retrieval operators, and vector instructions, further improving the retrieval capability. The procedure is as follows:

1. Install Milvus.

    For details, see the [Milvus Installation Guide](https://www.hikunpeng.com/document/detail/en/kunpengdbs/ecosystemEnable/Milvus/kunpeng_milvusinstall_42_014.html).

2. Apply the patch file into Milvus for full compilation.

    For details, see the [Milvus KScaNN Optimization Feature Guide](https://www.hikunpeng.com/document/detail/en/boostdb/milvus/Milvuskscannop/docs/en/milvus_kscann_optimization_feature_guide.md).

3. Use ann-benchmarks for the test.

    For details, see [Milvus Database ANN-Benchmarks Test Guide](https://www.hikunpeng.com/document/detail/en/kunpengdbs/testguide/tstg/kunpeng_ann_marks_001.html).
