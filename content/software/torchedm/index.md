---
title: torchEDM
date: 2026-09-16
links:
  - type: code
    url: https://github.com/candytaco/torchEDM
---

torchEDM is a fork of pyEDM, Python implementation of Empirical Dynamic Modeling, that replaces the computational backend with PyTorch. Computations are vectorized and run on GPUs, and the library adds object-oriented fitters with scikit-learn-like semantics: a model is constructed, fit to a time series, and then used to predict, so that it composes with the rest of a standard Python analysis pipeline.

Empirical Dynamic Modeling reconstructs the attractor of a dynamical system directly from observed time series using delay embeddings and nearest-neighbor prediction, without assuming a parametric model. The nearest-neighbor searches at its core are cheap for a single time series but prohibitive when applied to tens of thousands of voxels or to the large embedding libraries needed for whole-brain analysis. torchEDM was written to make these methods practical at that scale. It supports my work on the [dynamics of brain activity](/research/dynamic-perspectives/) in collaboration with Gerald Pao and Terry Sejnowski.
