---
title: ODE^2VAE Deep generative second order ODEs with Bayesian neural networks
date: 2019-10-26
categories:
- paper-reading
tags:
- bayesian neural networks
- NIPS
---

## ODE^2VAE Deep generative second order ODEs with Bayesian neural networks

VAE
- data associated with a single latent code
    - what about sequential data?
- latent space governed by a continuous-time ODE
- first order ODE
    - got it!
    - derivative parametrised as a NN
    - cannot modlelling high-order dynamics
- second-order ODE
    - similar to HMC...
- model
    - position encoder
    - velocity encoder
    - simulate dynamics
    - decoder
- loss
    - regularization: KL
    - VAE loss: loss for x_0
    - dynamic loss
