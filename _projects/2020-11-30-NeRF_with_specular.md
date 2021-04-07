---
title: 'Experiments on Neural Radiance Field'
date: 2020-11-30
permalink: /projects/2020/11/30/NeRF_experiments/
---

Below, I show some of my experiments on Neural Radiance Field(NeRF) during internship at ByteDance AILab.

### Introduction

Neural Radiance Field(NeRF) aims to learn a implicit scene representation from images and corresponding camera poses. Our main experiments on NeRF are
- add a reflection model to NeRF to model specularities, and
- exploit network capacity by train both coarse and fine network in an end-to-end way

#### Reflection Modeling

We observe that NeRF does not explicitly model reflection in the ray marching framework. However, interactions between objects are (implicitly) modeled by the view-dependent color, which will lead to some degenerate cases for specular scenes as the room scene below.

[image needed]

NeRF will learn a seperate world behind the monitor to model the reflection without anyknowledge of reflection. We added a reflection model(Karis' approximation of Microfacet model) with MC integration method into Neural Radiance Field. We assume a single ray bounce with depth and normal obtained from integrating and differentiating the network. Unfortunately, the results did not surpass the baseline, which we suspect the reasons are:
- explicit supervision of depth value are required, as done in [citation needed], or
- segmentation informations are also essential for efficient modeling of reflection, as done in [citation needed]

#### End-to-End Training of NeRF

We consider end-to-end training of NeRF, since in its coarse-fine sampling framework, the coarse network only serves as a (imperfect) depth regressor. We believe under some cases, the coarse network can "lend" some of its capacity to the fine one by end-to-end training.

##### Depth regression

A simple intuition to make NeRF end-to-end trainable is to replace the coarse network with a depth "oracle"(as in [citation needed]). We tried several attempts of regression/classification networks, whichever turns out to be not effective. We believe that direct depth supervision is necessary in this setting to help network figure out depth ambiguities.

##### Gaussian prior

The only thing that prohibits end-to-end training of NeRF is the sampling stage, where the opacity distribution CDF gets inverted. We observe that as training progresses, the distribution gets sharper and sharper and can be approximated by a Gaussian distribution. We have not yet achieved significant better performance against baseline under various conditions(hiddensize, sample size, number of layers, etc.)

##### Shared body/head

A step backwards from end-to-end training is to jointly train these two networks. An observation is that by concat coarse estimation of opacity and color with fine one, one can achieve slightly better results than baseline NeRF, and such performance gain is much more when network capacity is limited. From this observation, we tried to let both network share a rendering head, which is dedicated to render color and opacity from latent features of coarse/fine network. This does not yield better results, which may be from the fact that coarse and fine network has different input domain, and thus hard to align the output latent spaces.

A similar approach is to let networks share a feature extractor whose output is refined by coarse and fine head. This approach is under active experiment.