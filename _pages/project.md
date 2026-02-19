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

The Problem: 
Standard DDPM training uses "uniform" weights 𝑤_𝑡=1\/𝑇 or ”cosine" weights , which ignores that different timesteps 𝑡 have different loss magnitudes and variances.

Our Method: 
The Convex Formulation (P) We find the optimal weights 𝑤^∗ by solving a strictly convex quadratic program (QP): 
\[
\min_{w \in \Delta^T} F(w)
= \sum_{t=1}^{T} w_t \hat{l}_t
+ \lambda \sum_{t=1}^{T} w_t^2 \sigma_t^2
\]
We tranning the Baseline Model to collect empirical data (𝑙_t ) ̂𝑎𝑛𝑑 𝜎_𝑡^2 on the MNIST Set, later we will use KKT conditions to find the closed-form solution on primal model for 𝑤^∗. In final stage we evaluated and compared Model_Baseline and Model_Optimal, the KKT-derived w* minimizes the surrogate objective Fλ(w), and in practice this translates into better optimization behavior during training.


---
# IC Design

---

