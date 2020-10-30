---
title: Learning Representations and Generative Models for 3D Point Clouds
date: 2019-12-09
categories:
- paper-reading
permalink: /posts/2019/12/09/paper_representation_generative_model_pc/
tags:
- ICLR
- 3D generation
---

point cloud
- hard to manipulate in raw form
    - and not suited for generative models
- introducing metrics
    - JSD, coverage, MMD
- representation model
    - 2048 points
    - 1D conv -> encodes points independently
- generative model
    - lGAN: GAN in latent space
    - shape completion
