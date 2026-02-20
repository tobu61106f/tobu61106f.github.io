---
layout: archive
title: "Project"
permalink: /project/
author_profile: true
redirect_from:
  - /research
---

# Scientific Machine Learning/Machine Learning for Science (AI4Science)
## Convex Importance-Weight Optimization for Diffusion Model Training Timesteps
**Convex Optimization Course Project**, Author: *Ziqing Chang*, *Zhiyun Yu*

**The Problem:** Standard DDPM training typically employs uniform weights \\(w_t = 1/T\\) or cosine weights. However, these approaches fail to account for the fact that different timesteps \\(t\\) exhibit varying loss magnitudes and variances. To address this, we introduce a convex formulation to find the optimal weights, \\(w^*\\), by solving a strictly convex quadratic program (QP):

$$
F_{\lambda}(w) = \sum_{t=1}^{T} w_t \hat{l}_t + \lambda \sum_{t=1}^{T} w_t^2 \sigma_t^2
$$

First, we train a baseline model on the MNIST dataset to collect empirical data for the expected loss \\(\hat{l}_t\\) and variance \\(\sigma_t^2\\) at each timestep. Next, we apply the Karush-Kuhn-Tucker (KKT) conditions to derive a closed-form solution for \\(w^*\\) within the primal model. We evaluate and compare the baseline model against our optimized model. We show that the KKT-derived \\(w^*\\) effectively minimizes the surrogate objective \\(F_\lambda(w)\\), which in practice translates into improved optimization behavior during training.

# IC Design


