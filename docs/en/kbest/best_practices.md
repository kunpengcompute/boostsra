# Best Practices

## Performance Test

This document provides details on how to call the KBest algorithm API in C++. In the example, the <code>sift-128-euclidean.hdf5</code> dataset is used and the program runs with 32 threads. Before calling the APIs, ensure that KBest has been installed.

**Obtaining the Dataset and Test Program <a name="section5124167418"></a>**

1. Obtain the [test program](https://atomgit.com/openeuler/sra_test.git). The branch is <code>v2.0.0</code>. Assume that the program runs at the <code>/path/to/sra\_test</code> directory. The full directory structure is as follows:

    ```text
    ├── configs                                                   // Stores configuration files for the algorithm and dataset.
          └── kbest
                └── kbest_sift-128-euclidean.config 
    ├── include                                                   // Stores header files of the test framework.
          └── algo                                                // Algorithm index definitions
          └── core                                                // Header files for data processing and test result processing
          └── framework                                           // Header files related to the test framework
    ├── src                                                       // Stores source files of the test framework.
          └── algo                                                // Algorithm adaptation layers
          └── bench                                               // Centralized test file
          └── core                                                // Files for data processing and test result processing
          └── registry                                            // Algorithm factory registry
    ├── Makefile                                                  // Script for compiling the program.
    └── test.sh                                                 // Script for running the test.
    ├── test_muti-numas.sh                                        // Script for running the parallel test
    ├── data                                                      // Directory for storing datasets (You need to manually create and store datasets.)
          └── sift-128-euclidean.hdf5
    ├── indexes
          └── kbest                                               // Stores the built index.
                └── sift.kbest                                    // Built index, which is generated when the executable file kbest_test runs and the save_or_load parameter in the dataset configuration file is set to save.
    └── kbest_test                                                // Executable file generated after compilation.
    ```

2. <a name="li1673311431218"></a>Obtain the dataset and save it to <code>/path/to/sra\_test/data</code>.

    ```bash
    cd /path/to/sra_test
    mkdir -p data
    cd data
    wget http://ann-benchmarks.com/sift-128-euclidean.hdf5 --no-check-certificate
    ```

**Test Example <a name="section5255174043217"></a>**

1. Install dependencies.

    ```bash
    yum install hdf5 hdf5-devel numactl numactl-devel
    ```

2. Compile and install KBest as described in [Installation Guide](./installation_guide.md).
3. Build the executable file. Enter the KBest installation path and the paths to other required dependencies as prompted.

    ```bash
    make kbest_test
    ```

4. If this is the first time you run the command, ensure that the value of <code>save\_or\_load</code> in the <code>kbest\_sift-128-euclidean.config</code> file is <code>save</code>. You can change the value to <code>load</code> in subsequent runs to load the constructed graph index for query.
5. Run the executable file.

    ```bash
    numactl -C 0-31 -m 0 ./kbest_test kbest sift-128-euclidean
    ```

The test result is as follows:

<img src="figures/best_practices-c++.jpg" alt="best_practices-c++" width="800"/>

## Integrating KBest into Milvus

The KBest algorithm can be integrated into the Milvus database (version 2.4.5) to accelerate the query efficiency while ensuring a high recall rate. This practice integrates KBest into the open-source Milvus database as a patch file to provide graph search functionality.

Among all index algorithms supported by Milvus, the graph-based index algorithm is Hierarchical Navigable Small World (HNSW), which can perform quick query and achieve a high recall rate, but consumes a large amount of memory resources. To extend the graph-based index algorithm and accelerate the query while ensuring a high recall rate, the KBest algorithm optimizes the performance and precision of the nearest neighbor search by using methods such as quantization and vector instruction, providing the search capability equivalent to the open-source Faiss HNSW algorithm. The procedure is as follows:

1. Install Milvus.

    For details, see the [Milvus Installation Guide](https://www.hikunpeng.com/document/detail/en/kunpengdbs/ecosystemEnable/Milvus/kunpeng_milv_ins_42_001.html).

2. Apply the patch file into Milvus for full compilation.

    For details, see the [Milvus KBest Optimization Feature Guide](https://www.hikunpeng.com/document/detail/en/kunpengdbs/appAccelFeatures/milvuskbestop/kunpeng_kbest_43_002.html).

3. Use ann-benchmarks for the test.

    For details, see [Milvus ann-benchmarks Test Guide](https://www.hikunpeng.com/document/detail/en/kunpengdbs/testguide/tstg/kunpeng_ann_marks_001.html).
