# Quick Start

## Enabling KRL in Faiss

Faiss integrates with KRL to enhance the performance of the HNSW, PQFS, IVFPQ, IVFPQFS, and IVFFLAT algorithms. Users obtain the open source Faiss 1.8.0 code, integrate a patch for enabling KRL, and compile the code to obtain the dynamic library files with KRL performance enhanced.

1. Download the open-source Faiss source code from the [GitHub repository](https://github.com/facebookresearch/faiss.git) using the `v1.8.0` tag. Save the file to a path accessible to a compiler, such as `/path/to/faiss-1.8.0`.

    ```bash
    git clone --branch v1.8.0 --single-branch https://github.com/facebookresearch/faiss.git
    ```

2. Install Make, CMake, and GCC 12. The GCC 12 installation procedure applies to openEuler 22.03 LTS SP3. openEuler 24.03 LTS SP3 comes with GCC 12 pre-installed, so you only need to install Make and CMake.

    ```bash
    yum install make cmake gcc-toolset-12-gcc gcc-toolset-12-gcc-c++ gcc-toolset-12-libstdc++-static gcc-toolset-12-gcc-gfortran
    export PATH=/opt/openEuler/gcc-toolset-12/root/usr/bin/:$PATH
    export LD_LIBRARY_PATH=/opt/openEuler/gcc-toolset-12/root/usr/lib64/:$LD_LIBRARY_PATH
    ```

3. <a name="li84129301112"></a>Faiss depends on the math library. Download the open-source OpenBLAS source code from the [GitHub repository](https://github.com/OpenMathLib/OpenBLAS.git) using the v0.3.29 tag. Save the file to a path accessible to the compiler, such as `/path/to/OpenBLAS-0.3.29`.

    ```bash
    git clone --branch v0.3.29 --single-branch https://github.com/OpenMathLib/OpenBLAS.git
    ```

4. Compile the source code to generate the `libopenblas.so` dynamic library file.

    ```bash
    cd /path/to/OpenBLAS-0.3.29/OpenBLAS
    make
    make install
    ```

    >![NOTE](public_sys-resources/icon-note.gif) **NOTE**
    >You can run the `make install PREFIX=/path/to/openblas/install` command to specify the installation path `/path/to/openblas/install`. The default installation path is `/opt/OpenBLAS`.

5. Extract the patch file `0001-faiss-1.8.0-add-krl.patch` required for enabling KRL from `BoostKit-boostsra-krl\_1.0.0.zip`. If you install Faiss by compiling the source code, the patch file is stored in the `/path/to/krl` directory. Install the patch file.

    ```bash
    cd /path/to/faiss-1.8.0/faiss
    patch -p1 < 0001-faiss-1.8.0-add-krl.patch
    ```

6. Compile the Faiss code to obtain `libfaiss.so`.

    ```bash
    export KRL_PATH=/usr/local/sra_krl
    cd /path/to/faiss-1.8.0
    cmake -B build . \
      -DFAISS_ENABLE_GPU=OFF \
      -DBUILD_TESTING=OFF \
      -DBUILD_SHARED_LIBS=ON \
      -DCMAKE_BUILD_TYPE=Release \
      -DFAISS_OPT_LEVEL=generic \
      -DFAISS_ENABLE_PYTHON=OFF \
      -DMKL_LIBRARIES=/opt/OpenBLAS/lib/libopenblas.so
    make -C build -j faiss
    make -C build install
    ```

    >![NOTE](public_sys-resources/icon-note.gif) **NOTE**
    >- Set `KRL_PATH` to `/usr/local/sra_krl`.
    >- You can add the compilation option `-DCMAKE_INSTALL_PREFIX=/path/to/faiss/install` during compilation for specifying the installation path `/path/to/faiss/install`. The default installation path is `/usr/local`.
    >- The compilation option `-DMKL_LIBRARIES` must be set to the installation path of OpenBLAS in step [3](#li84129301112).

## Example

This section uses the sift-128-euclidean.hdf5 dataset, Faiss-supported algorithm (IVFPQ), and 32 threads for illustration. Before use, install KRL by following the instructions in [Installation Guide](./installation_guide.md) and enable KRL for Faiss.

**Obtaining the Dataset and Test Program<a name="section5300679419"></a>**

1. Obtain the [test program](https://atomgit.com/openeuler/sra_test.git). The branch is `v2.0.0`. Assume that the program runs at the `/path/to/sra\_test` directory. The full directory structure is as follows:

    ```text
    ├── configs                                                   // Stores configuration files for the algorithm and dataset.
          └── ivfpq
                └── ivfpq_sift-128-euclidean.config 
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
          └── ivfpq                                               // Stores the built index, which needs to be manually created.
                └── sift.faiss                                    // Built index, which is generated when the executable file ivfpq_test runs and the save_or_load parameter in the dataset configuration file is set to save.
    └── ivfpq_test                                                // Executable file generated after compilation.
    ```

2. <a name="li1673311431218"></a>Obtain the dataset and save it to <code>/path/to/sra\_test/data</code>.

    ```bash
    cd /path/to/sra_test
    mkdir -p data
    cd data
    wget http://ann-benchmarks.com/sift-128-euclidean.hdf5 --no-check-certificate
    ```

**Performance Test<a name="section183012712414"></a>**

1. Install dependencies.

    ```bash
    yum install hdf5 hdf5-devel numactl numactl-devel
    ```

2. Build the executable file. Enter the Faiss installation path and the paths to other required dependencies as prompted. When "Enter extra compile defines" is displayed, enter `-I/path/to/krl/out/include/ -L/path/to/krl/out/lib/ -lkrl`, where `/path/to/krl/out` is the KRL installation path.

    ```bash
    make ivfpq_test
    ```

    >![NOTE](public_sys-resources/icon-note.gif) **NOTE**
    >During the test, select the appropriate compilation instruction for each algorithm.
    >- HNSW: `make hnsw\_test`
    >- PQFS: `make pqfs\_test`
    >- IVFPQ: `make ivfpq\_test`
    >- IVFPQFS: `make ivfpqfs\_test`
    >- IVFFLAT: `make ivfflat\_test`

3. For the first run, ensure that `save\_or\_load` in the `ivfpq\_sift-128-euclidean.config` file is set to `save`. In subsequent runs, you can change it to `load` to use the built graph index or retriever for querying.
4. Run the executable file. Add the OpenBLAS, Faiss, and KRL dynamic library paths to the environment variable.

    ```bash
    numactl -C 0-31 -m 0 ./ivfpq_test ivfpq sift-128-euclidean
    ```

The command output is as follows:

<img src="figures/quick_start-running-result.jpg" alt="quick_start-running-result" width="800"/>
