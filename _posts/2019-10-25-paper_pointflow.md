---
title: PointFlow 3D Point Cloud Generation with Continuous Normalizing Flows
date: 2019-10-25
categories:
- paper-reading
tags:
- 3D reconstruction
- 3D generation
- ICCV
---

## PointFlow 3D Point Cloud Generation with Continuous Normalizing Flows

point cloud as a sample
- to gen. a p.c. -> gen. a dist. of dist.
- model the dist. of points as transformation of 3D points from a prior distribution
    - VI framework
    - sample from prior then move them to posterior dist.
- continuous normalizing flows
    - well...Jacobians.
- a learnable prior
- loss
    - shape encoding -> prior
    - prob. of reconstruction: MC
    - entropy of posterior
