---
title: Pixel2Mesh++ Multi-View 3D Mesh Generation via Deformation
date: 2019-10-25
categories:
- paper-reading
tags:
- 3D reconstruction
- 3D generation
- ICCV
---

## Pixel2Mesh++ Multi-View 3D Mesh Generation via Deformation

input: color images, camera poses

point2mesh: deform an initial shape conditioned on images

pipeline
- images -> geometry / semantic feature
- refine output of pixel2mesh
    - propose deformation for each vertex
    - assign features from image to each vertex
        - and statistics -> cross-view learning?
    - softmax of proposals -> differentiable
