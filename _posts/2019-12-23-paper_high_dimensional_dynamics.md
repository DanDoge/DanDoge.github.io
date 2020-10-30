---
title: High-dimensional dynamics of generalization error in neural networks
date: 2019-12-23
categories:
- paper-reading
permalink: /posts/2019/12/23/paper_high_dimentional_dynamics/
tags:
- statistics
- learning theory
---

generalization dynamics of large NN trained by GD
- GD naturally protect against overtraining and overfitting
    - more data decreases impact of weights initialization
- low genrgalization error requires small initial weights
- a frozen space where no learning occurs
    - directions with zero eigenvalues
    - low eigenvalues lead to serious overfitting
        - early stop can be effective, since its slow to learn
    - a large eigengap can protect against overfitting

L2 regularization performs best under Gaussian noise assumptions

experiments
- teacher NN generates ramdom labels for student NN to learn
- catastrophic overtraining when model complexity matches the size of training set
    - larger NNs are better
- NN with wide hidden layer can be expressive
    - even with first layers fixed
    - random CNNs can also achieve good results
- contradict VC dim or Rademacher bounds
    - effective complexity constrained by initialization of NN -> low Rademacher complexity even with more neurals
- GD trained NN learns a simpler function first
