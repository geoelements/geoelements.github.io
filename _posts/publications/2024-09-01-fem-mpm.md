---
title: "Sequential Hybrid Finite Element and Material Point Method to Simulate Slope Failures"
authors: "Sordo, B., Rathje, E., Kumar, K."
journal: 
layout: publication
categories: 
  - publications
tags:
  - journal
  - mpm
  - fem
  
preprint: https://arxiv.org/abs/2404.15860
doi: https://doi.org/10.1016/j.compgeo.2024.106525
---

Numerical modeling of slope failures seeks to predict two key phenomena: the initiation of failure and the post-failure runout. Currently, most modeling methods for slope failure analysis excel at one of these two but are deficient in the other. For example, the Finite Element Method (FEM) models the initiation of instability well but quickly loses accuracy when modeling large deformations because of mesh distortion, restricting its ability to predict runout. Conversely, the Material Point Method (MPM) utilizes material points which move freely across a background grid, allowing for indefinite deformations without computational issues. However, MPM is restricted in its ability to model slope failure initiation due to limitations of the available boundary conditions and reduced accuracy of its stress distributions. The sequential hybridization of these two methods, initiating a model in FEM and then transferring to MPM, presents an opportunity to accurately capture both initiation and runout by a single model. The exact time for this transfer is not self-apparent, but it must be conducted after the initiation mechanism and before excessive mesh distortion. By simulating two granular column failures and two slope failures, we demonstrate the effectiveness of this hybrid FEM-MPM method and identify the appropriate time to transfer.


## Cite

> Sordo, B., Rathje, E., & Kumar, K. (2024). Sequential Hybrid Finite Element and Material Point Method to Simulate Slope Failures. Computers and Geotechnics. 173 (106525). https://doi.org/10.1016/j.compgeo.2024.106525

### BibLaTeX

```BibLaTeX
@article{sordo2024sequential,
  title={Sequential Hybrid Finite Element and Material Point Method to Simulate Slope Failures},
  author={Sordo, Brent and Rathje, Ellen and Kumar, Krishna},
  journal={Computers and Geotechnics},
  volume={173},
  pages={106525},
  year={2024},
  publisher={Elsevier}
}
```