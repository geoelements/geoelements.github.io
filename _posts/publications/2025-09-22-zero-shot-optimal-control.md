---
title: "Zero-Shot Transferable Solution Method for Parametric Optimal Control Problems"
authors:
  - "Li, X."
  - "Kan, K."
  - "Verma, D."
  - "Kumar, K."
  - "Osher, S."
  - "Drgoňa, J."
journal: "arXiv preprint arXiv:2509.18404"
categories:
  - publications
layout: publication
tags:
  - journal
  - ml
  - control
  - operator-learning
preprint: https://arxiv.org/abs/2509.18404
doi:
---

This paper presents a transferable solution method for optimal control problems with varying objectives using function encoder (FE) policies. Traditional optimization-based approaches must be re-solved whenever objectives change, resulting in prohibitive computational costs for applications requiring frequent evaluation and adaptation. The proposed method learns a reusable set of neural basis functions that spans the control policy space, enabling efficient zero-shot adaptation to new tasks through either projection from data or direct mapping from problem specifications. The key idea is an offline-online decomposition: basis functions are learned once during offline imitation learning, while online adaptation requires only lightweight coefficient estimation. Numerical experiments across diverse dynamics, dimensions, and cost structures show our method delivers near-optimal performance with minimal overhead when generalizing across tasks, enabling semi-global feedback policies suitable for real-time deployment.
