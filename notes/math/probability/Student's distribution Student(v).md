---
aliases: 
anki: false
created: 2024-04-24 12:38
parent:
  - "[[Distribution of r.v. MOC]]"
  - "[[General Random Variables]]"
connected:
  - "#обс/linking"
tags:
  - content/empty
---
> [!tip] Student's distribution $Student(v)$
- [[PDF - f_X(x)|PDF]]: $f_X(x) = \frac{\Gamma(\frac{v+1}{2})}{\sqrt{v\pi}\Gamma(\frac{v}{2})}(1 + \frac{x^2}{v})^{-\frac{v+1}{2}}$
- [[CDF - F_X(x)|CDF]]: $F_X(x) = I_x\left(\frac{v}{2}, \frac{v}{2}\right)$$
- [[Expected Value E(X)|E(X)]]: $\mathbb{E}[X] = 0 \quad \text{if} \quad v > 1$
- [[Variance V(X)|Var(x)]]: $\mathbb{V}[X] = \begin{cases}  \frac{\nu}{\nu - 2} & \text{if } \nu > 2 \\ \infty & \text{if } 1 < \nu \leq 2 \end{cases}$

![[Pasted image 20240424123941.png|300]]
![[Pasted image 20240424123958.png|300]]