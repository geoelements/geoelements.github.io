---
title: "Neural Operators for Multi-Task Control and Adaptation"
authors:
  - "Sewell, D."
  - "Li, X."
  - "Tretiakov, S."
  - "Kumar, K."
  - "Fridovich-Keil, D."
journal: "arXiv preprint arXiv:2604.03449"
categories:
  - publications
layout: publication
tags:
  - journal
  - ml
  - control
  - operator-learning
preprint: https://arxiv.org/abs/2604.03449
doi: 
---

Neural operator methods have emerged as powerful tools for learning mappings between infinite-dimensional function spaces, yet their potential in optimal control remains largely unexplored. We focus on multi-task control problems, whose solution is a mapping from task description (e.g., cost or dynamics functions) to optimal control law (e.g., feedback policy). We approximate these solution operators using a permutation-invariant neural operator architecture. Across a range of parametric optimal control environments and a locomotion benchmark, a single operator trained via behavioral cloning accurately approximates the solution operator and generalizes to unseen tasks, out-of-distribution settings, and varying amounts of task observations. We further show that the branch-trunk structure of our neural operator architecture enables efficient and flexible adaptation to new tasks. We develop structured adaptation strategies ranging from lightweight updates to full-network fine-tuning, achieving strong performance across different data and compute settings. Finally, we introduce meta-trained operator variants that optimize the initialization for few-shot adaptation. These methods enable rapid task adaptation with limited data and consistently outperform a popular meta-learning baseline. Together, our results demonstrate that neural operators provide a unified and efficient framework for multi-task control and adaptation.
