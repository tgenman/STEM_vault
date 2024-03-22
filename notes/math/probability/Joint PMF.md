---
aliases: 
publish: true
anki: false
created: 2024-03-21 16:05
parent:
  - "[[PMF - p_X(x)|PMF]]"
connected:
  - "#обс/linking"
tags:
  - empty
---

> [!tip] Joint PMF
In particular, if $(x, y)$ is a pair of possible values of $X$ and $Y$, the probability mass of $(x, y)$ is the probability of the event $\{X = x, Y = y\}$:
$p_{X,Y}(x, y) = P(X = x, Y = y)$

Here and elsewhere, we use the abbreviated notation $P(X = x, Y = y)$ instead of the more precise notations $P(\{X = x\} \cap \{Y = y\})$ or $P(X = x \text{ and } Y = y)$.

![[Pasted image 20240321160907.png]]

$\sum_x \sum_y p_{X,Y}(x, y) = 1$
$p_X(x) = \sum_y p_{X,Y}(x, y)$
$p_Y(y) = \sum_x p_{X,Y}(x, y)$

