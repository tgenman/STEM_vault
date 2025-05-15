---
aliases:
  - Mean
  - Матожидание
  - Математическое ожидание
  - First moment
anki: false
created: 2024-03-20 11:20
parent:
  - "[[Moment of r.v.]]"
connected:
  - "[[Median]]"
  - "[[Variance V(X)]]"
  - "[[Пари Паскаля]]"
  - "[[Conditional expectation]]"
tags:
---

> [!tip] The expected value
$E[X] = \int x dF(x) =  \begin{cases} \sum_x xp_X(x) & \text{if } X \text{ is discrete} \\\int xf_X(x) dx & \text{if} X \text{ is continuous}\end{cases}$
assuming that the sum (or integral) is well defined. 
Requirement for well-definig $E[x]$ : $\sum_{x} |x|p(x) < \infty$

$p_X$ -[[PMF - p_X(x)|PMF]]
$f_x$ - [[PDF - f_X(x)|PDF]]

We use the following notation to denote the expected value of $X$:
$E[X] = EX = \int x dF(x) = \mu = \mu_X$


#### Discrete case
We define the expected value (also called the expectation or the mean) of a random variable $X$, with [[PMF - p_X(x)|PMF]] $p_X$, by
$$E[X] = \sum_x xp_X(x).$$
![[Pasted image 20240321124118.png|300]]

#### Properties of expectations
- $P[X = c] = 1 \Rightarrow E[X] = c$
- $E[cX] = cE[X]$
- $E[X + Y] = E[X] + E[Y]$ - [[Linearity of expectation]]
- $E[\varphi(X)] = \sum_{x} \varphi(x)p_X(x)$ - [[The Rule of the Lazy Statistician]]
	- $\mathbb{E}[\varphi(Y)] \neq \varphi(\mathbb{E} [X])$ (cf. [[Jensen Inequality]])
- $\mathbb{E}[XY] = \int x y f_{X,Y}(x, y) dF_X (x) dF_Y (y)$
- $\mathbb{P} [X \geq Y] = 1 \Rightarrow \mathbb{E} [X] \geq \mathbb{E} [Y]$
- $\mathbb{P} [X = Y] = 1 \Rightarrow \mathbb{E} [X] = \mathbb{E} [Y]$
- If $X \geq 0$, then $E[X] \geq 0$
- If $a \leq X \leq b$, then $a \leq E[X] \leq b$
- $\mathbb{E} [X] = \sum_{x=1}^{\infty} \mathbb{P} [X \geq x]$ X discrete


# Anki
TARGET DECK: math::probability 
START
Math_ONE_side
TITLE: Expected Value E(X)
DESCRIPTION: 
$E[X] = \int x dF(x) =  \begin{cases} \sum_x xp_X(x) & \text{if } X \text{ is discrete} \\\int xf_X(x) dx & \text{if} X \text{ is continuous}\end{cases}$
assuming that the sum (or integral) is well defined. 
Requirement for well-definig $E[x]$ : $\sum_{x} |x|p(x) < \infty$
FORMULA: 
$p_X$ -[[PMF - p_X(x)|PMF]]
$f_x$ - [[PDF - f_X(x)|PDF]]
ADDITIONAL:
We use the following notation to denote the expected value of $X$:
$E[X] = EX = \int x dF(x) = \mu = \mu_X$
PICTURE:
ID: 1711011746329
END

TARGET DECK: math::probability 
START
Math_ONE_side
TITLE: Elementary properties of expectations
DESCRIPTION: 
- $P[X = c] = 1 \Rightarrow E[X] = c$
- $E[cX] = cE[X]$
- $E[X + Y] = E[X] + E[Y]$ - [[Linearity of expectation]]
- $E[\varphi(X)] = \sum_{x} \varphi(x)p_X(x)$ - [[The Rule of the Lazy Statistician]]
	- $\mathbb{E}[\varphi(Y)] \neq \varphi(\mathbb{E} [X])$ (cf. [[Jensen Inequality]])
- $\mathbb{E}[XY] = \int x y f_{X,Y}(x, y) dF_X (x) dF_Y (y)$
- $\mathbb{P} [X \geq Y] = 1 \Rightarrow \mathbb{E} [X] \geq \mathbb{E} [Y]$
- $\mathbb{P} [X = Y] = 1 \Rightarrow \mathbb{E} [X] = \mathbb{E} [Y]$
- If $X \geq 0$, then $E[X] \geq 0$
- If $a \leq X \leq b$, then $a \leq E[X] \leq b$
- $\mathbb{E} [X] = \sum_{x=1}^{\infty} \mathbb{P} [X \geq x]$ X discrete
FORMULA: 
ADDITIONAL:
PICTURE:
ID: 1711011618300
END

TARGET DECK: math::probability
START
Math_ONE_side
TITLE: Requirement for well-definig $E[x]$
DESCRIPTION:  $\sum_{x} |x|p(x) < \infty$
FORMULA: 
ADDITIONAL:
PICTURE:
ID: 1711014287365
END