---
title: Object-Centric Neural Scene Rendering
date: 2021-02-03
permalink: /posts/2021/02/03/paper_ocnsr/
categories:
- paper-reading
tags:
  - arxiv
  - neural implicit field
---

object-centric neural scattering functions
- support for intra-object light transport
- each object as a 7-d function: pos + in + out -> opacity and color
  - model single light bounce, single light source, like appearance acquisition
- light do not intersect with objects are pruned