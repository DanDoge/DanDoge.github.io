---
title: SDFDiff Differentiable Rendering of Signed Distance Fields for 3D Shape Optimization
date: 2020-11-24
permalink: /posts/2020/11/24/paper_sdfdiff/
categories:
- paper-reading
tags:
  - CVPR
  - 3D reconstruction
---

sdf guarantee watertight surface? -> smooth prior

sample sdf on grids, ray casting find a intersection
- ray casting on GPU, since it donot need to be differentiable, maybe i should learn how to write cuda code
- trilinear interpolation of normal
- what a huge network

