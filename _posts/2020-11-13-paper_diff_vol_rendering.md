---
title: Differentiable Volumetric Rendering Learning Implicit 3D Representations without 3D Supervision
date: 2020-11-13
permalink: /posts/2020/11/13/paper_diff_vol_rendering/
categories:
- paper-reading
tags:
  - CVPR
  - 3D reconstruction
---

kind of like what I have tried before
- point -> occupancy -> surface -> depth map -> surface points -> color
  - problem: how gradient flow through surface? refer to paper for details
- implicit function conditioned on z from image
  - how can that work with NeRF?
    - if given a latent variable extracted (and averaged) from some images, NeRF should be able to extend to generalize on various scenes, which means: no parameter should be scene dependent including params. in CNN and MLP
    - if we do not generalize NeRF, then the additional model capacity from CNN need to be subtracted (somehow), if we are gonna compare that result with NeRF