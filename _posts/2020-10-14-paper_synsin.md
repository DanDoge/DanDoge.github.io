---
title: SynSin End-to-end View Synthesis from a Single Image
date: 2020-10-14
permalink: /posts/2020/10/14/paper_synsin/
categories:
- paper-reading
tags:
  - CVPR
  - 3D reconstruction
  - novel view synthesis
---

a hs pc of learned features
- trained using image pairs and camera poses
- image -> feature and depth map -> lift to 3d -> project to novel view -> image
- biggan... not doable for me 
- soft z-buffer and a disk of influence for each point
  - alpha compositing