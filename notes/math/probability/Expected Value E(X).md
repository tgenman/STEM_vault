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
![[Pasted image 20240321124118.png|300]]

#### Elementary properties of expectations

- If $X \geq 0$, then $E[X] \geq 0$

- If $a \leq X \leq b$, then $a \leq E[X] \leq b$
$E[X] = \sum_x x p_X(x) \geq \sum_x a p_X(x) = a \sum_x P_X(x) = a \cdot 1 = a$

- If $c$ is a constant, $E[c] = c$
$E[c] = c \cdot p(c) = c$


#### Calculating $E[g(X)]$
- $E[Y] = E[g(X)] = \sum_x g(x) p_X(x)$
	-  In general, $E[g(X)] \neq g(E[X])$

###### Proof:
$\sum_y \sum_{x:g(x)=y} g(x) p_X(x) = \sum_y y \sum_{x:g(x)=y} p_X(x) = \sum_y y p_Y(y) = E[Y]$


#### [[Linearity of expectation]]

#### Requirement for well-definig $E[x]$
 $\sum_{x} |x|p(x) < \infty$







#### Anki
> [!question]- Expected Value E(X)
TARGET DECK: Math::Probability 
START
Math_ONE_side
TITLE: Expected Value E(X)
DESCRIPTION: 
$E[X] = \int x dF(x) =  \begin{cases} \sum_x xp_X(x) & \text{if } X \text{ is discrete} \\\int xf_X(x) dx & \text{if} X \text{ is continuous}\end{cases}$
assuming that the sum (or integral) is well defined. 
FORMULA: 
$p_X$ -[[Probability mass function (PMF) p_X(x)|PMF]]
$f_x$ - [[Probability density function (PDF) f_X(x)|PDF]]
ADDITIONAL:
We use the following notation to denote the expected value of $X$:
$E[X] = EX = \int x dF(x) = \mu = \mu_X$
PICTURE:
ID: 1711011746329
END

> [!question]- Elementary properties of expectations
TARGET DECK: Math::Probability 
START
Math_ONE_side
TITLE: Elementary properties of expectations
DESCRIPTION: 
> - If $X \geq 0$, then $E[X] \geq 0$
> 
> - If $a \leq X \leq b$, then $a \leq E[X] \leq b$
> $E[X] = \sum_x x p_X(x) \geq \sum_x a p_X(x) = a \sum_x P_X(x) = a \cdot 1 = a$
> 
> - If $c$ is a constant, $E[c] = c$
> $E[c] = c \cdot p(c) = c$
FORMULA: 
ADDITIONAL:
PICTURE:
ID: 1711011618300
END

> [!question]- Calculating $E[g(X)]$
TARGET DECK: Math::Probability
START
Math_ONE_side
TITLE: Calculating $E[g(X)]$
DESCRIPTION: $E[Y] = E[g(X)] = \sum_x g(x) p_X(x)$
FORMULA: In general, $E[g(X)] \neq g(E[X])$
ADDITIONAL: Proof:
$\sum_y \sum_{x:g(x)=y} g(x) p_X(x) = \sum_y y \sum_{x:g(x)=y} p_X(x) = \sum_y y p_Y(y) = E[Y]$
PICTURE:
ID: 1711012211417
END

> [!question]- Requirement for well-definig $E[x]$
TARGET DECK: Math::Probability
START
Math_ONE_side
TITLE: Requirement for well-definig $E[x]$
DESCRIPTION:  $\sum_{x} |x|p(x) < \infty$
FORMULA: 
ADDITIONAL:
PICTURE:
ID: 1711014287365
END