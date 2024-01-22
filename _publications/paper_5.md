---
title: "(ICLR 2024 **spotlight**) How Over-Parameterization Slows Down Gradient Descent in Matrix Sensing: The Curses of Symmetry and Initialization"
collection: publications
permalink: /publication/paper_5
excerpt: '*Nuoya Xiong*, Lijun Ding, Simon S. Du'
date: 2024-01-16
venue: 'International Conference on Learning Representations'
paperurl: ' '
citation: ' '
---
This paper rigorously shows how over-parameterization dramatically changes the convergence behaviors of gradient descent (GD) for the matrix sensing problem, where the goal is to recover an unknown low-rank ground-truth matrix from near-isotropic linear measurements.
First, we consider the symmetric setting with the symmetric parameterization where $M^* \in \mathbb{R}^{n \times n}$ is a positive semi-definite unknown matrix of rank $r \ll n$, and one uses a symmetric parameterization $XX^\top$ to learn $M^\*$. Here $X \in \mathbb{R}^{n \times k}$ with $k > r$ is the factor matrix.
We give a novel $\Omega\left(1/T^2\right)$ lower bound of randomly initialized GD for the over-parameterized case ($k >r$) where $T$ is the number of iterations.
This is in stark contrast to the exact-parameterization scenario ($k=r$) where the convergence rate is $\exp\left(-\Omega\left(T\right)\right)$.
Next, we study asymmetric setting where $M^* \in \mathbb{R}^{n_1 \times n_2}$ is the unknown matrix of rank $r \ll \min\{n_1,n_2\}$, and one uses an asymmetric parameterization $FG^\top$ to learn $M^*$ where $F \in \mathbb{R}^{n_1 \times k}$ and $G \in \mathbb{R}^{n_2 \times k}$. Building on prior work, 
we give a global exact convergence result of randomly initialized GD for the exact-parameterization case ($k=r$) with an $\exp\left(-\Omega\left(T\right)\right)$ rate.
Furthermore, we give the first global exact convergence result for the over-parameterization case ($k>r$) with an $\exp\left(-\Omega\left(\alpha^2 T\right)\right)$ rate where $\alpha$ is the initialization scale.
This linear convergence result in the over-parameterization case is especially significant because one can apply the asymmetric parameterization to the symmetric setting to speed up from $\Omega\left(1/T^2\right)$ to linear convergence. Therefore, we identify a surprising phenomenon: asymmetric parameterization can exponentially speed up convergence.
Equally surprising is our analysis that highlights the importance of imbalance between $F$ and $G$. This is in sharp contrast to prior works which emphasize balance. 
We further give an example showing the dependency on $\alpha$ in the convergence rate is unavoidable in the worst case.
On the other hand, we propose a novel method that only modifies one step of GD and obtains a convergence rate independent of $\alpha$, recovering the rate in the exact-parameterization case.
We provide empirical studies to verify our theoretical findings.
[Download Paper Here](https://arxiv.org/abs/2310.01769)
