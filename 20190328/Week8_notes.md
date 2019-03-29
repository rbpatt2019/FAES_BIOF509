# Week 8 Notes
<!-- vim-markdown-toc GFM -->

- [K-means](#k-means)
- [Mixture models](#mixture-models)
   - [Types](#types)
   - [Strengths and weaknesses](#strengths-and-weaknesses)
   - [Expectation Maximisation (EM) Algoritm](#expectation-maximisation-em-algoritm)
      - [Steps:](#steps)
      - [Picking _k_](#picking-_k)
- [Dimensionality Reduction](#dimensionality-reduction)
   - [Factor Analysis](#factor-analysis)

<!-- vim-markdown-toc -->

## K-means

- Works best whe variance is the same in all directions - _ie_ data is sperical
- Frequently you can visually deduce it, but there are quantitative options
- If data aren't sperical, it will be sub-optimal - the real world case!

## Mixture models

Provide probablistic interpretation of clustering

### Types
  
1. Hard clustering: do **not** overlap
1. Soft clustering: can overlap

### Strengths and weaknesses

- Advantages:
   1. probablistic
   1. Soft clustering
- Disadvantages:
   1. Sensitive to starting points (requires multiple random initialisations)
   1. Can converge to local maximum
   1. Works best when number of observations, _n_, is significantly greater than the dimensionalit, _m_

### Expectation Maximisation (EM) Algoritm

- Assigning points to _k_ Gaussians with **equal** mean and variance
- Can be uni- or multi-variate

#### Steps:

1. Start with _k=2_ Gaussians
1. Repeat until convergence:
   1. E-Step: Estimate probabilities
   1. M-Step: Update mean and covariance

#### Picking _k_

- Occam's razor: simplest model that fits
- Normally using either:
   1. Bayes information cluster (BIC)
   2. Akaike information cluser (AIC)
- Both score on fit and penalise on complexity

## Dimensionality Reduction

### Factor Analysis

- Assumes variations in observed variables reflect variations in fewer latent variables
- Latent variables (facors) need not be weighted equally
- Number of factors is a hyper-parameter we provide
- Factors can be subjectively renamed

