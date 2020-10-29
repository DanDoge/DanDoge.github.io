---
title: Texture Fields Learning Texture Representations in Function Space
date: 2019-10-19
categories:
- paper-reading
tags:
- GAN
- image synthesis
- texture synthesis
---

## Texture Fields Learning Texture Representations in Function Space

representations of texture?
- voxel with color?
    - computational cost
- 2D texture atlas and UV mapping
    - assume known topology and predefined mesh
- surface texture as a continuous function in 3D space
    - regression task
    - conditioned on shape embedding and texture latent variable
        - pointnet encoder for 3D points sampled
        - image encoder: residual network
- loss
    - L_1 of gen. images
- need to be implemented
