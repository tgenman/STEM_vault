---
aliases:
  - Уровень значимости
  - Alpha level
anki: false
created: "2026-09-15"
parent:
  - "[[519.22 Statistic MOC]]"
connected:
  - "[[Hypothesis testing]]"
  - "[[False positive]]"
  - "[[p-value]]"
tags:
  - контент/определение
---

> [!tip] significance level
> A pre-specified upper bound $\alpha$ on a test's probability of rejecting a true null hypothesis.

For a level-$\alpha$ test,
$$
P_\theta(\text{reject }H_0)\le\alpha,\qquad \theta\in\Theta_0.
$$

The nominal bound need not equal the actual rejection probability. $\alpha$ is not the probability that $H_0$ is true, and $0.05$ is a convention rather than part of the definition.

Source: [NIST: critical values and p-values](https://itl.nist.gov/div898/handbook/prc/section1/prc131.htm).
