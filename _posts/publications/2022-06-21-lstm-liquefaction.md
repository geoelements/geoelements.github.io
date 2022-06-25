---
title: " Hybrid Finite Element and Material Point Method to simulate granular column collapse from failure initiation to runout"
authors: "Sordo, B., Rathje, E., Kumar, K."
journal: 
layout: publication
categories: 
  - publications
tags:
  - conference
  - mpm
  - fem
  
preprint: https://arxiv.org/abs/2206.07169
---

The performance evaluation of a potentially unstable slope involves two key components: the initiation of the slope failure and the post-failure runout. The Finite Element Method (FEM) excels at modeling the initiation of instability but quickly loses accuracy in modeling large-deformation problems due to mesh distortion. Hence, the FEM is unable to accurately model post-failure slope runout. Hybrid Eulerian-Lagrangian methods, such as the Material Point Method (MPM), offer a promising alternative for solving large-deformation problems, because particles can move freely across a background mesh, allowing for large deformation without computational issues. However, the use of moving material points in MPM for integration rather than the fixed Gauss points of the FEM reduces the accuracy of MPM in predicting stress distribution and thus failure initiation. We have created a hybrid method by initiating a failure simulation in FEM and subsequently transferring the coordinates, velocities, and stresses to MPM particles to model the runout behavior, combining the strength of both methods. We demonstrate the capability of the hybrid approach by simulating the collapse of a frictional granular column, comparing it to an empirical solution, and evaluating a suitable time to transfer from FEM to MPM by trialing multiple iterations with transfers at different stages of the collapse. 
