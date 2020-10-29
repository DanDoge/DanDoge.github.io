---
title: Few-Shot Viewpoint Estimation
date: 2019-08-21
categories:
- paper-reading
tags:
- pose estimation
- ECCV
---

## Few-Shot Viewpoint Estimation

two RexNet style networks for
- general keypoints
- 8 category specific semantic keypoints

then
- category specific viewpoint estimation block
- apply meta-learning
- estimate keypoints location, then solve equations for viewpoint

training
- MAML: min generalization loss each time
- keypoints' 2d, 3d, depth location loss
- meta-siamese: nothing but an initializer?
