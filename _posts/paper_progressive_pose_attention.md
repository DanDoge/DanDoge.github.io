---
title: Progressive Pose Attention Transfer for Person Image Generation
date: 2019-12-23
categories:
- paper-reading
tags:
- novel view synthesis
- image synthesis
- CVPR
---

pose transfer
- condition image + target pose
    - pose: heat maps
- images of all possible poses constitute a manifold
    - which structure is simple at local level but hard to transfer at global level
    - progressive transfer: a sequence of intermediate pose representations
        - attention mechanism: where to sample from and where to put patches
        - heat map of where to sample
        - concatenate new pose to the older one(subsampled)
- plus perceptual L1 loss
