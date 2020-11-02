---
title: Occupancy Networks Learning 3D Reconstruction in Function Space
date: 2019-10-25
categories:
- paper-reading
permalink: /posts/2019/10/25/paper_occupancy_networks/
tags:
- 3D reconstruction
- neural implicit field
- CVPR
---


3D output representation
- both memory efficient and efficiently inferred from data
- voxel: memory hungry
    - even using octrees: 256^3
- point clouds: need additional processing steps
- mesh: hard t oinferred by feed-forward network
- Occupancy Networks
    - field similar to texture field
    - loss: cross-entropy
    - MISE: incrementally building an octree
    - refine using gradient information: gradient toward GT normal
- experiment: similar to texture field
