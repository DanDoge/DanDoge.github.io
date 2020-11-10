---
title: State of the Art on Neural Rendering
date: 2020-09-07
permalink: /posts/2020/09/07/paper_sota_neural_rendering/
categories:
- paper-reading
tags:
  - EG
  - neural rendering
---

where and how rendering pipelines can be improved by ml
- BRDF / BSSRDF
- ray tracing in implicit representations
  - a few bounces of light would be enough
- IBR fails: few observations given or view-dependent effects or not covered parts
  - learning priors
- learn to relight
  - extract reflectance field, then combine them