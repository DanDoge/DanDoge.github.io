---
title: BeautyGlow On-Demand Makeup Transfer Framework with Reversible Generative Network
date: 2020-02-22
categories:
- paper-reading
tags:
- image synthesis
- CVPR
---


task: generate a specific makeup style
- needs a encoder to interpolate latent spaces, which doesnot exist in GAN
- BeautyGlow: decomposes latent vector into makeup features and facial identity features
    - in the same space
    - feature of image = W * (makeup) + (I - W) * (identity)
    - then switch features, gen. images
    - Glow based method
- perceptual loss
- makeup loss
    - makeup vector should be close to center of all makeup vectors
    - before/after-makeup vector should be close to center of its classes
        - kind of split the space into two halves, one for identity one for makeup
