---
title: PlenOctrees for Real-time Rendering of Neural Raidance Fields
date: 2021-04-06
permalink: /posts/2021/04/06/paper_plenoctree/
categories:
- paper-reading
tags:
  - arxiv
  - 3D reconstruction
  - neural rendering
  - neural implicit field
---

NeRF-SH
- a base color, and several view dependent color: sh coef 
- build a plen octree after training: only to speed up testing
  - sparsity loss for robust conversion
  - early-stopping ray tracing