---
title: Occupancy Flow 4D Reconstruction by Learning Particle Dynamics
date: 2020-11-30
permalink: /posts/2020/11/30/paper_occupancy_flow/
categories:
- paper-reading
tags:
  - arxiv
  - neural implicit representation
  - neural rendering
---

a velocity field: warp f(xyz, t) -> f(xyz, 0), similar to solve a ODE
- then a occupancy network for time 0
- conditional batch norm <- condition on image