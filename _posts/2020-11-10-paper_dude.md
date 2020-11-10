---
title: DUDE Deep Unsigned Distance Embeddings for Hi-Fidelity Representation of Complex 3D Surfaces
date: 2020-11-10
permalink: /posts/2020/11/10/paper_dude/
categories:
- paper-reading
tags:
  - arxiv
  - 3D reconstruction
---

reconstruct 3D model using a **unsigned** distance function and a vector field
- both supervised
- since udf is not differentiable, approx. the "true surface" using normal estimation as a guide: local planary assumption
- min normal l2 loss *up to module 180*
  - loss being min of |a - b| and |a - (-b)|
- udf to meshees
  - subdivision, then marching cubes