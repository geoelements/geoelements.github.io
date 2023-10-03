---
title: "An inverse analysis of fluid flow through granular media using differentiable lattice Boltzmann method"
authors: "Wang, Q., Kumar, K."
journal: 
layout: publication
categories: 
  - publications
tags:
  - ml
  - sciml
  - diff-programming
  - journal
preprint: https://arxiv.org/pdf/2310.00810.pdf
---

In this study, we introduce an effective method for the inverse analysis of fluid flow problems,
focusing on accurately determining boundary conditions and characterizing the physical properties of gran-
ular media, such as permeability, and fluid components, like viscosity. Our primary aim is to deduce either
constant pressure head or pressure profiles, given the known velocity field at a steady-state flow through
a conduit containing obstacles, including walls, spheres, and grains. We employ the lattice Boltzmann
Method (LBM) combined with Automatic Differentiation (AD), facilitated by the GPU-capable Taichi
programming language (AD-LBM). A lightweight tape is utilized to generate gradients for the entire LBM
simulation, enabling end-to-end backpropagation. For complex flow paths in porous media, our AD-LBM
approach accurately estimates the boundary conditions leading to observed steady-state velocity fields and
consequently derives macro-scale permeability and fluid viscosity. Our method demonstrates significant ad-
vantages in terms of prediction accuracy and computational efficiency, offering a powerful tool for solving
inverse fluid flow problems in various applications