---
title: Understanding Deep Image Representations by Inverting Them
date: 2020-11-04
permalink: /posts/2020/11/04/paper_understanding_representations/
categories:
- paper-reading
tags:
  - arxiv
---

understanding representations by training another network
- s.t. reconstruct image from such a representation
  - which is against the belief that deep representations represents for high level features
  - and thus not invertable
  - but, natural image should contain less high frequency noise, it may be possible to invert in natural image domain
  - natural image prior: min. total variation