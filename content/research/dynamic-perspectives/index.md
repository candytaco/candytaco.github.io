---
title: "Dynamic Perspectives"
date: 2026-09-15
summary: "Dynamical systems approaches to the brain activity that produces continuous, naturalistic behavior"
weight: 3
---

Real-world behavior unfolds continuously in time, yet most neuroimaging analyses are static. They describe the average response to a stimulus or condition and marginalize time away. Electrophysiology in animals has shown that the dynamics of neural populations occupy low-dimensional subspaces that track task variables as they evolve. I am interested in bringing this dynamical systems perspective to human neuroimaging, and in developing methods that capture how brain activity moves through time to produce behavior.

## Task-related state spaces in fMRI

I developed a voxel-based state space modeling method that recovers low-dimensional, task-related state spaces from human fMRI data, and applied it to a visual attention task and a video game task. Each task induces distinct brain states that embed within a low-dimensional subspace capturing the task parameters, and attention increases the separation between states within that subspace ([Zhang, Gao, Çukur & Gallant, 2021](/publications/voxel-based-state-space-modeling/)). This work established that the state space framework, developed largely for population recordings in animals, applies to whole-brain human data recorded during complex natural tasks. The data are [publicly available](https://doi.org/10.6080/K0668BDF) on CRCNS.

## Empirical dynamic modeling of brain and behavior

I am now extending this line of work with more powerful nonlinear methods in an ongoing collaboration with Gerald Pao at the Okinawa Institute of Science and Technology, where I am a Visiting Researcher, and Terry Sejnowski at the Salk Institute, supported by the W. M. Keck Foundation. Empirical dynamic modeling reconstructs the attractor of a dynamical system directly from time series, without assuming a parametric form. Applied to my navigation data, these methods let us decode behavior from the geometry of brain dynamics and build end-to-end models that map neural activity to the actions a participant takes. To make these methods practical at the scale of whole-brain fMRI, I wrote [torchEDM](/software/torchedm/), a GPU-accelerated implementation of the core empirical dynamic modeling algorithms.

The long-term goal is a description of naturalistic behavior in which the brain is treated as what it is: a dynamical system whose trajectory, not just its state, is the object of study.
