---
title: "Human-AI Interactions"
date: 2026-09-15
summary: "How humans and embodied AI agents understand one another in shared, interactive environments"
weight: 4
---

AI systems are increasingly deployed in the physical world as embodied agents. Autonomous vehicles already share the road with human drivers, and in that setting an AI agent is not a tool but a co-equal participant. Both humans and machines must continuously adjust their actions to account for the behavior of the other. This opens a new frontier for cognitive neuroscience. How do humans understand and predict other agents, and how should we build AI agents that humans find intuitive to interact with? The brain systems that mediate these interactions hold the key to both questions.

## Brain-AI alignment during driving

Driving is an ideal domain in which to study this problem, and my naturalistic navigation experiment provides the human brain data to do so. In an ongoing collaboration with Claire Tomlin's group in Electrical Engineering and Computer Sciences at UC Berkeley, supported by the Office of Naval Research, we treat the two directions of the problem symmetrically. AI algorithms provide testable hypotheses for how the brain implements dynamic control, and brain data provides a metric for how well an AI system's internal representations match those of the humans it must interact with.

We have compared the internal states of analytical, control-theoretic models of human driving and the activations of end-to-end driving neural networks against cortical activity recorded during active navigation. The results indicate that the human brain likely implements forward-predictive control to account for other agents on the road, and that end-to-end networks may transform perception into action using algorithms that differ from those of the brain ([Strong et al., 2024](https://proceedings.mlr.press/v242/strong24b/strong24b.pdf)). Together these studies establish a general framework for evaluating brain-AI alignment in interactive behavior.

## Toward interactive experiments with AI agents

The current framework compares an AI agent's representations against human brain data collected in the agent's absence. The next phase of this work puts the two in the same world. My experimental platform already populates its virtual city with autonomous traffic, and it is built to support experiments in which participants navigate alongside AI-controlled agents in the scanner. Such experiments will let us measure how the brain represents an artificial partner's intentions, how those representations differ from those for human partners, and which properties of an agent's behavior make it legible to the people around it. The answers will inform the design of AI systems that interact with humans the way humans expect.
