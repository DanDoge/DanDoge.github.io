---
title: Few-Shot Viewpoint Estimation
date: 2019-08-21
categories:
- paper-reading
permalink: /posts/2019/08/21/paper_fewshot_viewpoint_estimation/
tags:
- pose estimation
- ECCV
---


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
