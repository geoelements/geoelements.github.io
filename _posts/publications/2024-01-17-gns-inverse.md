---
title: "Inverse analysis of granular flows using differentiable graph neural network simulator"
authors: "Choi, Y.J, Kumar, K."
journal: 
layout: publication
categories: 
  - publications
tags:
  - journal
  - ml
  - gns
preprint: https://arxiv.org/abs/2401.13695
dataset: https://doi.org/10.17603/ds2-0wjq-0j84
doi: https://doi.org/10.1016/j.compgeo.2024.106374 
---

Inverse problems in granular flows, such as landslides and debris flows, involve estimating material parameters or boundary conditions based on target runout profile. Traditional high-fidelity simulators for these inverse problems are computationally demanding, restricting the number of simulations possible. Additionally, their non-differentiable nature makes gradient-based optimization methods, known for their efficiency in high-dimensional problems, inapplicable. While machine learning-based surrogate models offer computational efficiency and differentiability, they often struggle to generalize beyond their training data due to their reliance on low-dimensional input-output mappings that fail to capture the complete physics of granular flows. We propose a novel differentiable graph neural network simulator (GNS) by combining reverse mode automatic differentiation of graph neural networks with gradient-based optimization for solving inverse problems. GNS learns the dynamics of granular flow by representing the system as a graph and predicts the evolution of the graph at the next time step, given the current state. The differentiable GNS shows optimization capabilities beyond the training data. We demonstrate the effectiveness of our method for inverse estimation across single and multi-parameter optimization problems, including evaluating material properties and boundary conditions for a target runout distance and designing baffle locations to limit a landslide runout. Our proposed differentiable GNS framework offers an orders of magnitude faster solution to these inverse problems than the conventional finite difference approach to gradient-based optimization.

## Cite

> Choi, Y., & Kumar, K. (2024). Inverse analysis of granular flows using differentiable graph neural network simulator. Computers and Geotechnics, 171, 106374.

### BibLaTeX

```BibLaTeX
@article{choi2024inverse,
  title={Inverse analysis of granular flows using differentiable graph neural network simulator},
  author={Choi, Yongjin and Kumar, Krishna},
  journal={Computers and Geotechnics},
  volume={171},
  pages={106374},
  year={2024},
  publisher={Elsevier}
}
```
