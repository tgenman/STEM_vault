---
aliases: 
anki: false
created: 2024-04-11 13:27
parent:
  - "[[Convergence]]"
connected:
  - "#обс/linking"
tags:
  - empty
---


Convergence in $L^p$ $(p \geq 1)$
Let $(T_n)_{n\geq1}$ a sequence of r.v. and $T$ a r.v. ($T$ may be deterministic).

$$ T_n \xrightarrow{L^p} T \text{ iff } \mathbb{E}\left[\left|T_n - T\right|^p\right] \rightarrow 0 \text{ as } n \rightarrow \infty. $$

---


Последовательность $\xi_n$ сходится к случайному вектору $\xi$ в $L_p$
$$\xi_n\xrightarrow[]{L_p}\xi$$
если $\xi_n\in L_p$, что означает, что для любого $n$ математические ожидания:
$$E(||\xi_n||_P)^P<+\infty$$
$$E(||\xi||_P)^P< +\infty$$
$$E(||\xi_n-\xi||_P)^P\xrightarrow[n\to \infty]{}0$$

Норма вектора $x$ в пространстве $L_P$:
$$||x||_P=\big(|x_1|^P+\ldots+|x_n|^P\big)^{1/P}$$

