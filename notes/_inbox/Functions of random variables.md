---
aliases: 
anki: false
created: 2024-04-24 18:44
parent:
  - "[[Random Variable (r.v.) X]]"
connected:
  - "[[The Rule of the Lazy Statistician]]"
  - "[[Convolution]]"
tags:
---
A  [[Function (math)|function]] of a ==random variable== defines another ==random variable==.

- $Z = \varphi(X)$
	- $f_Z(z) = \mathbb{P}[\varphi(X) = z] = \mathbb{P} [X \in \varphi^{-1}(z)] = \sum_{x \in \varphi^{-1}(z)} f_X(x)$
	- $F_Z(z) = \mathbb{P}[\varphi(X) \leq z] = \int_{A_z} f(x) dx$ with $A_z = \{x : \varphi(x) \leq z\}$

[[The Rule of the Lazy Statistician]]
- $\mathbb{E}[Z] = \int \varphi(x) dF_X(x)$
- $\mathbb{E}[I_A(x)] = \int I_A(x) dF_X(x) = \int_A dF_X(x) = \mathbb{P}[X \in A]$


