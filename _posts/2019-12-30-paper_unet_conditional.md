---
title: A Variational U-Net for Conditional Appearance and Shape Generation
date: 2019-12-30
categories:
- paper-reading
tags:
- CVPR
- image synthesis
---

mapping from shape to target image
- condition on latent representation of variational AE for appearence
- shape? geometrical information: loc, shape, pose
- joint prior: p(x | y, z), q(z | x, y)
    - similar to CVPR 2019
- perceptual quality? perceptual loss
