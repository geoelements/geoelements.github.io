---
title: "Zero-Shot Function Encoder-Based Differentiable Predictive Control"
authors:
  - "Iqbal, H."
  - "Li, X."
  - "Ingebrand, T."
  - "Thorpe, A."
  - "Kumar, K."
  - "Topcu, U."
  - "Drgoňa, J."
journal: "arXiv preprint arXiv:2511.05757"
categories:
  - publications
layout: publication
tags:
  - journal
  - ml
  - control
  - neural-ode
preprint: https://arxiv.org/abs/2511.05757
doi:
---

We introduce a differentiable framework for zero-shot adaptive control over parametric families of nonlinear dynamical systems. Our approach integrates a function encoder-based neural ODE (FE-NODE) for modeling system dynamics with a differentiable predictive control (DPC) for offline self-supervised learning of explicit control policies. The FE-NODE captures nonlinear behaviors in state transitions and enables zero-shot adaptation to new systems without retraining, while the DPC efficiently learns control policies across system parameterizations, thus eliminating costly online optimization common in classical model predictive control. We demonstrate the efficiency, accuracy, and online adaptability of the proposed method across a range of nonlinear systems with varying parametric scenarios, highlighting its potential as a general-purpose tool for fast zero-shot adaptive control.
