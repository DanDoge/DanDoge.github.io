---
title: NeRF-- Neural Radiance Fields without Known Camera Parameters
date: 2021-02-20
permalink: /posts/2021/02/20/paper_nerfmm/
categories:
- paper-reading
tags:
  - arxiv
  - neural rendering
---

NeRF: camera parameters from COLMAP
- learned camera parameters?
  - jointly train parameters with MLPs
  - assumptions: principle points are at center
  - axis-angle representation of rotation
  - initialization matters: R=I, t=0
  - train and drop initial NeRF, keep camera
- drop hierarchical sampling: for a weaker baseline or stable training?
- 128 hidden size...