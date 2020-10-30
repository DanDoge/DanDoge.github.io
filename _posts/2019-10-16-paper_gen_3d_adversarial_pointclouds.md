---
title: Generating 3D Adversarial Point Clouds
date: 2019-10-16
categories:
- paper-reading
permalink: /posts/2019/10/16/paper_gen_3d_adversarial_pointclouds/
tags:
- 3D generation
- adversarial learning
- CVPR
---


challenging to gen. adv. data on point clouds
- no value to tune
- search space being quite large
- L_p norm not apply to point cloud data

targeted adv. attack
- min D(x, x') s.t. F(x') = t' ==> difficult!
- min f(x') + wD(x, x')
    - where f(x') = (max(Z(x')[i]) - Z(x')[t'])
    - diff of logits of other labels from target label
- adv. point perturbation and adv. point gen.(new)
    - initialize to some existing points
    - and shift it while optimizing
- adv. cluster gen.
    - small radius and close to surface

measure of point addition
- Hausdorff distance
- Chamfer
- # of points added

...and defence
- PointNet more robust than tradition CNN on MNIST
