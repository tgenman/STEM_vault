---
aliases: 
publish: true
anki: false
created: 2024-03-21 13:16
parent:
  - "[[Expected Value E(X)]]"
connected: 
tags: []
---

Let $X$ be a random variable with PMF $p_X$, and let $g(X)$ be a function of $X$. Then, the expected value of the random variable $g(X)$ is given by
$E[g(X)] = \sum_{x} g(x)p_X(x)$
	-  In general, $E[g(X)] \neq g(E[X])$


###### Proof:
$\sum_y \sum_{x:g(x)=y} g(x) p_X(x) = \sum_y y \sum_{x:g(x)=y} p_X(x) = \sum_y y p_Y(y) = E[Y]$


#### Anki
> [!question]- Expected Value Rule for Functions of Random Variables
TARGET DECK: Math::Probability
START
Math_ONE_side
TITLE: Expected Value Rule for Functions of Random Variables
DESCRIPTION: Let $X$ be a random variable with PMF $p_X$, and let $g(X)$ be a function of $X$. Then, the expected value of the random variable $g(X)$ is given by
$E[g(X)] = \sum_{x} g(x)p_X(x)$
FORMULA: In general, $E[g(X)] \neq g(E[X])$
ADDITIONAL: Proof:
$\sum_y \sum_{x:g(x)=y} g(x) p_X(x) = \sum_y y \sum_{x:g(x)=y} p_X(x) = \sum_y y p_Y(y) = E[Y]$
PICTURE:
ID: 1711012211417
END
