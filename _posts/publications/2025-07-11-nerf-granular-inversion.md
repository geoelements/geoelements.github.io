---
title: "From images to properties: a NeRF-driven framework for granular material parameter inversion"
authors:
  - "Hsiao, C. H."
  - "Kumar, K."
journal: "arXiv preprint arXiv:2507.09005"
categories:
  - publications
layout: publication
tags:
  - journal
  - ml
  - nerf
  - mpm
  - inverse-problems
preprint: https://arxiv.org/abs/2507.09005
doi:
---

We introduce a novel framework that integrates Neural Radiance Fields (NeRF) with Material Point Method (MPM) simulation to infer granular material properties from visual observations. Our approach begins by generating synthetic experimental data, simulating a plow interacting with sand. The experiment is rendered into realistic images as the photographic observations. These observations include multi-view images of the experiment's initial state and time-sequenced images from two fixed cameras. Using NeRF, we reconstruct the 3D geometry from the initial multi-view images, leveraging its capability to synthesize novel viewpoints and capture intricate surface details. The reconstructed geometry is then used to initialize material point positions for the MPM simulation, where the friction angle remains unknown. We render images of the simulation under the same camera setup and compare them to the observed images. By employing Bayesian optimization, we minimize the image loss to estimate the best-fitting friction angle. Our results demonstrate that friction angle can be estimated with an error within 2 degrees, highlighting the effectiveness of inverse analysis through purely visual observations. This approach offers a promising solution for characterizing granular materials in real-world scenarios where direct measurement is impractical or impossible.
