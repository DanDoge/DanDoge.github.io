---
title: Single Image Reflection Separation with Perceptual Losses
date: 2020-11-04
permalink: /posts/2020/11/04/paper_reflection_seperation_perceptual/
categories:
- paper-reading
tags:
  - CVPR
  - reflection modeling
---

image = bg + reflection
- where the bg part should be consistant with image at feature level
- and all edges should belong to **either** bg or reflection but not both
  - introducing exclusion loss in gradient domain
- plus a adv loss