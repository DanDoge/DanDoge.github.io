---
title: FUNCTION CONTRASTIVE LEARNING OF TRANSFERABLE REPRESENTATIONS
date: 2020-11-02
permalink: /posts/2020/11/02/paper_function_contrasive/
categories:
- paper-reading
tags:
  - arxiv
  - few shot learning
---

idea: two set of examples from same function should share similar latent representations, while from different functions shoule be easily distinguishable
- find an encoder that maps such partial observations to low-dim. representations
- encoder: pointwise transformation(MLP) -> average pooling
  - training: cosine similarity measure with temperature