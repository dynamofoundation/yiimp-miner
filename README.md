# yiimp-miner
Source code for yiimp compatible miner

To build on Visual Studio 2019 use included solution file.

To build on Ubuntu 18.04 or greater, use

g++-11 -I. -std=gnu++20 *.cpp core/*.cpp -lpthread -L/opt/cuda/lib64 -lOpenCL -o dyn_miner -DGPU_MINER

You will need pthreads and opencl/cuda libraries.  You will also need recent versions of g++ and stdlib, which can be obtained as follows:

sudo apt install g++-11
sudo apt install libstdc++-10-dev

