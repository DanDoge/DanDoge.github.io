---
title: DISN Deep Implicit Surface Network for High-quality Single-view 3D Reconstruction
date: 2019-09-15
categories:
- paper-reading
tags:
- 3D reconstruction
- NIPS
---

## DISN Deep Implicit Surface Network for High-quality Single-view 3D Reconstruction

limitations
- low res.
- fixed representation but limied topology(e.g. holes)
- Chanfer Distance or EMD: approx. metrics
- study global features but ignore details
    - introduce a local feature module
    - project query point into input image -> get a local patch

Signed Distance Functions
- implicit representation
- propose a DISN to predict SDF
- potential to generate infnite res. 3D model
- continuous function: R^3 -> R, SDF(p) = distance from surface

DISN
- regress SDF
    - based on global feature and local feature
- local feature?
    - extracted from endoder, then concat
- map 3d point to 2d image
    - estimate cam pose first!
- marching cubes to get iso-surface
