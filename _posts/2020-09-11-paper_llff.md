---
title: Local Light Field Fusion Practical View Synthesis with Prescriptive Sampling Guidelines
date: 2020-09-11
permalink: /posts/2020/09/11/paper_llff/
categories:
- paper-reading
tags:
  - siggraph
  - neural rendering
---

local light field with a multiplane image representation
- skip sampling part... do not get it... I really need to take a signal processing course
  - number of input views reqired decreases with number of planes
- view -> layered scene representation, blending between neighboring scene representations
  - input: 5 views: a reference view and 4 neighbors, CNN outputs a opacity and selection weights