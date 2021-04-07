---
title: MVSNeRF Fast Generatizable Radiance Field Reconstruction from Multi-View Stereo
date: 2021-04-07
permalink: /posts/2021/04/07/paper_mvsnerf/
categories:
- paper-reading
tags:
  - arxiv
  - 3D reconstruction
  - neural rendering
---

train a generalizable nerf
- generalize with as few as three images
- images -> image[0] as pivot image -> cost volume from variance in feature -> 3dconv -> neural encoding volume -> rendering
  - pixel color also used (and trained) for rendering