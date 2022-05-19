---
title: "Using Convolutional Neural Networks (CNN) to develop starting models for 2D full waveform inversion"
authors: 
  - "Vantassel, J. P."
  - "Kumar, K."
  - "Cox, B. R."
journal: Geophysics
categories:
  - publications
tags:
  - journal
  - ml
layout: publication
preprint: https://arxiv.org/abs/2104.01626
---

Non-invasive subsurface imaging using full waveform inversion (FWI) has the potential to fundamen-tally change engineering site characterization by enabling the recovery of high resolution 2D/3D maps ofsubsurface stiffness.  Yet, the accuracy of FWI remains quite sensitive to the choice of the initial start-ing model due to the complexity and non-uniqueness of the inverse problem.  In response,  we presentthe  novel  application  of  convolutional  neural  networks  (CNNs)  to  transform  an  experimental  seismicwavefield acquired using a linear array of surface sensors directly into a robust starting model for 2DFWI.  We  begin  by  describing  three  key  steps  used  for  developing  the  CNN,  which  include:  selectionof a network architecture, development of a suitable training set, and performance of network training.The ability of the trained CNN to predict a suitable starting model for 2D FWI was compared againstother commonly used starting models for a classic near-surface imaging problem; the identification of anundulating, two-layer, soil-bedrock interface.  The CNN developed during this study was able to predictcomplex 2D subsurface images of the testing set directly from their seismic wavefields with an averagemean absolute percent error of 6%.  When compared to other common approaches, the CNN approachwas able to produce starting models with smaller seismic image and waveform misfits, both before andafter FWI. The ability of the CNN to generalize to subsurface models which were dissimilar to the onesupon which it was trained was assessed using a more complex, three-layered model.  While the predictiveability of the CNN was slightly reduced, it was still able to achieve seismic image and waveform misfitscomparable to the other commonly used starting models.  This study demonstrates that CNNs have greatpotential as a tool for developing good starting models for FWI, which are critical for producing accurateFWI results.
