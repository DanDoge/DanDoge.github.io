---
title: Neural Scene Graphs for Dynamic Scenes
date: 2020-11-24
permalink: /posts/2020/11/24/paper_nsgd/
categories:
- paper-reading
tags:
  - arxiv
  - 3D reconstruction
  - neural rendering
---

radiance field for dynamic scene
- scene graph: seems to be from dataset, not learned
  - obj position, bbox
- a nerf for a single object
- convertion between world coord and obj coord
  - but still feed some feature from global coord -> count for global illumination?
- a nerf for bg
  - assume bg consists of several planes: which planes?