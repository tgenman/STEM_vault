---
aliases:
  - Stein paradox
publish: true
anki: false
created: 2024-04-11 15:46
parent:
  - "[[Bias]]"
  - "[[Variance V(X)]]"
connected:
  - "#обс/linking"
tags:
  - empty
---

[[Bias]] and [[Standard error]] are strongly connected in a [[Mean squared error MSE|MSE]]:
$\text{MSE}(\hat{\theta}) = \text{bias}^2(\hat{\theta}) + \text{se}^2(\hat{\theta})$
$\text{MSE}(\hat{\theta}) = \text{bias}^2(\hat{\theta}) + \text{Var}(\hat{\theta})$

![[Pasted image 20240411154556.png]]
*Figure 1: Example of bias-variance tradeoff on a regression problem*