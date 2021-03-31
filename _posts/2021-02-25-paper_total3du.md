---
title: Total3DUnderstanding Joint Layout, Object Pose and Mesh Reconstruction for Indoor Scenes form a single Image
date: 2021-02-25
permalink: /posts/2021/02/25/paper_total3du/
categories:
- paper-reading
tags:
  - arxiv
  - 3D reconstruction
---

reconstruct layout, object bbox and meshes
- image -> 2dbbox -> 3d mesh / 3d bbox -> layout
  - image -> feature, then deform a template sphere
  - remove a face by local density
  - relative feature compared to local neighbors