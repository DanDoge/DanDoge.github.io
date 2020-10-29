---
title: Bayesian Learning via Stochastic Gradient Langevin Dynamics
date: 2019-10-21
categories:
- paper-reading
tags:
- statistics
- ICLR
---

## Bayesian Learning via Stochastic Gradient Langevin Dynamics

motivation
- emerge of large-scale datasets
- success of SGD
- left-behind: Bayesian methods
    - MCMC: requires whole dataset, time!

SGD methods
- var. in gardient cancelled out in the whole dataset
- step sizes: able to travel far and stay at stable point

Langevin dynamics
- insert gaussian noise in gard.
- matched step size and noise
- can be corrected using MH
    - as epsilon -> zero, no need to correct

this work
- change the gradient in Langevin dynamics to estimation by mini-batch
- injected noise after all dominated stochastic noise
- and will converge
- step size must goes to zero
    - or switch to a diff. algo. later
- adjust noise cov. to control var. of grad.
- est. by weighted sum.(weighted by step sizes)
