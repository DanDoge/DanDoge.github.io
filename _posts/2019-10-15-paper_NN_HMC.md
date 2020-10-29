---
title: GENERALIZING HAMILTONIAN MONTE CARLO WITH NEURAL NETWORKS
date: 2019-10-15
categories:
- paper-reading
tags:
- statistics
---

## GENERALIZING HAMILTONIAN MONTE CARLO WITH NEURAL NETWORKS

HMC
- struggle to mix energy levels
- cannot easily traverse low-density zones
- slow mixing in some cases

introcude
- translation, rescale of gradient and rescale of mementum
- all implemented by multi layer perceptrons
- loss: max lag-one distance
    - on both target and prior dist.
