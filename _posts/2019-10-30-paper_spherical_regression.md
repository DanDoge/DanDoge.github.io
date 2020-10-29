---
title: Spherical Regression Learning Viewpoints, Surface Normals and 3D Rotations on n-Spheres
date: 2019-10-30
categories:
- paper-reading
tags:
- pose estimation
- CVPR
---

## Spherical Regression Learning Viewpoints, Surface Normals and 3D Rotations on n-Spheres

regression methods on continuous problems are not popular
- classification based approaches being more reliable
    - contained in a probability n-simplex geometry defined by softmax
    - gradients being constrained
- continuous output also contained in closed geometrical manifolds
    - introducing n-spheres
- e.g. nn can be viewed as x -> o -> p
    - where o being latent embedding and p being activated o
    - explicit activation function serves as a constraint
        - and partial L / o is bounded
        - not true in regression case
- n-spheres constraint
    - we need a. activation function s.t.
        - output p lieves on a n-sphere
        - gradient w.r.t. o also depends only on p
    - and seperate sign and magnitute
    
