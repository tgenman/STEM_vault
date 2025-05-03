---
aliases:
anki: false
created: 2024-04-25 11:39
parent:
  - "[[Limit of function]]"
connected:
  - "#обс/linking"
tags:
  - empty
---

- For independent random variables $X_1, \ldots, X_n$ bounded within intervals $[a_i, b_i]$, Hoeffding's inequality is given by $\mathbb{P}[\bar{X} - \mathbb{E}[\bar{X}] \geq t] \leq e^{-2nt^2}$ for $t > 0$.

- It also states $\mathbb{P}[|\bar{X} - \mathbb{E}[\bar{X}]| \geq t] \leq 2 \exp \left(- \frac{2n^2t^2}{\sum_{i=1}^n (b_i - a_i)^2}\right)$ for $t > 0$.