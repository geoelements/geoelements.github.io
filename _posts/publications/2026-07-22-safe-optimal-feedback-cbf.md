---
title: "End-to-End Learning of Safe Optimal Feedback Control in High Dimensions with Control Barrier Function Layers"
authors:
  - "Li, X."
  - "Kan, K."
  - "Verma, D."
  - "Kumar, K."
  - "Osher, S."
  - "Wu Fung, S."
journal: "arXiv preprint arXiv:2607.20674"
categories:
  - publications
layout: publication
tags:
  - journal
  - ml
  - control
  - safety
preprint: https://arxiv.org/abs/2607.20674
doi: 
---

We consider the problem of learning high-dimensional semi-global feedback controllers under hard safety constraints enforced by control barrier functions (CBFs). Incorporating CBFs into end-to-end policy training requires embedding a quadratic-program-based safety filter as an optimization layer, but computational and differentiation bottlenecks have largely restricted prior approaches to low-dimensional systems, typically with at most 16 state dimensions. We address this limitation by combining operator splitting with the recently developed Jacobian-Free Backpropagation (JFB) method to enable scalable end-to-end training while preserving hard safety guarantees through the CBF safety filter. We justify this training methodology theoretically using nonsmooth analysis techniques and demonstrate its effectiveness on high-dimensional multi-agent nonlinear control problems with state and control dimensions up to 1200 and 400, respectively.
