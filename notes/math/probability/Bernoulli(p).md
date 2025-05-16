---
aliases: 
anki: true
created: 2024-03-20 19:01
parent:
  - "[[Discrete Random Variable]]"
connected:
  - "[[Схема испытиний Бернулли]]"
  - "[[Binomial distribution Bin(n, p)]]"
  - "[[Indicator function]]"
tags: 
---

Consider the toss of a coin, which comes up a head with probability $p$, and a tail with probability $1 - p$. The Bernoulli random variable takes the two values 1 and 0, depending on whether the outcome is a head or a tail:

$X = \begin{cases} 1 & \text{if a head}, \\ 0 & \text{if a tail}. \end{cases}$

Its PMF is

$p_X(k) = \begin{cases} p & \text{if } k = 1, \\ 1 - p & \text{if } k = 0. \end{cases}$

Using [[Indicator function]]
![[Pasted image 20240320190523.png|300]]

For all its simplicity, the Bernoulli random variable is very important. In practice, it is used to model generic probabilistic situations with just two outcomes, such as:
- The state of a telephone at a given time that can be either free or busy.
- A person who can be either healthy or sick with a certain disease.
- The preference of a person who can be either for or against a certain political candidate.

Furthermore, by combining multiple Bernoulli random variables, one can construct more complicated random variables, such as the [[Binomial distribution Bin(n, p)]] 

#### [[Expected Value E(X)]]

$X = \begin{cases} 1, & \text{w.p. } p \\0, & \text{w.p. } 1-p \end{cases}$
$E[X] = 1\cdot p + 0\cdot(1-p) = p$


#### [[Variance V(X)]]
$\text{var}(X) = p(1-p)$

###### Proof
$\text{var}(X) = \sum_{x} (x - E[X])^2 p_X(x) = (1-p)^2 p + (0-p)^2 (1-p) =$
$= p - 2p^2 + p^3 + p^2 - p^3 = p - p^2 = p(1-p)$

$\text{var}(X) = E[X^2] - (E[X])^2 = E[X] - (E[X])^2 = p - p^2 = p(1-p)$






# Anki
TARGET DECK: math::probability
START
math_complex
TITLE: Bernoulli r.v.
DESCRIPTION: Consider the toss of a coin, which comes up a head with probability $p$, and a tail with probability $1 - p$. The Bernoulli random variable takes the two values 1 and 0, depending on whether the outcome is a head or a tail:
$X = \begin{cases} 1 & \text{if a head}, \\ 0 & \text{if a tail}. \end{cases}$
Its PMF is
$p_X(k) = \begin{cases} p & \text{if } k = 1, \\ 1 - p & \text{if } k = 0. \end{cases}$
FORMULA: 
ADDITIONAL:
For all its simplicity, the Bernoulli random variable is very important. In practice, it is used to model generic probabilistic situations with just two outcomes, such as:
- The state of a telephone at a given time that can be either free or busy.
- A person who can be either healthy or sick with a certain disease.
- The preference of a person who can be either for or against a certain political candidate.
Furthermore, by combining multiple Bernoulli random variables, one can construct more complicated random variables, such as the [[Binomial distribution Bin(n, p)]] 
PICTURE:
Using [[Indicator function]]
![[Pasted image 20240320190523.png|300]]
ID: 1710951062308
END

TARGET DECK: math::probability 
START
math_complex
TITLE: Expected Value E(X) of Bernoulli r.v.
DESCRIPTION: 
$X = \begin{cases} 1, & \text{w.p. } p \\0, & \text{w.p. } 1-p \end{cases}$
$E[X] = 1\cdot p + 0\cdot(1-p) = p$
FORMULA: 
ADDITIONAL:
PICTURE:
ID: 1711010147059
END

TARGET DECK: math::probability 
START
math_complex
TITLE: Variance V(X) of Bernoulli r.v.
DESCRIPTION: $\text{var}(X) = p(1-p)$
FORMULA: 
ADDITIONAL: Proof
$\text{var}(X) = \sum_{x} (x - E[X])^2 p_X(x) = (1-p)^2 p + (0-p)^2 (1-p) =$
$= p - 2p^2 + p^3 + p^2 - p^3 = p - p^2 = p(1-p)$
$\text{var}(X) = E[X^2] - (E[X])^2 = p - p^2 = p(1-p)$
PICTURE:
ID: 1711017462547
END
