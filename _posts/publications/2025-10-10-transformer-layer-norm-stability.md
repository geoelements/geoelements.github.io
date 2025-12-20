---
title: "Stability of Transformers under Layer Normalization"
authors:
  - "Kan, K."
  - "Li, X."
  - "Zhang, B. J."
  - "Sahai, T."
  - "Osher, S."
  - "Kumar, K."
  - "Katsoulakis, M. A."
journal: "arXiv preprint arXiv:2510.09904"
categories:
  - publications
layout: publication
tags:
  - journal
  - ml
  - transformers
  - deep-learning
preprint: https://arxiv.org/abs/2510.09904
doi:
---

Despite their widespread use, training deep Transformers can be unstable. Layer normalization, a standard component, improves training stability, but its placement has often been ad-hoc. In this paper, we conduct a principled study on the forward (hidden states) and backward (gradient) stability of Transformers under different layer normalization placements. Our theory provides key insights into the training dynamics: whether training drives Transformers toward regular solutions or pathological behaviors. For forward stability, we derive explicit bounds on the growth of hidden states in trained Transformers. For backward stability, we analyze how layer normalization affects the backpropagation of gradients, thereby explaining the training dynamics of each layer normalization placement. Our analysis also guides the scaling of residual steps in Transformer blocks, where appropriate choices can further improve stability and performance. Our numerical results corroborate our theoretical findings. Beyond these results, our framework provides a principled way to sanity-check the stability of Transformers under new architectural modifications, offering guidance for future designs.
