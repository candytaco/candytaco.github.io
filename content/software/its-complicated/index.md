---
title: "It's Complicated"
date: 2026-03-23
links:
  - type: code
    url: https://github.com/gallantlab/its-complicated
  - type: site
    url: https://gallantlab.org/Its-Complicated/

featured: true
---

It's Complicated is a software library and guide for architecting interactive fMRI experiments in Unreal Engine. It provides the replay infrastructure that a naturalistic, closed-loop experiment: we leverage the replication engine to record the entire state of the virtual world as the experiment runs, and play it back later offline to extract as many features as we want for analyzing the brain activity. Because the recordings allow us to _recreate_ the entire history of the environment, we are able to compute and extract features _post hoc_ that were not even thought of during data collection.

The library grew out of my [spatial navigation](/research/spatial-navigation/) experiment, in which participants drive through a large virtual city with dynamic traffic, and it forms the technical basis of my [naturalistic neuroimaging platform](/research/naturalistic-neuroimaging/). The same components have since been used to port the paradigm new scientific questions. Work is in progress on an in-depth tutorial that walks through building a complete experiment with these plugins.
