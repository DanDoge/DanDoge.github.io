---
title: A mininal review on outdoor 3D reconstruction
date: 2019-10-12
categories:
- paper-reading
permalink: /posts/2019/10/12/paper_SLAM_series/
tags:
- 3D reconstruction
---


I am gonna review some paper on 3D reconstruction, both to
- know some critical technics for FYP, and
- find out the answer to the question in the inverview

### Large-Scale Multi-Resolution Surface Reconstruction from RGB-D Sequences

ICCV 13

octtree, surface as a signed distance function

error in pose graph construction: error defined on images and depth informations
- error ~ t-dist.

keyframe
- entropy introduced
    - also used for loop closures

### Dense Visual SLAM for RGB-D Cameras

IROS 13

min geometric error
- ICP
- prone to drift if only odometry constraint considered
- similar to above...really?
    - and same author...what?
- also t-dist.

### Unsupervised Learning of Threshold for Geometric Verification in Visual-Based Loop-Closure

ICRA 14

two log-Gaussian model for T/F positive loop-closures
- has emperical clue for this

### Robust Reconstruction of Indoor Scenes

CVPR 15

a weight for each loop-clousures
- with prior/regulization: more loop-closures are better
