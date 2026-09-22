---
title: "Naturalistic Neuroimaging Methods"
date: 2026-09-15
summary: "Building the experimental platform and modeling tools for closed-loop neuroimaging experiments that engage the full perception-cognition-action loop"
weight: 2
---

Real-world experience emerges from a continuous perception-cognition-action loop. The brain is a nonlinear system, and the activity that implements this loop cannot be fully engaged by classical neuroimaging paradigms in which participants passively view static, controlled stimuli. I have shown this directly. Visual-semantic tuning across the cortex differs substantially between an active navigation task and passive movie watching, with tuning shifting toward task-relevant categories such as vehicles and traffic signs during navigation ([Zhang & Gallant, 2026](/publications/visual-semantic-tuning-shifts-between-tasks/)). Object representations measured during closed-loop behavior are not the same as those measured in static experiments. Studying any behavior that engages the full loop therefore requires tasks that resemble the situations in which the behavior actually occurs.

## An interactive experimental platform

To make such experiments possible, I built a naturalistic neuroimaging platform around modern game engines. Rather than presenting predetermined stimuli, the platform immerses participants in dynamic virtual worlds that respond to their actions. The game engine that renders the world also records it, so the platform simultaneously captures tens of thousands of covariates spanning perception, cognition, and action. I built every component: the experimental paradigm, custom MRI-compatible peripherals, the virtual-world software, and the analysis pipeline. The same platform has since been ported to new games and new questions, from hierarchical planning in a sheepherding task to collaborative problem solving in Portal 2.

The core infrastructure is released as [It's Complicated](/software/its-complicated/), a library and guide for architecting interactive fMRI experiments in Unreal Engine. [SharpEyes](/software/sharpeyes/) provides the companion eyetracking tools needed to build gaze-centered features from stimulus video.

## High-dimensional modeling and interpretation

Interactive experiments produce data that classical analyses were not designed for: thousands of continuously varying, correlated features and no repeated trials. My approach is to fit high-dimensional voxelwise encoding models that jointly account for many feature spaces, and then to develop methods that make the fitted models interpretable. I have demonstrated that such models are tractable at the scale of tens of thousands of features, and I have introduced methods for characterizing what a region encodes, including generative reconstructions of a region's preferred visual experience. Current work develops encoding-model-based high-throughput hypothesis testing, which uses a single rich dataset to evaluate many hypotheses about cortical function without collecting new data for each one.

This platform is the backbone of my research program. It is designed to be general, and the tools are public so that others can bring naturalistic interactivity into their own scanners.
