---
title: "Spatial Navigation"
date: 2026-09-15
summary: "Mapping the cortical network that lets humans find their way through a dynamic world, and asking how it varies across people and across the lifespan"
weight: 1
---

Spatial navigation is among the most fundamental of everyday behaviors, and one of the most demanding. To move through the world we must know where we are, decide where we are going, and continuously work out how to get there while the world changes around us. My research program aims to explain how the human brain accomplishes this.

## Driving in the scanner

Most of what is known about the neural basis of human navigation comes from experiments in which participants view static images or passively watch movement through simple environments. Real navigation is neither static nor passive. To study it as it actually occurs, I developed an experiment in which participants drive through a large virtual city with dynamic traffic while their brain activity is recorded with functional MRI. I built every component of this experiment: the virtual city in Unreal Engine, MRI-compatible driving peripherals, and the analysis pipeline that extracts tens of thousands of navigation-related features from the game engine as participants play.

## A map of the cortical navigation network

Using these data, I fit high-dimensional voxelwise encoding models spanning 38 feature spaces and more than 28,000 features. This approach identified eleven functionally distinct cortical regions that support active navigation: five in prefrontal cortex, three in parietal cortex, and three previously known visual regions. Each region represents a distinct combination of navigation-related information, and the regions are organized along broadly distributed functional gradients across the cortical surface. This work provides the first quantitative map of the cortical network that mediates naturalistic navigation ([Zhang, Meschke & Gallant, 2025](/publications/cortical-network-naturalistic-navigation/), accepted at *Nature Neuroscience*).

Because these regions are tuned for complex, high-dimensional combinations of features, their functional properties are hard to describe in words. Together with Cheol Jun Cho, I used a variational autoencoder to reconstruct the dynamic visual experience predicted to maximally drive each region. These preferred visual experiences show that the navigation network is more engaged by dynamic scenes than by static ones, and they generate concrete, data-driven hypotheses for future experiments ([Zhang\*, Cho\* & Gallant, 2026](/publications/preferred-visual-experiences-navigation/)).

## Where this work is going

The map establishes the anatomy of the system. The next phase of my research program asks how this network produces behavior, and how it differs across people.

- **Navigation among other agents.** Real-world navigation is a multiagent problem: other people, vehicles, and animals share the space, and their actions must be anticipated. I am characterizing how the navigation network represents other agents and their likely future behavior, and how those representations feed into our own actions.
- **Responding to a changing world.** Routes get blocked, goals change, and plans must be revised mid-course. In collaboration with Won Mok Shim's group at Sungkyunkwan University, I have ported my experimental paradigm to a sheepherding task to study how the brain forms hierarchical plans and adapts them as circumstances change.
- **Individual differences and aging.** People differ enormously in navigational ability, and this ability declines with age. I am relating functional differences in the cortical navigation network to individual differences in navigation behavior, and characterizing how the network changes across the lifespan.
