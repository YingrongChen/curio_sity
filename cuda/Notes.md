GPU is for solving puzzles that the order of operations does not matter. You can solve multiple pieces at the same time, as long as they don't interfere with each other.

- cpu/host/functions vs gpu/device/kernels

CPU (host)
- minimize time of one task
- metric: latency in seconds
GPU (device)
- maximize throughput
- metric: throughput in tasks per second (ex: pixels per ms)

## Typical CUDA program
1. CPU allocates CPU memory
2. CPU copies data to GPU
3. CPU launches kernel on GPU (processing is done here) - gpu parallel function
4. CPU copies results from GPU back to CPU to do something useful with it

## Some terms to remember
- kernels (not popcorn, not convolutional kernels, not linux kernels, but GPU kernels)
- threads, blocks, and grid (next chapter)
- GEMM = **GE**neral **M**atrix **M**ultiplication
- SGEMM = **S**ingle precision (fp32) **GE**neral **M**atrix **M**ultiplication
