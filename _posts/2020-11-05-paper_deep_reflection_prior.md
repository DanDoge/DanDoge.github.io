---
title: Deep Reflection Prior
date: 2020-11-05
permalink: /posts/2020/11/05/paper_deep_reflection_prior/
categories:
- paper-reading
tags:
  - arxiv
  - reflection modeling
---

single branch FCN
- assumption: background are the same
- I -> B + R
  - recons loss, cross recons loss, floor/ceiling rejection loss
    - how could such a loss work?
- latent code of B and R feed into network -> best preformance at first norm layer