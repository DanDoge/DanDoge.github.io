---
title: Novel View Synthesis from only a 6-DoF Camera Pose by Two-stage Networks
date: 2020-11-02
permalink: /posts/2020/11/02/paper_nvs_from_camerapose/
categories:
- paper-reading
tags:
  - arxiv
  - neural rendering
  - novel view synthesis
---

extreme simple idea
- pose -> coarse image(conditioned on training image embedding) : L1loss
- refine image : L1, perceptual, adversarial