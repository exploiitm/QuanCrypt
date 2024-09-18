# QuanCrypt

# The wait is over, guys. We will jump into actual samples. There are two choices.
# Actual NIST-Implemented Library (kyber512)
## The child repo contains 12 C source and 12 associated C header files (+2 independent C header files).
## The problem with this repo is that this is predominantly C, but for SYCL, we need C++
## We may need to modify this code to C++, before proceeding.

## We need to focus on very specific files first to get an initial boost in speed.
## For this, getting a overall picture of how each file's output is dependent on the other, is also important. 
## Therefore, Each one of us, need to take 2 files (source files), and analyse what files are dependent on it, what files it depends onn ,etc
## With this, we need to create a generic task graph, based on which we can focus.

# C++ Library (ml-kem)
## Has 12 C++ header files. NOT actual NIST implementation. But, there is no headstart of converting from C to C++.
## Documentation is clear. 
## Still, we need to split among us and analyse these headers for task graph and profiling. 

# Attaching these two codebases here, for completeness. Based on simplicity, we can start on the codebase, preferred by all.
