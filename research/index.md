---
title: Research
layout: collection
permalink: /research/
collection: projects
entries_layout: grid
---

We build world models that let robots predict and act in unfamiliar physical environments. Our work spans physical AI, adaptive world models, computational mechanics, learned simulation, in-context learning, differentiable control, and embodied autonomy. Each area below lists representative papers.

## Physics-grounded perception and material identification

We combine 3D Gaussian Splatting, physical constraints, and weak-form mechanics to infer material behavior from observations. Weak-form momentum balance turns observed motion and contact forces into linear equations in the unknown material parameters. The same equations test whether learned or generated motion is physically consistent.

* [FORM: Robot Manipulation through Direct Material Law Identification]({% post_url publications/2026-09-29-form-material-law-identification %}) (2026)
* [Damage detection and identification using a differentiable material point method]({% post_url publications/2026-07-01-damage-detection-differentiable-mpm %}) (2026)
* [Structural identification of material properties and load parameters using a differentiable material point method]({% post_url publications/2025-08-22-differentiable-mpm-structural-identification %}) (2025)
* [From images to properties: a NeRF-driven framework for granular material parameter inversion]({% post_url publications/2025-07-11-nerf-granular-inversion %}) (2025)

## Adaptive learned simulators

We develop graph network simulators (GNS), operator-learning methods, and reduced-order models that respect conservation laws and material-dependent dynamics. A material-conditioned simulator adapts in context, so a world model can generalize to an unfamiliar material from limited interaction data.

* [Parameter-Efficient Conditioning for Material Generalization in Graph-Based Simulators]({% post_url publications/2025-11-07-gns-material-generalization %}) (2025)
* [Learning Generalizable Neural Operators for Inverse Problems]({% post_url publications/2025-12-19-neural-operators-inverse-problems %}) (2025)
* [Basis-to-Basis Operator Learning using Function Encoders]({% post_url publications/2024-10-02-function-encoder %}) (2025)
* [SetONet: A Deep Set-based Operator Network for Solving PDEs]({% post_url publications/2025-05-08-setonet %}) (2025)
* [Graph Neural Network-based surrogate model for granular flows]({% post_url publications/2023-05-09-gns-column %}) (2024)

## Differentiable world models and control

We combine differentiable physics, reduced-order simulation, and function-encoder representations for fast prediction and planning in deformable environments. The aim is to adapt both the physical model and the control strategy online, without retraining and without repeated high-fidelity simulation.

* [End-to-End Learning of Safe Optimal Feedback Control in High Dimensions with Control Barrier Function Layers]({% post_url publications/2026-07-22-safe-optimal-feedback-cbf %}) (2026)
* [Neural Operators for Multi-Task Control and Adaptation]({% post_url publications/2026-04-03-neural-operators-multi-task-control %}) (2026)
* [Zero-Shot Function Encoder-Based Differentiable Predictive Control]({% post_url publications/2025-11-07-zero-shot-dpc %}) (L4DC 2026)
* [Zero-Shot Transferable Solution Method for Parametric Optimal Control Problems]({% post_url publications/2025-09-22-zero-shot-optimal-control %}) (ACC 2026)
* [Inverse analysis of granular flows using differentiable graph neural network simulator]({% post_url publications/2024-01-17-gns-inverse %}) (2024)

## Embodied autonomy in complex physical environments

We develop physically viable world models for robotic construction, soft-material manipulation, deformable-terrain navigation, and multi-robot coordination. A physically viable world model represents the physical structure that determines the outcome of an action, so it can answer intervention queries. Applications extend to autonomous parafoil flight and lunar construction, where the robot must infer physical properties and environmental conditions during operation.

* [Physically Viable World Models: A Case for Query-Conditioned Embodied AI]({% post_url publications/2026-05-28-physically-viable-world-models %}) (2026)
* [Path Planning in Physically Viable World Models]({% post_url publications/2026-07-01-path-planning-physically-viable-world-models %}) (2026)
* [Physics-Aware Gaussian Splat World Models for Place-Based Climate Serious Games]({% post_url publications/2026-11-02-gaussian-splat-world-models-serious-games %}) (HICSS 2027)

## AI for engineering and natural hazards

We build computational methods and open research infrastructure through [Chishiki.ai](https://www.chishiki-ai.org/) and [DesignSafe-CI](https://www.designsafe-ci.org/) for scientific discovery, simulation, and autonomous engineering systems. We also test when machine learning is trustworthy in safety-critical geotechnical prediction.

* [A Critical Assessment of PINNs and Operator Learning for Geotechnical Engineering]({% post_url publications/2025-12-30-pinns-operator-learning-assessment %}) (2025)
* [Formal verification of tree-based machine learning models for lateral spreading]({% post_url publications/2026-03-17-formal-verification-lateral-spreading %}) (2026)
* [A Decade of DesignSafe: Enabling Open Science in Natural Hazards]({% post_url publications/2025-07-30-decade-designsafe %}) (2025)
* [Hybrid Finite-Element and Material Point Method for Modeling Liquefaction-Induced Tailings Dam Failures]({% post_url publications/2024-12-11-hybrid-fem-mpm-tailings-dam %}) (2025)

## Simulation codes

Our learned simulators and world models build on numerical methods that the group develops and maintains as open-source codes.

<div class="course-grid"> 

  <div class="course-card">
    <img src="{{site.url}}/images/geoelements/logo.png" alt="sciml" class="course-image">
    <div class="card-content">
      <div>
        <h3>GNS and Differentiable MPM</h3>
        <p>The Graph Network Simulator (GNS) is a learned simulator for particulate and fluid systems. Differentiable MPM passes gradients through Material Point Method simulations for inverse analysis and design.</p>
      </div>
    </div>
    <a href="{{ site.url }}/research/sciml/" class="launch-button">Discover SciML</a>
  </div>

  <div class="course-card" href="{{ site.url }}/research/mpm/">
    <img src="{{site.url}}/images/geoelements/logo.png" alt="MPM" class="course-image">
    <div class="card-content">
      <div>
        <h3>Material Point Method</h3>
        <p>The Material Point Method (MPM) simulates large-deformation problems such as landslides, soft-material manipulation, and robot interaction with deformable terrain.</p>
      </div>
    </div>
    <a href="{{ site.url }}/research/mpm/" class="launch-button">Discover MPM</a>
  </div>

  <div class="course-card">
    <img src="{{site.url}}/images/geoelements/logo.png" alt="lbm" class="course-image">
    <div class="card-content">
      <div>
        <h3>LBM/DEM: Lattice Boltzmann & Discrete Element Method</h3>
        <p>The Lattice Boltzmann equation Method (LBM) is a meso-scale fluid solver for modeling grain-scale fluid flow. The Discrete-Element Method (DEM) is coupled with LBM to model particle-fluid interactions at the mesoscale.</p>
      </div>
    </div>
    <a href="{{ site.url }}/research/lbm/" class="launch-button">Discover LBM</a>
  </div>
</div>


<h2 style="text-align: center;">Research Spotlights</h2>
