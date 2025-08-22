---
aliases: 
anki: false
created: 2024-04-11 13:28
parent: 
connected:
  - "[[Convergence]]"
tags:
  - fix/empty
---

Let $(T_n)_{n\geq1}$ a sequence of r.v. and $T$ a r.v. ($T$ may be deterministic).

$$ T_n \xrightarrow{(d)} T \text{ iff } \mathbb{P}[T_n \leq x] \rightarrow \mathbb{P}[T \leq x] \text{ as } n \rightarrow \infty, $$ 

for all $x \in \mathbb{R}$ at which the [[CDF - F_X(x)|CDF]] of $T$ is continuous.

---



Последовательность $\xi_n$ сходится по распределению к случайному вектору $\xi$ , если для любой функции $f$, которая действует из $\mathbb{R}^n$ в $\mathbb{R}$ и которая должна быть непрерывна и ограничена, выполнено следующее условие
$$Ef(\xi_n)\to Ef(\xi)$$
