---
title: DEEP DOUBLE DESCENT WHERE BIGGER MODELS AND MORE DATA HURT
date: 2019-12-23
categories:
- paper-reading
tags:
- learning theory
- blogpost
---

traditional statistical learning: larger model -> higher variance
- modern ML: larger model are better
- contradiction!

emperical evidence
- in under-parameterized regime: U-like test error
- over-parameterized regime: bigger models are better
- effective model complexity: max. \# of samples can achieve zero training error
- double descent occurs as a function of EMC
    - test error peaks around where EMC matches the number of samples: only one model(set of params.) that fits all training data, whereas larger model can ensemble multiple models/params.
    - model/epoch/sample-wise double descent
    - large models can undergo double descent and then decreases again, but intermediate model gets stucked
