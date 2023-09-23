---
title: "Accelerating particulate and fluid simulations with graph neural networks for solving forward and inverse problems"
authors: "Kumar, K., Choi, Y.J."
journal: 
layout: publication
categories: 
  - publications
tags:
  - ml
  - gns
preprint: 
---

We leverage physics-embedded differentiable graph network simulators (GNS) to accelerate particulate and fluid simulations to solve forward and inverse problems. GNS represents the domain as a graph with particles as nodes and learned interactions as edges. Compared to modeling global dynamics, GNS enables learning local interaction laws through edge messages, improving its generalization to new environments. GNS achieves over 165x speedup for granular flow prediction compared to parallel CPU numerical simulations. We propose a novel hybrid GNS/Material Point Method (MPM) to accelerate forward simulations by minimizing error on a pure surrogate model by interleaving MPM in GNS rollouts to satisfy conservation laws  and minimize errors achieving 24x speedup compared to pure numerical simulations. The differentiable GNS enables solving inverse problems through automatic differentiation, identifying material parameters that result in target runout distances. We demonstrate the ability of GNS to solve inverse problems by iteratively updating the friction angle (a material property) by computing the gradient of a loss function based on the final and target runouts, thereby identifying the friction angle that best matches the observed runout. The physics-embedded and differentiable simulators open an exciting new paradigm for AI-accelerated design, control, and optimization.