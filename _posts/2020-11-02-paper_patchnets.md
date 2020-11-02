---
title: PatchNets Patch-Based Generalizable Deep Implicit 3D Shape Representations
date: 2020-11-02
permalink: /posts/2020/11/02/paper_patchnets/
categories:
- paper-reading
tags:
  - arxiv
  - 3D reconstruction
  - neural implicit field
---

mid-level patch-based surface representation
- 3D model being a collection of patches
- estimate patch extrinsics
  - latent optimazation
  - each patch being a signed-distance function: truncated to 0.1
  - while the number of patch being fixed
- then blend to a 3D model
  - weight: gaussian kernel - constant, s.t. weight = 0 at the boundry