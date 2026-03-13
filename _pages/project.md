---
layout: archive
title: "Project"
permalink: /project/
author_profile: true
redirect_from:
  - /research
---

# Machine Learning

[**EE441/541: Convex Optimization with Applications in Communication and Machine Learning**](https://mingshihomepage.com/studentsandteaching.html)

Department of Electrical Engineering, University at Buffalo, Fall 2025.

Author: *Ziqing Chang*, *Zhiyun Yu*

**Title**: Convex Importance-Weight Optimization for Diffusion Training Timesteps.

Me and my Partner Ziqing remodified this specific Diffusion Model based on two NeurIPS paper:

[*Denoising Diffusion Probabilistic Models, Jonathan Ho and Ajay Jain and Pieter Abbeel, NeurIPS2020*](https://hojonathanho.github.io/diffusion/)
[*Generative modeling by Estimating Gradients of the Data Distribution, Yang Song, Stefano Ermon, NeurIPS2019*](https://arxiv.org/abs/1907.05600)


**The Problem:** Standard DDPM training typically employs uniform weights \\(w_t = 1/T\\) or cosine weights. However, these approaches fail to account for the fact that different timesteps \\(t\\) exhibit varying loss magnitudes and variances. To address this, we introduce a convex formulation to find the optimal weights, \\(w^*\\), by solving a strictly convex quadratic program (QP):

$$
F_{\lambda}(w) = \sum_{t=1}^{T} w_t \hat{l}_t + \lambda \sum_{t=1}^{T} w_t^2 \sigma_t^2
$$


First, we train a baseline model on the MNIST dataset to collect empirical data for the expected loss $\hat{l}t$ and variance sigma_t^2 at each timestep. Next, we apply the Karush-Kuhn-Tucker (KKT) conditions to derive a closed-form solution for \\(w^*\\) within the primal model. We evaluate and compare the baseline model against our optimized model. We show that the KKT-derived $w^*$ effectively minimizes the surrogate objective $F{\lambda}(w)$, which in practice translates into improved optimization behavior during training.

# IC Design




# Power Systems Optimization
