---
aliases: 
publish: true
anki: false
created: 2024-03-20 11:33
parent:
  - "[[Random Variable (r.v.) X]]"
connected:
  - "[[General Random Variables]]"
tags:
  - empty
---


- A ==discrete random variable== is a real-valued function of the outcome of the [[Random experiment|experiment]]  that can take a finite or countably infinite number of values.
- A discrete random variable has an associated [[Probability mass function (PMF) p_X(x)]], which gives the probability of each numerical value that the ==random variable== can take.
- A function of a ==discrete random variable== defines another ==discrete random variable==, whose [[Probability mass function (PMF) p_X(x)|PMF]] can be obtained from the [[Probability mass function (PMF) p_X(x)|PMF]]  of the original ==random variable==.



![[Pasted image 20240320172753.png]]



[[Probability mass function (PMF) p_X(x)|PMF]]

[[Expected Value E(X)]]

### Expected Value Rule for Functions of Random Variables
Let $X$ be a random variable with PMF $p_X$, and let $g(X)$ be a function of $X$. Then, the expected value of the random variable $g(X)$ is given by
$$E[g(X)] = \sum_x g(x)p_X(x).$$

### Variance
The variance $\text{var}(X)$ of a random variable $X$ is defined by
$$\text{var}(X) = E\left[\left(X - E[X]\right)^2\right],$$
and can be calculated as
$$\text{var}(X) = \sum_x (x - E[X])^2 p_X(x).$$
It is always nonnegative. Its square root is denoted by $\sigma_X$ and is called the standard deviation.

### Mean and Variance of a Linear Function of a Random Variable
Let $X$ be a random variable and let
$$Y = aX + b,$$
where $a$ and $b$ are given scalars. Then,
$$E[Y] = aE[X] + b, \quad \text{var}(Y) = a^2 \text{var}(X).$$

### Variance in Terms of Moments Expression
$$\text{var}(X) = E[X^2] - (E[X])^2.$$
