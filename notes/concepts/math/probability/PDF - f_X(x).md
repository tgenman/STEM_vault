---
aliases:
  - PDF
  - Probability density function
  - Плотность функции распределения
anki: false
created: 2024-03-20 18:32
parent:
  - "[[General Random Variables]]"
connected:
  - "[[PMF - p_X(x)|PMF]]"
  - "[[CDF - F_X(x)|CDF]]"
tags:
  - контент/определение
---

> [!tip] probability density function
> For a real random variable with an absolutely continuous law, a density $f_X$ is nonnegative and satisfies
> $$P(X\in A)=\int_A f_X(x)\,dx$$
> for Borel sets $A$.

Its integral over $\mathbb R$ is one. Density values are not point probabilities and may exceed one. Not every [[probability distribution]] has a density.

Source: [NIST: probability distributions](https://www.itl.nist.gov/div898/handbook/eda/section3/eda361.htm).
