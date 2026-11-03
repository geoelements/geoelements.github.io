---
title: "A Critical Assessment of PINNs and Operator Learning for Geotechnical Engineering"
authors:
  - "Kumar, K."
journal: "arXiv preprint arXiv:2512.24365"
categories:
  - publications
layout: publication
tags:
  - journal
  - ml
  - sciml
  - operator-learning
preprint: https://arxiv.org/abs/2512.24365
doi: 
---

Scientific machine learning (SciML) offers neural-network alternatives to numerical workflows in geotechnical engineering. This paper benchmarks multi-layer perceptrons (MLPs), physics-informed neural networks (PINNs), deep operator networks (DeepONet), and graph network simulators (GNS) against finite-difference and particle-based references on geotechnical benchmarks, and compares PINN inversion with automatic differentiation (AD) through a conventional solver. We evaluate each method for extrapolation, training, and inference cost, transfer across problem instances, and physics accuracy. An MLP trained on two years of Terzaghi consolidation fits the data, but at year ten predicts ~290 mm with ReLU and ~60 mm with tanh or sigmoid, against a reference of 99.3 mm. A PINN on a damped oscillator with a time domain inside [0,1] matches the closed form within that interval but fails outside, since the residual constrains the fit only where it is sampled. For the 1D wave equation, PINN training is ~96,000 times slower than finite-difference methods and less accurate. DeepONet avoids PINN retraining, yet for the beam on elastic foundation, its training cost equals ~1.8 million finite-difference solves, and inference is slower per query than the direct solver. GNS improves geometric transfer through local particle interactions, though formulations still need trajectories, large training sets, and substantial memory. In the inverse wave benchmark, AD through the finite-difference solver recovers the material profile in seconds with ~1% error. The results support a cautious role for SciML. Neural networks suit interpolation and pattern recognition inside validated domains, while inverse analysis should first try differentiable physics-based solvers when a reliable forward solver exists.
