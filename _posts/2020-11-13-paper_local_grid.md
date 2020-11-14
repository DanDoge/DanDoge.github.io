---
title: Local Implicit Grid Representations for 3D Scenes
date: 2020-11-13
permalink: /posts/2020/11/13/paper_local_grid/
categories:
- paper-reading
tags:
  - CVPR
  - 3D reconstruction
---

reconstruct 3d model in an intermediate scale
- utilize part similarity across models
- improved generalizability
- part autoencoder
  - part -> latent, a implicit function f(pixel pos, latent) -> occupancy
  - test time: sparse point cloud -> coarse grid, for each grid, optimize a part reconstruction