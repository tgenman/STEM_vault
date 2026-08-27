---
aliases: 
anki: false
created: 2024-04-24 18:54
parent:
  - "[[Random Variable (r.v.) X]]"
connected:
  - "[[Variance V(X)]]"
  - "[[Correlation]]"
tags:
  - fix/empty
---

> [!tip] Covariance
 $\text{Cov}[X, Y] = \mathbb{E}[(X - \mathbb{E}[X])(Y - \mathbb{E}[Y])] = \mathbb{E}[XY] - \mathbb{E}[X]\mathbb{E}[Y]$.

### Properties
- $\text{Cov}[X, a] = 0$.
- $\text{Cov}[X, X] = V[X]$.
- $\text{Cov}[X, Y] = \text{Cov}[Y, X]$ - [[Symmetric]]
- $\text{Cov}[aX, bY] = ab\text{Cov}[X, Y]$.
- $\text{Cov}[X + a, Y + b] = \text{Cov}[X, Y]$.
- $\text{Cov}\left[\sum_{i=1}^{n} X_i, \sum_{j=1}^{m} Y_j\right] = \sum_{i=1}^{n}\sum_{j=1}^{m} \text{Cov}[X_i, Y_j]$.

