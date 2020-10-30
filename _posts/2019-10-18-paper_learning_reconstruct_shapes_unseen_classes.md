---
title: Learning to Reconstruct Shapes from Unseen Classes
date: 2019-10-18
categories:
- paper-reading
permalink: /posts/2019/10/18/paper_learning_reconstruct_shapes_unseen_classes/
tags:
- 3D reconstruction
- NIPS
---

## Learning to Reconstruct Shapes from Unseen Classes

problem
- NN to approx. mapping from 2d -> 2.5d -> 3d may be overparametried
    - overfitting to training classes
- geometric projections generalize better

pipeline
- RGB -> depth map
- depth map -> partial spherical map
    - spherical map inpainting
    - proj. back to voxel space
- depth map -> 3d voxels (by projection)
- finetune two voxels
