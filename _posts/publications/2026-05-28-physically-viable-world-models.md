---
title: "Physically Viable World Models: A Case for Query-Conditioned Embodied AI"
authors:
  - "Thorpe, A. J."
  - "Tretiakov, S."
  - "Hsiao, C.-H."
  - "Low, S. A."
  - "Li, X."
  - "Iqbal, H."
  - "Bhatt, N. P."
  - "Topcu, U."
  - "Kumar, K."
journal: "arXiv preprint arXiv:2605.30542"
categories:
  - publications
layout: publication
tags:
  - journal
  - robotics
  - world-models
  - ml
preprint: https://arxiv.org/abs/2605.30542
doi: 
---

World models for embodied AI must be physically viable: constructed to answer intervention queries by representing the physical structure governing action outcomes, rather than merely predicting future observations. Existing observation-predictive world models can produce visually plausible but physically wrong rollouts. This failure is structural; distinct physical systems can look identical yet diverge under intervention. We expose this problem with controlled benchmarks that fix the visible scene while varying latent physics. We show that such models may recommend infeasible actions, mispredict interaction outcomes, or certify unsafe behavior. We argue that embodied AI requires world models that identify the simplest physical abstraction sufficient to answer an intervention query. Such a model comprises modular components, including environment representation, latent state and parameter estimation, action specification, interventional dynamics, and query-level response. An autonomous orchestrator should identify the relevant abstraction and compose compatible learned and structured components per query. When closed-form physics is unavailable, uncertain, or costly, the transition model may be analytic, simulated, learned, or hybrid, but it must preserve the structure that determines interventional outcomes. This decomposition makes the model interpretable, its components verifiable, and its outputs auditable against the query. It also provides a design principle for new world models and a feasibility test for existing ones: the right abstraction is not the most detailed model of the world, but the simplest model that preserves the distinctions relevant to the query. We demonstrate this approach on queries that existing systems fail to answer correctly, and outline how an orchestrator can dynamically assemble and adapt physically viable models for planning, control, and verification.
