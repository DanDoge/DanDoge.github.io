---
title: AutoInt Automatic Integration for Fast Neural Volume Rendering
date: 2020-12-07
permalink: /posts/2020/12/07/paper_autoint/
categories:
- paper-reading
tags:
  - arxiv
  - neural implicit representation
  - 3D reconstruction
---

since nerf is evaluating a intergration
- build a grad/integral network: share params from diff. rules: (fg)' = f'g + g'f
- inference speed for accuracy
  - 10x faster but -10 in psnr...