---
title: Fast-Pairwise
date: 2024-07-15
links:
  - type: code
    url: https://github.com/gallantlab/Fast-Pairwise
---

Fast Pairwise is a parallelized pairwise distance calculator built as a drop-in replacement for the single-threaded `scipy.spatial.distance.pdist`. It is written in C++ with Python bindings, uses multi-threading and AVX-512 vector instructions to compute distances on large two-dimensional NumPy arrays, and supports Euclidean, correlation, and random forest distances.

The need for it arose from my modeling work in the [/publications/cortical-network-naturalistic-navigation](spatial navigation experiment), in which we bootstrap the [https://www.biorxiv.org/content/10.1101/2023.07.17.549356v1.abstract](model connectivity) process, incurrings hundreds of pairwise comparisons across tens of thousands of vertices. At that scale the pairwise distance matrix becones an additional computational bottleneck on top of the high-dimensional model fitting process. Fast Pairwise streamlines one operation in the analysis process.
