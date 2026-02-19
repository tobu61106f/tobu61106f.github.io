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
**Convex Optimization Course Project, Author: *Ziqing Chang*, *Zhiyun Yu*
The Problem: 
Standard DDPM training uses "uniform" weights 𝑤_𝑡=1\/𝑇 or ”cosine" weights , which ignores that different timesteps 𝑡 have different loss magnitudes and variances.
Our Method: 
The Convex Formulation (P) We find the optimal weights 𝑤^∗ by solving a strictly convex quadratic program (QP): 
min┬(𝑤∈Δ^𝑇 )⁡  𝐹(𝑤)=⏟(∑_(𝑡=1)^𝑇▒〖𝑤_𝑡 (𝑙_𝑡 ) ̂ 〗)┬"Weighted Loss" +𝜆 ⏟(∑_(𝑡=1)^𝑇▒〖𝑤_𝑡^2 𝜎_𝑡^2 〗)┬"Weighted Variance" 
We tranning the Baseline Model to collect empirical data (𝑙_t ) ̂𝑎𝑛𝑑 𝜎_𝑡^2 on the MNIST Set, later we will use KKT conditions to find the closed-form solution on primal model for 𝑤^∗



---
# IC Design

---

