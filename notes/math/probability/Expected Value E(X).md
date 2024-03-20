---
aliases:
  - Среднее арифметическое
  - Mean
  - Матожидание
  - Математическое ожидание
  - First moment
publish: true
anki: false
created: 2024-03-20 11:20
parent:
  - "[[Moment of r.v.]]"
connected:
  - "[[Median]]"
  - "[[Variance V(X)]]"
  - "[[Пари Паскаля]]"
tags:
  - empty
---

> [!tip] The expected value
$E[X] = \int x dF(x) =  \begin{cases} \sum_x xp_X(x) & \text{if } X \text{ is discrete} \\\int xf_X(x) dx & \text{if} X \text{ is continuous}\end{cases}$
assuming that the sum (or integral) is well defined. 

$p_X$ -[[Probability mass function (PMF) p_X(x)|PMF]]
$f_x$ - [[Probability density function (PDF) f_X(x)|PDF]]

We use the following notation to denote the expected value of $X$:
$E[X] = EX = \int x dF(x) = \mu = \mu_X$


#### Discrete case
We define the expected value (also called the expectation or the mean) of a random variable $X$, with [[Probability mass function (PMF) p_X(x)|PMF]] $p_X$, by
$$E[X] = \sum_x xp_X(x).$$





