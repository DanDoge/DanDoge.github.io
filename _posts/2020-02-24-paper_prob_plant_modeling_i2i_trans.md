---
title: Probabilistic Plant Modeling via Multi-View Image-to-Image Translation
date: 2020-02-24
categories:
- paper-reading
permalink: /posts/2019/02/24/paper_prob_plant_modeling_i2i_trans/
tags:
- CVPR
- 3D reconstruction
- image synthesis
---

task: infer 3D branch structures from multi-view observations
- infer prob. of branch using Bayesian i2i, then generates a prob. plant 3D model
    - why prob? access to credibility of estimates, consolidate view dependent inferences
- previous methods
    - branching model of trees: low deviation from presumed models
    - BNN: in this work, MC via dropout
- method
    - Pix2Pix, with dropout layer inserted
    - take the mean of stochastic samples as estimation of 2D prob of being a branch, multipliing into 3D prob.
    - branch generation using particle flows
        - generates particles propto log prob. of 3D prob, with root set to bottonmost point
        - particle pos. updated by three forces
            - F_root
            - F_c: toward to branch prob.
            - F_d: parallel to branch prob.
        - unification of particles
    - smoothing, refinement, simplification
