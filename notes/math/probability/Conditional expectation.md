---
aliases: 
publish: true
anki: false
created: 2024-04-24 18:35
parent:
  - "[[Expected Value E(X)]]"
  - "[[Conditional Probability]]"
connected:
  - "[[Conditional variance]]"
tags:
---


### Properties
- $\mathbb{E} [Y | X = x] = \int y f(y | x) dy$
- $\mathbb{E} [X] = \mathbb{E} [\mathbb{E} [X | Y]]$
- $\mathbb{E}_{\varphi(X,Y) | X=x} = \int_{-\infty}^{\infty} \varphi(x, y) f_{Y|X} (y | x) dy$
- $\mathbb{E} [\varphi(Y, Z) | X = x] = \int_{-\infty}^{\infty} \varphi(y, z) f_{Y,Z|X}(y, z | x) dy dz$
- $\mathbb{E} [Y + Z | X] = \mathbb{E} [Y | X] + \mathbb{E} [Z | X]$
- $\mathbb{E} [\varphi(X)Y | X] = \varphi(X)\mathbb{E} [Y | X]$
- $\mathbb{E} [Y | X] = c \Rightarrow \text{Cov} [X, Y] = 0$