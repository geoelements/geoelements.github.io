---
title: "Minority Report: A graph network oracle for in situ visualization"
authors: "Kumar, K., Navratil, P., Solis, A., Vantassel, J"
journal: 
layout: publication
categories: 
  - publications
tags:
  - conference
  - ml
  - insitu
  - viz
  
preprint: 
---

In situ visualization techniques are hampered by a lack of foresight: crucial simulation phenomena can be missed due to a poor sampling rate or insufficient detail at critical timesteps. Keeping a human in the loop is impractical, and defining statistical triggers can be difficult. This paper demonstrates the potential for using a machine-learning-based simulation surrogate as an oracle to identify expected critical regions of a large-scale simulation. These critical regions are used to drive the in situ analysis, providing greater data fidelity and analysis resolution with an equivalent I/O budget to a traditional in situ framework. We develop a distributed asynchronous in situ visualization by integrating TACC Galaxy with CB-Geo MPM for material point simulation of granular flows. We employ a PyTorch-based 3D Graph Network Simulator (GNS) trained on granular flow problems as an oracle to predict the dynamics of granular flows. Critical regions of interests are manually tagged in GNS for in situ rendering in MPM.
