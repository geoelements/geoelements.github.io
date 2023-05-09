---
title: "Graph Neural Network-based surrogate model for granular flows"
authors: "Choi, Y.J, Kumar, K."
journal: 
layout: publication
categories: 
  - publications
tags:
  - journal
  - ml
  - gns
preprint: 
---

Accurate simulation of granular flow dynamics is crucial for assessing various geotechnical risks, including landslides and debris flows. Granular flows involve a dynamic rearrangement of particles exhibiting complex transitions from solid-like to fluid-like responses. Traditional continuum and discrete numerical methods are limited by their computational cost in simulating large-scale systems. Statistical or machine learning-based models offer an alternative. Still, they are largely empirical, based on a limited set of parameters. Due to their permutation-dependent learning, traditional machine learning-based models require huge training data to generalize. To resolve these problems, we use a graph neural network, a state-of-the-art machine learning architecture that learns local interactions. Graphs represent the state of dynamically changing granular flows and the interaction laws, such as energy and momentum exchange between grains. We develop a graph neural network-based simulator (GNS) that takes the current state of granular flow and predicts the next state using Euler explicit integration by learning the local interaction laws. We train GNS on different granular trajectories. We then assess the performance of GNS by predicting granular column collapse. GNS accurately predicts flow dynamics for column collapses with different aspect ratios unseen during training. GNS is hundreds of times faster than high-fidelity numerical simulators. The model also generalizes to domains much larger than the training data, handling more than twice the number of particles than it was trained on.