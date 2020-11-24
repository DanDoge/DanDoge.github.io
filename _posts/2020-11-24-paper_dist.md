---
title: DIST Rendering Deep Implicit Signed Distance Function with Differentiable Sphere Tracing
date: 2020-11-24
permalink: /posts/2020/11/24/paper_dist/
categories:
- paper-reading
tags:
  - CVPR
  - neural rendering
---

optimize forward and backward pass of neural rendering
- tldr, coarse-to-fine, aggressive ray marching
- apply to any sdf model
- sample per 4 pixel and double each 3 iterations
  - at 6 iter, back to origin res
- aggressive ray marching
  - x = x + 1.5 * sdf(x) * rd
  - sample points under surface
- converge if a pixel donot confuse with its neighbor
  - refer to supp. for details
- gradient bp
  - tbh, i donot understand it


