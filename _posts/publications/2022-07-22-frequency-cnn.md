---
title: "A frequency-velocity CNN for developing near-surface 2D Vs images from linear-array, active-source wavefield measurements"
authors: "Abbas, A, Vantassel, J., Cox, B. R., Kumar, J., Crocker, J"
journal: 
layout: publication
categories: 
  - publications
tags:
  - ml
  - fwi
  
preprint: https://arxiv.org/abs/2207.09580
---

This paper presents a frequency-velocity convolutional neural network (CNN) for rapid, non-invasive 2D shear wave velocity (Vs) imaging of near-surface geo-materials. Operating in the frequency-velocity domain allows for significant flexibility in the linear-array, active-source experimental testing configurations used for generating the CNN input, which are normalized dispersion images. Unlike wavefield images, normalized dispersion images are relatively insensitive to the experimental testing configuration, accommodating various source types, source offsets, numbers of receivers, and receiver spacings. We demonstrate the effectiveness of the frequency-velocity CNN by applying it to a classic near-surface geophysics problem, namely, imaging a two-layer, undulating, soil-over-bedrock interface. This problem was recently investigated in our group by developing a time-distance CNN, which showed great promise but lacked flexibility in utilizing different field-testing configurations. Herein, the new frequency-velocity CNN is shown to have comparable accuracy to the time-distance CNN while providing greater flexibility to handle varied field applications. The frequency-velocity CNN was trained, validated, and tested using 100,000 synthetic near-surface models. The ability of the proposed frequency-velocity CNN to generalize across various acquisition configurations is first tested using synthetic near-surface models with different acquisition configurations from that of the training set, and then applied to experimental field data collected at the Hornsby Bend site in Austin, Texas, USA. When fully developed for a wider range of geological conditions, the proposed CNN may ultimately be used as a rapid, end-to-end alternative for current pseudo-2D surface wave imaging techniques or to develop starting models for full waveform inversion. 
