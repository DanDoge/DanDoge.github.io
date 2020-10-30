---
title: Gradient Descent Can Take Exponential Time to Escape Saddle Points
date: 2019-09-16
categories:
- paper-reading
permalink: /posts/2019/09/16/paper_GD_escape_saddle/
tags:
- learning theory
- NIPS
---

## Gradient Descent Can Take Exponential Time to Escape Saddle Points

time for theory papers! focus on works from Simon S. Du this time

for non-convex problem, GD can find a stationary point in poly. time
- stationary point? saddle points, local minimizer
- GD can escape saddle point
    - given that 1. local min. are global min. 2. saddle points are strict
    - hold for ML problems!2
    - incorporate perturbations: escape in poly. time
    - no perturbations: **proofed to be exp. time** <- this work

examples
- initialization within a thin band
- initialization far away from saddle point
- what about natural cases?
    - exists a function s.t. w.h.p. GD cannot visit second-order stationary point in T <= exp(omega(d))
    - excape 2 or more saddle points sequentially
