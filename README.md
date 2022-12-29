# HOSKY

## Introduction
In optimization of the least absolute shrinkage and selection operator (Lasso) problem, the fastest algorithm has a convergence rate of $O(1/\sqrt{\epsilon})$.
This polynomial order of $1/\epsilon$ is caused by the undesirable behavior of the absolute function at the origin.
In this paper, we propose an algorithm called _homotopy shrinkage yielding_ (HOSKY), which helps expedite the warm-up stage of the existing algorithms.
With the acceleration by HOSKY in the warm-up stage, one can get a provable convergence rate lower than $O(1/\sqrt{\epsilon})$.
The main idea of the proposed HOSKY algorithm is to use a sequence of surrogate functions to approximate the $\ell_1$ penalty that is used in Lasso.
This sequence of surrogate functions, on the one hand, gets closer and closer to the $\ell_1$ penalty; on the other hand, they are strictly convex and well-conditioned, which enables a provable exponential rate of convergence by gradient-based approaches.
As we will prove in this paper, the convergence rate of the HOSKY algorithm is $O([\log(1/\epsilon_w)]^2)$, where $\epsilon_w$ is the precision used in the warm-up stage.
Our numerical simulations also show that HOSKY empirically performs better in the warm-up stage and accelerates the overall convergence rate.

## Paper reference
Zhao, Yujie, and Xiaoming Huo. "A homotopic method to solve the lasso problems with an improved upper bound of convergence rate." arXiv preprint arXiv:2010.13934 (2020).
