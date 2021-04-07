---
title: KiloNeRF Speeding up Neural Radiance Field with Thousands of Tiny MLPs
date: 2021-04-06
permalink: /posts/2021/04/06/paper_kilonerf/
categories:
- paper-reading
tags:
  - arxiv
  - 3D reconstruction
  - neural rendering
  - neural implicit field
---

each individual mlp responsible for a tiny space
- knowledge distilled from a NeRF
- empty space skipping and early ray termination
  - so, basically a mlp version of octree with feature
  - L2 regularization on last two layers to mimic nerf's smooth view dependent color prior