---
title: Disentangling Disentanglement in Variational Autoencoders
date: 2019-11-22
categories:
- paper-reading
permalink: /posts/2019/11/22/paper_distentangle_in_VAE/
tags:
- disentangle learning
- VAE
- ICML
---

well, time for reading papers!

from disentanglement to decomposition
- the former being explicit independence between latents
- while decomposition being more general
    - latent coding have appropriate level of overlap
    - encoding close to prior
- formal evaluation metrics/datasets
    - may be harmful/not generalisable
    - cannot mimic the generation of real data
- deconstruction of beta-vae
    - VAE + regulariser encouraging encoder variance
    - rotation invariant: not enough to encourage meaningful representations
- use of synthetic data?
    - still not real world data
    - happens to be independent by construction of datasets
- number of latent dimentions
    - less than true generative factors
    - true generative factors are not independent
- prior as a powerful means for expressing desired sturcture
- beta-VAE
    - enforcing a max. ent. on posterior
    - still independent w.r.t. rotation of z
        - strong coorelation between latents
    - standard VAE up to a scaling
