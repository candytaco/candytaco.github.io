---
title: Fast-Pairwise
date: 2024-07-15
links:
  - type: code
    url: https://github.com/gallantlab/Fast-Pairwise
---

Fast-Pairwise is a parallelized pairwise distance calculator built as a drop-in replacement for the single-threaded `scipy.spatial.distance.pdist`. It is written in C++ with Python bindings, uses AVX-512 instructions for multi-threaded computation on large 2D NumPy arrays, and supports euclidean, correlation, and random forest distances.

<!--more-->
