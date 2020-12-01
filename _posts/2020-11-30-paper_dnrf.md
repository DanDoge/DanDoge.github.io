---
title: Deformable Neural Radiance Fields
date: 2020-11-30
permalink: /posts/2020/11/30/paper_dnrf/
categories:
- paper-reading
tags:
  - arxiv
  - neural rendering
  - neural implicit representation
---

model non-rigidly deforming scene
- warp each point to canonical 5d nerf
  - latent deformation code per image
  - estimate deformation params. v, s, t
- zeroing out hf for stable(non-overfitting) training
- elastic reg.: local jacobian should be close to a rotation matrix
- robust loss: refer to paper, read later
- bg: pre-assign some point to be stable
- positional encoding: low freq then high freq, anti-overfitting
  - NTK view of positional encoding: read later
- softplus for density, why?
