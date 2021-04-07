---
title: Mip-NeRF A Multiscale Representation for Anti-Aliasing Neural Radiance Fields
date: 2021-04-02
permalink: /posts/2021/04/02/paper_mipnerf/
categories:
- paper-reading
tags:
  - arxiv
  - 3D reconstruction
  - neural implicit representation
---

point sampling in NeRF leads to aliasing
- scpecially for scenes where caneras are from different distances
- integrate posenc in a cone instead of sample form a point
- single MLP, no coarse and fine network, but still have coarse and fine points: not needed, scale modeled in IPE
  - update weight before sample fine points, leap-frog