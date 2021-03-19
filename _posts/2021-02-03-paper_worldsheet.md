---
title: Worldsheet Wrapping the World in a 3D Sheet for View Synthesis from a Single Image
date: 2021-02-03
permalink: /posts/2021/02/03/paper_worldsheet/
categories:
- paper-reading
tags:
  - arxiv
  - novel view synthesis
---

shrink-warpping a planar mesh sheet with learned depth
- trained via differentiable rendering
- image -> depth -> grid offset -> mesh -> mesh with texture by differentiable sampling from input view -> novel view
- L2 regularization of grid offsets