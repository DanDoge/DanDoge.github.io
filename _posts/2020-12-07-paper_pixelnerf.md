---
title: pixelNeRF Neural Radiance Fields from One or Few Images
date: 2020-12-07
permalink: /posts/2020/12/07/paper_pixelnerf/
categories:
- paper-reading
tags:
  - arxiv
  - neural implicit representation
  - image synthesis
  - 3D reconstruction
---

nerf for fewshot novel view synthesis
- conditioned on image feature -> mapped to 3d world -> collected from query viewpoint
- multiple views: avg pooling in the last fc layer