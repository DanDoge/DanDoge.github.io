---
title: Local Deep Implicit Functions for 3D Shape
date: 2020-08-31
permalink: /posts/2020/08/31/paper_local_deep_implicit_functions/
categories:
- paper-reading
tags:
  - CVPR
  - 3D reconstruction
  - neural impliclt field
---

one neural field -> mixture of multiple neural fields
- more like a conditioned image generation than really learn a neural field
  - and that is (probably) why it uses much less params -> elegant design
  - trasform to local space: learn a easy function?
- weighted by oriented Gaussian