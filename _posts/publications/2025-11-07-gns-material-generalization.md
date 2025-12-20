---
title: "Parameter-Efficient Conditioning for Material Generalization in Graph-Based Simulators"
authors:
  - "Manoharan, N. R."
  - "Iqbal, H."
  - "Kumar, K."
journal: "arXiv preprint arXiv:2511.05456"
categories:
  - publications
layout: publication
tags:
  - journal
  - ml
  - gns
  - graph-neural-networks
preprint: https://arxiv.org/abs/2511.05456
doi:
---

Graph network-based simulators (GNS) have demonstrated strong potential for learning particle-based physics (such as fluids, deformable solids, and granular flows) while generalizing to unseen geometries due to their inherent inductive biases. However, these models typically work with single materials and struggle with different constitutive behaviors. We propose a parameter-efficient conditioning mechanism using Feature-wise Linear Modulation (FiLM) targeting early message-passing layers, where material sensitivity is concentrated. Our approach achieves comparable performance by fine-tuning only 1-5 of 10 layers using merely 12 short simulation trajectories from new materials—a five-fold data reduction versus baseline methods. The mechanism successfully handles interpolated and moderately extrapolated material parameter values, and demonstrates utility for inverse problems by identifying unknown cohesion parameters, enabling applications in inverse design and closed-loop control tasks where material properties are treated as design variables.
