---
title: NeRV Neural Reflectance and Visibility Fields for Relighting and View Synthesis
date: 2020-12-11
permalink: /posts/2020/12/11/paper_nerv/
categories:
- paper-reading
tags:
  - arxiv
  - neural implicit representation
  - 3D reconstruction
---

novel view and novel lighting
- reduce computation for one-bounce and direct lighting
  - by using a neural visibility field
  - one-bounce expanison of the rendering equation
  - enforce the visibility field to resemble the current state of shape MLP