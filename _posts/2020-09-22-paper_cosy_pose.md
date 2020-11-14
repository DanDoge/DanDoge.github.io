---
title: CosyPose Consistent multi-view multi-object 6D pose estimation
date: 2020-09-22
permalink: /posts/2020/09/22/paper_cosy_pose/
categories:
- paper-reading
tags:
  - ECCV
  - pose estimation
---

estimate camera views and 6D poses of all objs
- explicitly handles symmetries, no depth requirements
- render-and-compare
- RANSAC -> refer to wikipedia
- assumption: obj of interest are known, with some of them not visible, unposed images
  - output: scene model, # of objs, poses, camera poses
  - object detection and pose estimation
  - loss: up to a symmetry