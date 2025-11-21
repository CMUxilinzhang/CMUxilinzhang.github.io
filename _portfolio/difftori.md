---
title: "DiffTORI with Adaptive Horizon & Hybrid Dynamics"
excerpt: "Extensions to differentiable trajectory optimization for robot learning."
collection: portfolio
---


This project extends DiffTORI, a differentiable trajectory optimization method for reinforcement learning, by incorporating adaptive horizons, hybrid residual dynamics, and variational latent regularization.  
The social value lies in improving **stability, efficiency, and long-horizon performance** in real-world robot learning.

## Objective
Enhance the task performance and training robustness of DiffTORI by addressing limitations in:
- fixed-horizon optimization  
- shallow latent models  
- deterministic latent encodings  

## Method

### 1. Adaptive Horizon Optimization  
We propose a horizon-selection rule based on gradient consistency and multistep cost-to-go analysis.  
This mechanism integrates directly into Theseus (a differentiable optimization library).

### 2. Residual MLP Dynamics  
We incorporate:
- physical prior dynamics  
- residual MLP corrections  
- LayerNorm + residual blocks for stability  

This hybrid model improves prediction accuracy and smoothness.

### 3. Variational Latent Regularization  
A VAE-style encoder with KL annealing encourages smoother latent transitions and improved generalization.

## Results
- Adaptive horizons improved convergence in dense-reward tasks.  
- Residual MLP dynamics provided smoother trajectories and better policy stability.  
- Variational latent modeling exposed a trade-off between smoothness and precision.  

<!-- ## My Role
I implemented:
- adaptive horizon mechanisms  
- residual MLP architectures  
- KL-annealed latent regularization  
- experiments, tuning, and final report analysis   -->
