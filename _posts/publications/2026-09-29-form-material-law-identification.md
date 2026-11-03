---
title: "FORM: Robot Manipulation through Direct Material Law Identification"
authors:
  - "Tretiakov, S."
  - "Zhao, R."
  - "Hsiao, C.-H."
  - "Li, X."
  - "Thorpe, A. J."
  - "Iqbal, H."
  - "Chinchali, S."
  - "Topcu, U."
  - "Kumar, K."
journal: "arXiv preprint arXiv:2609.38105"
categories:
  - publications
layout: publication
tags:
  - journal
  - robotics
  - mpm
  - material-identification
  - weak-form
preprint: https://arxiv.org/abs/2609.38105
doi: 
---

When interacting with an unfamiliar deformable material, a robot lacks prior knowledge of its physical properties and how it will respond to applied forces and motion. Rapid online identification is therefore essential for reliable manipulation. We present FORM (From Observed Response to Material laws), which identifies material properties from a single robot interaction and reuses the recovered model to plan manipulation under new actions and geometries. We use weak-form momentum balance to convert observed material motion and contact forces into linear equations in the unknown material parameters. These equations are assembled using the same material point method discretization as the forward simulator, so identification reduces to linear least-squares solves whose solutions can be used directly for prediction without refitting or conversion. Across four material classes, FORM reduces identification time from roughly 10–25 minutes for iterative baselines to 2–5 seconds, while maintaining competitive accuracy on new motions, initial conditions, and geometries. We demonstrate our approach in simulation and on hardware across four manipulation tasks: elastic rod insertion, golf putting with an elastic club, elastoplastic shaping, and target-volume pouring. In each task, the model identified from a single interaction is reused to plan new motions or manipulate a different geometry. FORM estimates elastic properties within 3.4% and elastoplastic properties within 2%, achieves 72.4–77.8% IoU in dough shaping, and keeps mean pouring error at 3.8 mL across target volumes of 60–160 mL.
