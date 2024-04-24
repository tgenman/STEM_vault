---
aliases:
  - Дисперсия
  - Dispersion
  - Second moment
  - Второй момент
publish: true
anki: false
created: 2024-01-06 13:08
parent:
  - "[[Moment of r.v.]]"
connected:
  - "[[Expected Value E(X)]]"
  - "[[Standard deviation]]"
tags:
---

> [!tip] Variance 
a measure of the spread of a [[PMF - p_X(x)|PMF]]  and [[PDF - f_X(x)|PDF]]
$\text{var}(X) = \sum_{x} (x-\mu)^2 p_X(x)$
$\text{var}(X) = E[(X - E[X])^2]$


#### Properties
- $\text{var}(aX + b) = a^2\text{var}(X)$
	- $\text{var}(aX + b) = \sum_{x} (ax + b - E[aX + b])^2 p_X(x)$ $= \sum_{x} (ax + b - aE[X] - b)^2 p_X(x)$ $= a^2 \sum_{x} (x - E[X])^2 p_X(x) = a^2 \text{var}(X).$
- $\text{var}(X) = E[X^2] - (E[X])^2$ - Variance in Terms of [[Moment of r.v.|Moments]]  Expression
	- $\text{var}(X) = E[(X-\mu)^2] = E[X^2 - 2\mu X + \mu^2]$ $= E[X^2] - 2\mu E[X] + \mu^2 = E[X^2] - (E[X])^2$
- $V\left[\sum_{i=1}^{n} X_i\right] = \sum_{i=1}^{n} V[X_i] + \sum_{i\neq j} \text{Cov}[X_i, X_j]$.
- $V\left[\sum_{i=1}^{n} X_i\right] = \sum_{i=1}^{n} V[X_i]$ if $X_i \perp\!\!\!\perp X_j$.




#### Anki
> [!question]- Variance
TARGET DECK: Math::Probability
START
Math_ONE_side
TITLE: Variance
DESCRIPTION: a measure of the spread of a [[PMF - p_X(x)|PMF]] 
FORMULA: 
> $\text{var}(X) = \sum_{x} (x-\mu)^2 p_X(x)$
> $\text{var}(X) = E[(X - E[X])^2]$
ADDITIONAL:
PICTURE:
ID: 1711017251662
END

> [!question]- Properties of Variance
TARGET DECK: Math::Probability
START
Math_ONE_side
TITLE: Properties of Variance
DESCRIPTION: 
> - $\text{var}(aX + b) = a^2\text{var}(X)$
>	- $\text{var}(aX + b) = \sum_{x} (ax + b - E[aX + b])^2 p_X(x)$ $= \sum_{x} (ax + b - aE[X] - b)^2 p_X(x)$ $= a^2 \sum_{x} (x - E[X])^2 p_X(x) = a^2 \text{var}(X).$
> - $\text{var}(X) = E[X^2] - (E[X])^2$ - Variance in Terms of [[Moment of r.v.|Moments]]  Expression
>	- $\text{var}(X) = E[(X-\mu)^2] = E[X^2 - 2\mu X + \mu^2]$ $= E[X^2] - 2\mu E[X] + \mu^2 = E[X^2] - (E[X])^2$
> - $V\left[\sum_{i=1}^{n} X_i\right] = \sum_{i=1}^{n} V[X_i] + \sum_{i\neq j} \text{Cov}[X_i, X_j]$.
> - $V\left[\sum_{i=1}^{n} X_i\right] = \sum_{i=1}^{n} V[X_i]$ if $X_i \perp\!\!\!\perp X_j$.
FORMULA: 
ADDITIONAL:
PICTURE:
ID: 1711017251672
END









