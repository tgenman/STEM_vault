---
aliases:
  - Распределение случайной величины
  - Закон распределения
anki: false
created: "2026-09-15"
parent:
  - "[[Probability measure]]"
connected:
  - "[[Real numbers R]]"
  - "[[517.518.113 Borel sigma-algebra]]"
  - "[[Sample space]]"
  - "[[Random Variable (r.v.) X]]"
  - "[[Distribution of r.v. MOC]]"
  - "[[CDF - F_X(x)]]"
tags:
  - контент/определение
---

> [!tip] probability distribution
> The law of a random variable is the probability measure it induces on its value space.

For a real-valued measurable $X:(\Omega,\mathcal F,P)\to(\mathbb R,\mathcal B(\mathbb R))$:
$$
P_X(A)=P(X^{-1}(A))=P(X\in A),\qquad A\in\mathcal B(\mathbb R).
$$

Thus a law on $\mathbb R$ is a [[Probability measure]] on the Borel sets of $\mathbb R$. The original experiment's sample space $\Omega$ need not equal $\mathbb R$.

A [[CDF - F_X(x)|CDF]] determines a real-valued law. A [[PDF - f_X(x)|density]] is an additional representation available for absolutely continuous laws.

Source: [MIT: random variables and distributions](https://ocw.mit.edu/courses/18-175-theory-of-probability-spring-2014/827332a721e47b09cb0cbcfb4b60ecf6_MIT18_175S14_Lecture3.pdf).
