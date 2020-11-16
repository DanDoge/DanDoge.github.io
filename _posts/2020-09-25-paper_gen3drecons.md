---
title: On the generalization of learning-based 3D reconstruction
date: 2020-09-25
permalink: /posts/2020/09/25/paper_gen3drecons/
categories:
- paper-reading
tags:
  - arxiv
  - 3D reconstruction
---

learn a scalar field
- xyz -> occupancy, conditioned on input view
- image -> feature -> alignment loss
  - camera pose given
- um, since camera poses are given, there must exist a more elegant way of incorporating information across different views, like, even geometry based ones would work, instead of relying heavily on the representation capacity of neural nets