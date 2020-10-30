---
title: Stochastic Gradient Hamiltonian Monte Carlo
date: 2019-10-22
categories:
- paper-reading
permalink: /posts/2019/10/22/paper_SGHMC/
tags:
- statistics
- ICLR
---


HMC
- requires full gradient
- how to introduce mini-batch?
    - correct using MH?
        - low acceptance rate or high computational time
    - introduce friction: second-order Langevin dynamics
- naive SGHMC
    - what's the effect of stochastic var.?
        - entropy increases!
    - introducing friction
    - simular to slides
