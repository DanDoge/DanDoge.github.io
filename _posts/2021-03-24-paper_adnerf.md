---
title: iMAP Implicit Mapping and Positioning in Real-Time
date: 2021-03-25
permalink: /posts/2021/03/25/paper_imap/
categories:
- paper-reading
tags:
  - arxiv
  - neural rendering
---

SLAM as an incremental learning problem
- add new frames as keyframe only if they see new regions(> than 0.35)
- sample points for rendering proportional to depth distribution
  - retain key frames with highest loss to prevent size of keyframes grow too large