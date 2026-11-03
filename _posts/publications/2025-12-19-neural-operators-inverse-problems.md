---
title: "Learning Generalizable Neural Operators for Inverse Problems"
authors:
  - "Thorpe, A. J."
  - "Tretiakov, S."
  - "Sarkar, D. R."
  - "Kumar, K."
  - "Topcu, U."
journal: "arXiv preprint arXiv:2512.18120"
categories:
  - publications
layout: publication
tags:
  - journal
  - ml
  - operator-learning
  - inverse-problems
preprint: https://arxiv.org/abs/2512.18120
doi: 
---

Inverse problems challenge existing neural operator architectures because ill-posed inverse maps violate continuity, uniqueness, and stability assumptions. We introduce B2B<sup>-1</sup>, an inverse basis-to-basis neural operator framework that addresses this limitation. Our key innovation is to decouple function representation from the inverse map. We learn neural basis functions for the input and output spaces, then train inverse models that operate on the resulting coefficient space. This structure allows us to learn deterministic, invertible, and probabilistic models within a single framework, and to choose models based on the degree of ill-posedness. We evaluate our approach on six inverse PDE benchmarks, including two novel datasets, and compare against existing invertible neural operator baselines. We learn probabilistic models that capture uncertainty and input variability, and remain robust to measurement noise due to implicit denoising in the coefficient calculation. Our results show consistent re-simulation performance across varying levels of ill-posedness. By separating representation from inversion, our framework enables scalable surrogate models for inverse problems that generalize across instances, domains, and degrees of ill-posedness.
