---
title: Making Convolutional Networks Shift-Invariant Again
date: 2020-09-29
permalink: /posts/2020/09/29/paper_MCNSIA/
categories:
- paper-reading
tags:
  - ICML
---

max pooling does not provide anti-aliasing capability
- from striding!!
- recall signal processing: blur before max-pooling
  - max pooling -> maxing and subsampling
  - solution: maxing and blurring and subsampling
  - accuracy and shift-equivariance improves at the same time
    - and rotation-equivariance