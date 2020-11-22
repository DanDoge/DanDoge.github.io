---
title: Cycle-Consistent Generative Rendering for 2D-3D Modality Translation
date: 2020-11-20
permalink: /posts/2020/11/20/paper_ccgr/
categories:
- paper-reading
tags:
  - arxiv
  - 3D reconstruction
---

contributions
- a cyclic gen model on **unpaired 2D and 3D data, w/o camera calibration**
- adv methods for a strong prior on shape/texture/poses and renders
- cyclegan like training process
  - shape -> latent var -> canonical shape, +random texture/pose -> rendered image
  - image -> latent var( -> canonical shape), pose, texture

