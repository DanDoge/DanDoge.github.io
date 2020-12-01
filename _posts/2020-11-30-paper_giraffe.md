---
title: GIRAFFE Representing Scenes as Compositional Generative Neural Feature Fields
date: 2020-11-30
permalink: /posts/2020/11/30/paper_giraffe/
categories:
- paper-reading
tags:
  - arxiv
  - neural rendering
  - neural implicit representation
---

conpositional nerf
- one for bg
  - only model several planes
- one for each obj
  - with rotation matrix generated
  - aabb intersection test
- render at lower res, then sr
  - that's... basically treating...