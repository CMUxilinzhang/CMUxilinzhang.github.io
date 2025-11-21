---
title: "DiffTORI with Adaptive Horizon and Hybrid Dynamics"
excerpt: >
  Improving DiffTORI with adaptive planning horizons, residual MLP models, and variational latent regularization.<br/>
#   <img src="/images/difftori.png">
collection: portfolio
---


## Introduction  
DiffTORI combines differentiable trajectory optimization with model-based RL, but struggles with unstable gradients, fixed horizons, and shallow latent models. Improving these limitations has direct impact on **robust robot learning**, especially in long-horizon or contact-rich tasks.  
**Objective:** enhance DiffTORI’s stability, sample efficiency, and convergence through architectural and algorithmic improvements.

## Methods  
Based on the implementation (:contentReference[oaicite:3]{index=3}), we introduced:
- **Gradient- and loss-driven adaptive horizons** that expand or shrink the planning window.  
- **Cost-to-go horizon selection** using Theseus-based optimization.  
- **Residual MLP blocks** to improve latent dynamics expressiveness.  
- **Variational latent-space regularization** for smoother latent manifolds.

## Results  
- Adaptive horizons improved convergence stability in continuous tasks like *walker-run*.  
- Residual MLPs improved long-horizon planning smoothness.  
- Variational regularization reduced latent collapse but degraded task reward due to precision loss.  
- Fixed-horizon DiffTORI still outperformed adaptive methods in sparse-reward tasks.

## Discussion  
Findings show a trade-off between model expressiveness and stability. Sparse reward settings remain challenging for horizon adaptation, while dense-reward environments benefit significantly. This suggests future work toward warm-starting and smoothing horizon transitions.

## My Contribution  
I implemented adaptive-horizon rules, performed experiments on Meta-World and DiffTORI benchmarks, analyzed failure modes, and contributed to the full report structure.  
