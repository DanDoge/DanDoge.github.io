---
title: VoxelPose Towards Multi-Camera 3D Human Pose Estimation in Wild Environment
date: 2021-02-25
permalink: /posts/2021/02/25/paper_voxelpose/
categories:
- paper-reading
tags:
  - arxiv
  - neural rendering
  - pose estimation
---

image -> 2D feature -> 3D feature -> pose estimation
- discretized 3D space -> cuboid proposals
  - supervised by a Gaussian filtered score
  - similar to object detection, but in 3D
- fine-grained feature volume at each proposal
  - global softargmax to get a finer pose