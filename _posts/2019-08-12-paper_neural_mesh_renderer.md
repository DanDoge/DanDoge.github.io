---
title: 'Neural 3D Mesh Renderer'
date: 2019-08-12
categories:
- paper-reading
permalink: posts/2019/08/12/paper_neural_mesh_renderer/
tags:
- neural rendering
- CVPR
---


problem: rendering 3d model is not differentiable
- ...until now, this paper proposes an approximate gradient for rendering

repersentation of 3d models
- voxels: low resolution
- point clouds: not scalable, cannot apply texture and lighting

rasterization: sampling a pixel's color same as the corresponding facet' color
- instead of defining color as square wave, replace it with linear functions

regularization: interection angles of facets close to 180 degrees

applications: style transfer, reconstruction, etc.
