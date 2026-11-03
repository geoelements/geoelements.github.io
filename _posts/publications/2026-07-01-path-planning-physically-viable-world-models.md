---
title: "Path Planning in Physically Viable World Models"
authors:
  - "Low, S. A."
  - "Hsiao, C.-H."
  - "Li, X."
  - "Thorpe, A. J."
  - "Topcu, U."
  - "Kumar, K."
journal: "arXiv preprint arXiv:2607.00673"
categories:
  - publications
layout: publication
tags:
  - journal
  - robotics
  - world-models
  - gaussian-splatting
  - navigation
preprint: https://arxiv.org/abs/2607.00673
doi: 
---

Robots deployed in unstructured outdoor environments often plan from scene reconstructions collected before deployment because operators cannot remap large or remote sites before every mission. As a result, robots must make long-horizon planning decisions using stale maps that assume the terrain remains unchanged, even though physical changes to the environment may render previously feasible routes unsafe or unreachable at execution time. We present a physically viable world model for evaluating what-if queries for robot navigation under future terrain change. The system augments reconstructed 3D Gaussian splat scenes with physics-based simulation to generate physically modified versions of the same environment without recollecting sensor data or rebuilding the map. We then implement a terrain-aware planner that accounts for physical events, obstacles, and deformations that are simulated by the world model. This allows robots and human operators to evaluate whether planned routes remain feasible before committing to a planned route, particularly in constrained environments where retreat or recovery may become impossible once conditions change. We evaluate the system on a real outdoor field site in Central Texas using simulated flooding across multiple severity levels. We measure route and mission feasibility as terrain conditions deteriorate under physically simulated interventions. Our results show that physically viable world models expose long-horizon route failures and rerouting behavior that are not apparent when planning only on the original reconstructed environment, allowing robots to evaluate how future terrain changes may affect route feasibility before deployment.
