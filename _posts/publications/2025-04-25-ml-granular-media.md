---
title: "Towards scientific machine learning for granular material simulations -- challenges and opportunities"
authors: "Fransen, M., Fürst, A., Tunuguntla, D., Wilke, D.N., Alkin, B., Barreto, D., Brandstetter, J., Cabrera, M.A., Fan, X., Guo, M., Kieskamp, B., Kumar, K., Morrissey, J., Nuttall, J., Ooi, J., Orozco, L., Papanicolopulos, S.-A., Qu, T., Schott, D., Shuku, T., Sun, W.C., Weinhart, T., Ye, D., Cheng, H."
journal: 
layout: publication
categories: 
  - publications
tags:
  - journal
  - ml
  
preprint: https://arxiv.org/abs/2504.08766
doi: 
---

Micro-scale mechanisms, such as inter-particle and particle-fluid interactions, govern the behaviour of granular systems. While particle-scale simulations provide detailed insights into these interactions, their computational cost is often prohibitive. Attended by researchers from both the granular materials (GM) and machine learning (ML) communities, a recent Lorentz Center Workshop on "Machine Learning for Discrete Granular Media" brought the ML community up to date with GM challenges.
This position paper emerged from the workshop discussions. We define granular materials and identify seven key challenges that characterise their distinctive behaviour across various scales and regimes, ranging from gas-like to fluid-like and solid-like. Addressing these challenges is essential for developing robust and efficient digital twins for granular systems in various industrial applications. To showcase the potential of ML to the GM community, we present classical and emerging machine/deep learning techniques that have been, or could be, applied to granular materials. We reviewed sequence-based learning models for path-dependent constitutive behaviour, followed by encoder-decoder type models for representing high-dimensional data. We then explore graph neural networks and recent advances in neural operator learning. Lastly, we discuss model-order reduction and probabilistic learning techniques for high-dimensional parameterised systems, which are crucial for quantifying uncertainties arising from physics-based and data-driven models.
We present a workflow aimed at unifying data structures and modelling pipelines and guiding readers through the selection, training, and deployment of ML surrogates for granular material simulations. Finally, we illustrate the workflow's practical use with two representative examples, focusing on granular materials in solid-like and fluid-like regimes.

## Cite

> Fransen, M., Fürst, A., Tunuguntla, D., Wilke, D. N., Alkin, B., Barreto, D., ... & Cheng, H. (2025). Towards scientific machine learning for granular material simulations--challenges and opportunities. arXiv preprint arXiv:2504.08766.

### BibLaTeX

```BibLaTeX
@misc{fransen2025towards,
  title         = {Towards Scientific Machine Learning for Granular Material Simulations---Challenges and Opportunities},
  author        = {Fransen, Marc and F{\"u}rst, Andreas and Tunuguntla, Deepak and Wilke, Daniel~N. and Alkin, Benedikt and Barreto, Daniel and Brandstetter, Johannes and Cabrera, Miguel~Angel and Fan, Xinyan and Guo, Mengwu and Kieskamp, Bram and Kumar, Krishna and Morrissey, John and Nuttall, Jonathan and Ooi, Jin and Orozco, Luisa and Papanicolopulos, Stefanos\hyp Aldo and Qu, Tongming and Schott, Dingena and Shuku, Takayuki and Sun, WaiChing and Weinhart, Thomas and Ye, Dongwei and Cheng, Hongyang},
  year          = {2025},
  eprint        = {2504.08766},
  archivePrefix = {arXiv},
  primaryClass  = {physics.comp-ph},
  note          = {arXiv:2504.08766}
}
```