---
aliases: 
anki: true
created: 2024-03-21 13:16
parent:
  - "[[Expected Value E(X)]]"
connected: 
tags:
---

- $Z = \varphi(X)$
    - $\mathbb{E}[Z] = \int \varphi(x) dF_X(x)$
    - In general, $E[g(X)] \neq g(E[X])$
    - $\mathbb{E}[I_A(x)] = \int I_A(x) dF_X(x) = \int_A dF_X(x) = \mathbb{P}[X \in A]$

###### Proof:
$\sum_y \sum_{x:g(x)=y} g(x) p_X(x) = \sum_y y \sum_{x:g(x)=y} p_X(x) = \sum_y y p_Y(y) = E[Y]$


# Anki
TARGET DECK: math::probability
START
math_complex
FRONT: Expected Value Rule for Functions of Random Variables
BACK: - $Z = \varphi(X)$
- $\mathbb{E}[Z] = \int \varphi(x) dF_X(x)$
    - In general, $E[g(X)] \neq g(E[X])$
    - $\mathbb{E}[I_A(x)] = \int I_A(x) dF_X(x) = \int_A dF_X(x) = \mathbb{P}[X \in A]$
FORMULA: In general, $E[g(X)] \neq g(E[X])$
ADDITIONAL: Proof:
> $\sum_y \sum_{x:g(x)=y} g(x) p_X(x) = \sum_y y \sum_{x:g(x)=y} p_X(x) = \sum_y y p_Y(y) = E[Y]$
PICTURE:
ID: 1711012211417
END
