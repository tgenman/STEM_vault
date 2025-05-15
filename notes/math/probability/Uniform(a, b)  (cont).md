---
aliases: 
anki: true
created: 2024-04-24 11:13
parent:
  - "[[General Random Variables]]"
  - "[[Distribution of r.v. MOC]]"
connected:
  - "[[Uniform(a, b)  (discrete)]]"
tags: 
---

> [!tip] Uniform $\text{Unif}(a, b)$ - continious
- [[PDF - f_X(x)|PDF]]: $f_X(x) = \frac{1}{b-a} \mathbb{I}(a \le x < b)$
- [[CDF - F_X(x)|CDF]]: $F_X(x) = \begin{cases} 0 & x < a \\ \frac{x-a}{b-a} & a \le x < b \\ 1 & x > b \end{cases}$
- [[Expected Value E(X)|E(X)]]: $\mathbb{E}[X] = \frac{a+b}{2}$
- [[Variance V(X)|Var(x)]]: $\mathbb{V}[X] = \frac{(b-a)^2}{12}$
- [[Производящая функция моментов случайной M_X(s)|M_X(s)]]: $M_X(s) = \frac{e^{sb} - e^{sa}}{s(b-a)}$  

![[Pasted image 20240424112617.png|300]]
![[Pasted image 20240424112716.png|300]]

# Anki
TARGET DECK: math::probability 
START
Math_ONE_side
TITLE: Uniform(a, b) (cont)
DESCRIPTION: 
- [[PDF - f_X(x)|PDF]]: $f_X(x) = \frac{1}{b-a} \mathbb{I}(a \le x < b)$
- [[CDF - F_X(x)|CDF]]: $F_X(x) = \begin{cases} 0 & x < a \\ \frac{x-a}{b-a} & a \le x < b \\ 1 & x > b \end{cases}$$
- [[Expected Value E(X)|E(X)]]: $\mathbb{E}[X] = \frac{a+b}{2}$
- [[Variance V(X)|Var(x)]]: $\mathbb{V}[X] = \frac{(b-a)^2}{12}$
- [[Производящая функция моментов случайной M_X(s)|M_X(s)]]: $M_X(s) = \frac{e^{sb} - e^{sa}}{s(b-a)}$  
FORMULA: 
ADDITIONAL:
PICTURE:
![[Pasted image 20240424112617.png|300]]
![[Pasted image 20240424112716.png|300]]
ID: 1713947658742
END