---
title: "Investigating the Effect of CPT in Lateral Spreading Prediction Using Explainable AI"
authors: "Hsiao, C. H., Rathje, E., Kumar, K."
journal: 
layout: publication
categories: 
  - publications
tags:
  - conference
  - xai
  
preprint: https://arxiv.org/abs/2503.13389
doi: https://doi.org/10.1061/9780784485989.012
---

This study proposes an autoencoder approach to extract latent features from cone penetration test profiles to evaluate the potential of incorporating CPT data in an AI model. We employ autoencoders to compress 200 CPT profiles of soil behavior type index (Ic) and normalized cone resistance (qc1Ncs) into ten latent features while preserving critical information. We then utilize the extracted latent features with site parameters to train XGBoost models for predicting lateral spreading occurrences in the 2011 Christchurch earthquake. Models using the latent CPT features outperformed models with conventional CPT metrics or no CPT data, achieving over 83% accuracy. Explainable AI revealed the most crucial latent feature corresponding to soil behavior between 1-3 meter depths, highlighting this depth range's criticality for liquefaction evaluation. The autoencoder approach provides an automated technique for condensing CPT profiles into informative latent features for machine-learning liquefaction models. 


## Cite

> Hsiao, C. H., Rathje, E. M., & Kumar, K. (2025). Investigating the Effect of CPT in Lateral Spreading Prediction Using Explainable AI. In Geotechnical Frontiers 2025 (pp. 104-115).

### BibLaTeX

```BibLaTeX
@incollection{hsiao2025investigating,
  title={Investigating the Effect of CPT in Lateral Spreading Prediction Using Explainable AI},
  author={Hsiao, Cheng-Hsi and Rathje, Ellen M and Kumar, Krishna},
  booktitle={Geotechnical Frontiers 2025},
  year={2025},
  pages={104--115}
}
```