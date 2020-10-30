---
title: Learning to Generate Textures on 3D Meshes
date: 2019-10-03
categories:
- paper-reading
permalink: /posts/2019/10/03/paper_learn_to_gen_texture/
tags:
- texture synthesis
- CVPR
---

## Learning to Generate Textures on 3D Meshes

approach
- inputs: normalized object coordinates, masks, albedo
    - avalible from blender for me
- data: unpaired 2d/3d data
- from 2.5D information to multiview images, then generate texture using diff. renderer
    - first stage: cyclegan-style
    - seconds stage: L_2 + perception loss + consistancy loss

comparable result to novel view synthesis
- but only on one dataset: CompCar
- handle multiclass scenario?
- comparation to geometry method?
