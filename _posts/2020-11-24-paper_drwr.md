---
title: DRWR A Differentiable Renderer without Rendering for Unsupervised 3D Structure Learning from Silhouette Images
date: 2020-11-24
permalink: /posts/2020/11/24/paper_drwr/
categories:
- paper-reading
tags:
  - ICML
  - 3D reconstruction
---

supervision only from silouette image
- intuition: points should be inside and fill the silouette
  - two losses: a smooth binary loss(avoid local minima) and a pairwise loss
