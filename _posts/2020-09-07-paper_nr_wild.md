---
title: Neural Rerendering in the Wild
date: 2020-09-07
permalink: /posts/2020/09/07/paper_nr_wild/
categories:
- paper-reading
tags:
  - CVPR
  - neural rendering
---

scene under varying appearance
- render scene into deep buffer, render buffers(neural textures) to photos
- introducing appearance vector and semantic mask
  - seperate vp, appearance conditions and transient objects (auto decoder framework)
  - pretrain encoder for stable training, jointly finetune both networks