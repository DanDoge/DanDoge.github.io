---
title: NeMI Unifying Neural Radiance fieldswith Multiplane Images for Novel View Synthesis
date: 2021-04-07
permalink: /posts/2021/04/07/paper_nemi/
categories:
- paper-reading
tags:
  - arxiv
  - 3D reconstruction
  - neural rendering
---

nvs from a single image
- seems like strong prior needs to be learned
- image -> feature + depth(sampled in disparity) -> color and sigma -> render under novel viewpoint, ray marching
- L1 and SSIM losses