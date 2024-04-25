---
title: "Modeling liquefaction-induced runout of a tailings dam using a hybrid finite element and material point method approach"
authors: "Sordo, B., Rathje, E., Kumar, K."
journal: 
layout: publication
categories: 
  - publications
tags:
  - conference
  - mpm
  - fem
  
preprint: https://arxiv.org/abs/2404.15860
---

Tailings dams impound large amounts of saturated soil which can be highly susceptible to liquefaction. Liquefaction results in a severe loss of strength in the retained soil and potentially failure of the dam. If the dam is breached, a massive debris flow of liquefied soil is then released with potentially disastrous consequences downstream. Numerical models are frequently utilized to predict the liquefaction response of tailings dams and the potential runout,
and these analyses inform engineering decisions regarding hazard avoidance and mitigation. The Finite Element Method (FEM) is a widespread tool which excels at modeling liquefaction triggering and initial movements, but it quickly loses accuracy when modeling large deformations due to mesh distortion. Conversely, the Material Point Method (MPM), a hybrid Eulerian-Lagrangian method, employs particles that move freely across a background grid and can account for large deformations without losing accuracy. However, issues with the accuracy of MPM’s stress distributions and limits associated with the available boundary conditions impair its ability to predict liquefaction initiation. In this paper, we utilize a sequential hybridization of the FEM and MPM methods as a superior alternative to either individually. To demonstrate the efficacy of this hybrid method to simulate the entire process of tailings dam failures from initiation to runout, we model the 1978 Mochikoshi Tailings Dam failure. In this case, the dam collapsed during the main shaking of an earthquake due to the combined effects of the inertial seismic loading and liquefaction. We initiate this model in FEM to capture the immediate effects of the earthquake: the seismic response and liquefaction triggering. Then, we transfer the model into MPM, inheriting the FEM failure mechanism and capturing the runout behavior without mesh issues. The analysis successfully captures the liquefaction triggering and movements, but underestimates the final runout. Further refinements to the MPM phase of the analysis are required to better capture the large runout response.


## Cite

> Sordo, B., Rathje, E., & Kumar, K. (2024). Modeling liquefaction-induced runout of a tailings dam using a hybrid finite element and material point method approach. https://arxiv.org/abs/2404.15860

### BibLaTeX

```BibLaTeX
@misc{sordo2024modeling,
      title={Modeling liquefaction-induced runout of a tailings dam using a hybrid finite element and material point method approach}, 
      author={Brent Sordo and Ellen Rathje and Krishna Kumar},
      year={2024},
      eprint={2404.15860},
      archivePrefix={arXiv},
      primaryClass={physics.geo-ph}
}
```