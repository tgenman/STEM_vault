---
aliases:
  - CDF
  - Cumulative distribution function
  - Функция распределения
anki: false
created: 2024-03-20 18:33
parent:
  - "[[General Random Variables]]"
connected:
  - "[[PMF - p_X(x)|PMF]]"
  - "[[PDF - f_X(x)|PDF]]"
tags:
  - контент/определение
---

> [!tip] cumulative distribution function
> For a real random variable $X$, $F_X(x)=P(X\le x)$.

The definition applies to discrete, absolutely continuous and other real-valued laws. For an absolutely continuous law,
$$
F_X(x)=\int_{-\infty}^x f_X(t)\,dt.
$$

General properties and an existing proof are in [[Distribution function]]; that note is retained separately.

Sources: [MIT: random variables and distributions](https://ocw.mit.edu/courses/18-175-theory-of-probability-spring-2014/827332a721e47b09cb0cbcfb4b60ecf6_MIT18_175S14_Lecture3.pdf), [NIST: CDF](https://www.itl.nist.gov/div898/handbook/eda/section3/eda362.htm).
