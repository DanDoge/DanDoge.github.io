---
title: Momentum Contrast for Unsupervised Visual Representation Learning
date: 2020-11-13
permalink: /posts/2020/11/13/paper_moco/
categories:
- paper-reading
tags:
  - CVPR
---

contrastive learning
- from a dictionary point of view
- maintain a dictrionary of keys, then matching the current query to elements in the queue
  - degenerating results
- seperate encoder for key and queries
  - gradient update query encoder
  - key encoder: average of key and query -> mometum