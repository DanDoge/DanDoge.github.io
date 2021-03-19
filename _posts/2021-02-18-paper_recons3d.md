---
title: Reconstructing 3D Human Pose from 2D Image Landmarks
date: 2021-02-18
permalink: /posts/2021/02/18/paper_recons3d/
categories:
- paper-reading
tags:
  - arxiv
  - pose estimation
---

a quite traditional approach to pose estimation
- mean pose + some main directions(from PCA)
- pose estimation -> estimation coeficient under above pose basis
  - conditioned on limb length (relaxation: sum of limb length squared should be equal)
  - coordinate descent