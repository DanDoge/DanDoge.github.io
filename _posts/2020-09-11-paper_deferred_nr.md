---
title: Deferred Neural Rendering Image Synthesis using Neural Textures
date: 2020-09-11
permalink: /posts/2020/09/11/paper_deferred_nr/
categories:
- paper-reading
tags:
  - siggraph
  - neural rendering
---

neural textures as maps on top of 3D mesh proxies
- assumptions: captures 3D scenes are always corrupted in some way
  - combine neural texture and traditional graphic pipeline
- end-to-end training to find a renderer and texture map
- under sampling and over sampling
  - inspired by mipmap, introducing a hierarchical rendering strategy