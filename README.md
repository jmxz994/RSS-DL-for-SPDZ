# RSS-DL-for-SPDZ

This project is a deep learning privacy-preserving research based on the MP-SPDZ framework implementation, which currently contains two components: privacy classification for difficult cases and privacy inference for fast SwinTransformer.
 
 # Instructions for use 
 First, download the source code of this project or clone it to a Linux system, and be careful not to use the administrator identity to clone it.
 
 Then check if the following dependencies are installed, if any are missing please install them first.
 `sudo apt-get install automake build-essential clang cmake git libboost-dev libboost-filesystem-dev libboost-iostreams-dev libboost-thread-dev libgmp-dev libntl-dev libsodium-dev libssl-dev libtool python3`
 
 The next step is to run the following command in the source root directory to complete the initialization of the SPDZ library.
 `make all`
 `Scripts/tldr.sh`

If none of the above steps make the code work, see [MP-SPDZ](https://github.com/data61/MP-SPDZ).
 
 #Troubleshooting classification model
 We use different activation function optimization algorithms for different types of datasets and difficult problems. We use different activation function optimization algorithms for different types of datasets and difficult problems. Optimization approaches in generic computational frameworks are primarily categorized into two distinct methodological approaches. The first strategy employs activation function approximation techniques, utilizing polynomial interpolation or piecewise linearization to achieve computational simplification while maintaining functional equivalence, thereby substantially reducing arithmetic complexity and inter-process communication costs. The second paradigm focuses on systemic enhancement through computational graph optimizations, including but not limited to operator fusion for memory locality improvement, parallelization of tensor operations through SIMD vectorization, and adaptive memory management strategies. These orthogonal optimization dimensions - algorithmic simplification and system-level computational refinement - collectively address different aspects of performance bottlenecks in modern computing architectures.
 # Troubleshooting classification model
 We use different activation function optimization algorithms for different types of datasets and difficult problems.There are two main optimization methods used for generic frameworks. One is by approximating the activation function to reduce the computation and communication overhead, and the other is an indirect optimization by updating the efficiency of the underlying base operations.
 Our work is currently focused on the former, with the latter to be updated in the future.
 
 To briefly illustrate how the code runs in this project, I use the [Eryhemato-Squamous Disease](https://archive.ics.uci.edu/dataset/33/dermatology) dataset as an example.


