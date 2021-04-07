---
title: Baking Neural Radiance Fields for Real-time View Synthesis
date: 2021-04-07
permalink: /posts/2021/04/07/paper_bnerf/
categories:
- paper-reading
tags:
  - arxiv
  - 3D reconstruction
  - neural rendering
  - neural implicit field
---

goal: run nerf on a macbook
- train a nerf -> store grid values at a sparse grid
  - opacity, diffuse color, feature vector for view dependent affects
  - feature vector is integrated, and then transformed by an mlp -> rendered per ray
    - this mlp can be trained after storing -> fine tuning
- Cauthy loss for density: sparse prior
  - on coarse samples only