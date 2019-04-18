# Deep Learning Practicuum

<!-- vim-markdown-toc GFM -->

- [CPU vs GPU](#cpu-vs-gpu)
   - [CPU](#cpu)
   - [GPU](#gpu)
- [GPU Acceleration](#gpu-acceleration)
- [Biowulf](#biowulf)

<!-- vim-markdown-toc -->

## CPU vs GPU

### CPU

- Latency limited
- We don't care how much data, but the response needs to be stable and fast
- Runs things like OS, keyboard interrupts, etc.

### GPU

- Throughput limited
- We don't care about time, but we need to cram as much through it as possible
- Highly parallel

## GPU Acceleration

1. Identify code that is compute intensive and parallel
   - Sequential is run on CPU
1. Rewrite to GPU
1. Enjoy speed boost
1. Repeat

## Biowulf

- See tutorials online
