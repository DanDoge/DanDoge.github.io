---
title: Convolutional Occupancy Networks
date: 2020-11-13
permalink: /posts/2020/11/13/paper_conv_occu_net/
categories:
- paper-reading
tags:
  - ECCV
  - 3D reconstruction
---

previous implicit models are prevented from structured reasoning
- only act in global scale -> overly smoothed reconstructions
  - positional encoding may help
- fc nets donot allow for integrating local features or translational equivariance
  - but, fc nets can achieve these from the smooth prior in MLP
- point -> feature -> proj to predefined plane -> refine feature
- extension: predefined plane -> dynamic plane
  - no significant performance gain compared to predefined plane
  - not to say with positional encoding introduced