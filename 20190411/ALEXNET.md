# ALEXNET

Guest lecture,

<!-- vim-markdown-toc GFM -->

- [Early Problems](#early-problems)
- [Solutions](#solutions)
- [Architecture](#architecture)

<!-- vim-markdown-toc -->

## Early Problems

1. Datasets were small and general
1. Computational capacity/complexity made models hard to train
1. Hardware was limiting

Jeffrey Hinton's group solved in 2012

## Solutions

1. ImageNet = 15 million images, 22000 categories
1. Convolutional layers are faster but not much worse
1. An interface language was developed with high-powered GPUs

## Architecture

1. They used ReLU
   - Previously used Sigmoid, TanH
   - ReLU was simpler, faster
   - Is non-saturating, non-linear
1. Multi-GPU training
   - They used model parallelism - This is still challenging!
   - Creates a columnar process
   - Allows for larger models
   - In modern era, frequently data parallel
1. Local response normalisation
   - Not much used any more
   - Biologically inspired by lateral inhibition
   - Helps supress noise around larger signals
1. Overlapping pooling

