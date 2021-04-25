---
title: "Microsimulation Analysis for Network Traffic Assignment (MANTA)
at Metropolitan‑Scale for Agile Transportation Planning"
authors: 
  - "Yedavalli, P."
  - "Kumar, K."
  - "Waddell, P."
journal: "Transportmetrica A: Transport Science"
categories: 
  - publications
layout: publication
tags:
  - journal
  - gpu
  - microsim
  - traffic-flow
preprint: https://arxiv.org/abs/2007.03614
---

## Abstract:

Abrupt changes in the environment, such as unforeseen events due to climate change, have triggered massive and precipitous changes in human mobility. The ability to quickly predict traffic patterns in different scenarios has become more urgent to support short-term operations and long-term transportation planning. This requires modeling entire metropolitan areas to recognize the upstream and downstream effects on the network. However, there is a well-known trade-off between increasing the level of detail of a model and decreasing computational performance. To achieve the level of detail required for traffic microsimulation, current implementations often compromise by simulating small spatial scales, and those that operate at larger scales often require access to expensive high-performance computing systems or have computation times on the order of days or weeks that discourage productive research and real-time planning. This paper addresses the performance shortcomings by introducing a new platform, MANTA (Microsimulation Analysis for Network Traffic Assignment), for traffic microsimulation at the metropolitan-scale. MANTA employs a highly parallelized GPU implementation that is capable of running metropolitan-scale simulations within a few minutes. The runtime to simulate all morning trips, using half-second timesteps, for the nine-county San Francisco Bay Area is just over four minutes, not including routing and initialization. This computational performance significantly improves the state of the art in large-scale traffic microsimulation. MANTA expands the capacity to analyze detailed travel patterns and travel choices of individuals for infrastructure planning. 