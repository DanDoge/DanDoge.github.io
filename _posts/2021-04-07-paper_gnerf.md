---
title: GNeRF Gan-based Neural Radiance Field without Posed Camera
date: 2021-04-07
permalink: /posts/2021/04/07/paper_gnerf/
categories:
- paper-reading
tags:
  - arxiv
  - 3D reconstruction
  - neural rendering
  - neural implicit field
---

learn a set of pose embedding, assign to input un-posed images
- pose -> NeRF -> images -> discriminator -> T/F / encoder -> pose
  - for GT images, only pose embeddings are trained/maintained
- then, jointly update NeRF and pose embedding as in NeRF--