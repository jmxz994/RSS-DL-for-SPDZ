# Fast_Secure_ESD

This project is a deep learning privacy-preserving research based on the MP-SPDZ framework implementation, which currently contains two components: privacy classification for difficult cases and privacy inference for fast SwinTransformer.

# Instructions for use 
First, download the source code of this project or clone it to a Linux system, and be careful not to use the administrator identity to clone it.

Then check if the following dependencies are installed, if any are missing please install them first.
`sudo apt-get install automake build-essential clang cmake git libboost-dev libboost-filesystem-dev libboost-iostreams-dev libboost-thread-dev libgmp-dev libntl-dev libsodium-dev libssl-dev libtool python3`

The next step is to run the following command in the source root directory to complete the initialization of the SPDZ library.
`make all`
`Scripts/tldr.sh`

If none of the above steps make the code work, see [MP-SPDZ](https://github.com/data61/MP-SPDZ).
