---
title: Learning Category-Specific Mesh Reconstruction from Image Collections
date: 2019-08-09
categories:
- paper-reading
tags:
- 3D reconstruction
- ECCV
---

## Learning Category-Specific Mesh Reconstruction from Image Collections

human brain: previous birds in 3d ==> new birds in 3d, given its 2d view

input data: no 3d gt needed!
- 2d image
- object category
- foreground masks
- semantic keypoints

outputs
- shape
    - actually diff. with mean shape
    - mean shape: predetermined(similar to hand reconstruction SOTA paper...which enables high accuracy on relatively small data, maybe)
        - starting with convex hull of keypoints, then finetuned(how? refer to code on github, some models are manually selected?)
- camera / viewpoint
- texture
    - texture flow: flow based on input image
    - UV mapping: paint on a unit ball, then deform the ball to, say, a bird

losses
- key points, camera, texture
- and some priors
    - symmetry
    - smoothness
    - deformation regularization: small diff. matrix
    - entropy of keypoint association matrix
        - keypoint as a distribution on vertices

Neural mesh renderer
- read later...
