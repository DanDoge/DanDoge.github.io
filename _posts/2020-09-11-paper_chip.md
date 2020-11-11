---
title: Seeing the World in a Bag of Chips
date: 2020-09-11
permalink: /posts/2020/09/11/paper_chip/
categories:
- paper-reading
tags:
  - CVPR
  - neural rendering
  - reflection modeling
---

nvs and **environment reconstruction**
- reconstruct specular reflectance maps: environment map convolve with BRDF
  - given RGB**D** video: geometry given!!!
- diffuse color using previous methods: approx. min of all values
  - refined using CNN
- predefine some number of basis textures
  - each point is a mixture of different textures
  - each texture has a specific environment map(BRDF conv true envirionment map)
- consider fresnel effect and interreflection
  - only by feeding fresnel coef. and reflection color into a CNN