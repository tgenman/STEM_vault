---
aliases: 
publish: true
anki: false
created: 2024-04-11 16:15
parent:
  - "[[519.22 Statistic MOC]]"
connected:
  - "#обс/linking"
tags:
  - empty
---

> [!tip] A $1 - \alpha$ confidence interval for a parameter $\theta$ 
is an interval $C_n = (a, b)$ where $a = a(X_1, \ldots, X_n)$ and $b = b(X_1, \ldots, X_n)$ are functions of the data such that
$P(\theta \in C_n) \geq 1 - \alpha, \text{ for all } \theta \in \Theta.$

> [!tip] Coverage of the confidence interval
In words, $(a, b)$ traps $\theta$ with probability $1 - \alpha$. We call $1 - \alpha$ the coverage of the confidence interval.

> [!tip] Confidence set
If $\theta$ is a vector then we use a confidence set (such as a sphere or an ellipse) instead of an interval.


#### Interpretation
On day 1, you collect data and construct a 95 percent confidence interval for a parameter $\theta_1$. On day 2, you collect new data and construct a 95 percent confidence interval for an unrelated parameter $\theta_2$. On day 3, you collect new data and construct a 95 percent confidence interval for an unrelated parameter $\theta_3$. You continue this way constructing confidence intervals for a sequence of unrelated parameters $\theta_1, \theta_2, \ldots$. Then 95 percent of your intervals will trap the true parameter value. There is no need to introduce the idea of repeating the same experiment over and over.
