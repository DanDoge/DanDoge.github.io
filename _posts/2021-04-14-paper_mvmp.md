---
title: Multi-View Multi-Person 3D Pose Estimation with Place Sweep Stereo
date: 2021-04-14
permalink: /posts/2021/04/14/paper_mvmp/
categories:
- paper-reading
tags:
  - arxiv
  - pose estimation
---

image -> 2D poses
- mapping to different virtual planes, matched with reference view
  - a score matrix obtained: possibility of person at a single depth
  - weighted average with all reference views
- then estimate a joint-level relative depth (relative to person depth)