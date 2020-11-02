---
title: RotationNet Joint Object Categorization and Pose Estimation Using Multiviews from Unsupervised Viewpoints
date: 2020-02-24
categories:
- paper-reading
permalink: /posts/2020/02/24/paper_rotationnet/
tags:
- CVPR
- 3D categorization
- pose estimation
---

method: treat veiwpoint as latent variables, learned unsupervised
- similar to frcnn, outputs prob of each category in each viewpoint, with a i_view stands for incorrect view
    - max. the prob. of each vp being the output vp and class label being target label -> EM!
        - determine vp: max. prob. of vp_i == v and vp_{j != i} = i_view
        - update params: max. log p., cross entropy optim.
