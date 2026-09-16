---
aliases:
anki: false
created: 2024-03-21 11:20
parent:
  - "[[Discrete Random Variable]]"
  - "[[Distribution of r.v. MOC]]"
connected:
  - "[[Uniform(a, b)  (cont)]]"
tags:
---

> [!tip] Uniform r.v. $U(a, b)$
- [[PMF - p_X(x)|PMF]]: $p_X(x) = \frac{1}{b-a+1} \mathbb{I}(x\in\mathbb Z,\ a \le x \le b)$
- [[CDF - F_X(x)|CDF]]: $F_X(x) = \begin{cases} 0 & x < a \\ \frac{\lfloor x \rfloor-a + 1}{b-a+1} & a \le x \le b \\ 1 & x > b \end{cases}$
- [[Expected Value E(X)|E(X)]]: $\mathbb{E}[X] = \frac{a+b}{2}$
- [[Variance V(X)|Var(x)]]: $\mathbb{V}[X] = \frac{(b-a+1)^2-1}{12}$
- [[Производящая функция моментов случайной M_X(s)|M_X(s)]]: $M_X(s) = \frac{1}{b-a+1}\sum_{k=a}^{b}e^{sk},\quad s\in\mathbb R$
- Parameters: integers $a, b$; $a \leq b$
- [[Random experiment|Experiment]]: Pick one of $a, a + 1, \ldots, b$ at random; all equally likely
- [[Sample space]]: $\{a, a + 1, \ldots, b\}$
- Random variable $X$: $X(\omega) = \omega$
- Model of: complete ignorance


![[Pasted image 20240423215103.png|400]]


- Special case: $a = b$ constant/deterministic r.v.
![[Pasted image 20240321112304.png|300]]


#### [[Expected Value E(X)]]
The following proof uses the special case $a=0$, $b=n$.
$E[X] = \frac{n}{2}$
###### Proof
$E[X] = 0 \cdot \frac{1}{n+1} + 1 \cdot \frac{1}{n+1} + \ldots + n \cdot \frac{1}{n+1} = \frac{1}{n+1} (0 + 1 + \ldots + n) = \frac{1}{n+1} \cdot \frac{n(n+1)}{2} = \frac{n}{2}$

#### [[Variance V(X)]]
The proof starts with $a=0$, $b=n$.
$\text{var}(X) = \frac{1}{12} (b-a)(b-a+2)$

###### Proof
$\text{var}(X) = E[X^2] - (E[X])^2 = \frac{1}{n+1} (0^2 + 1^2 + 2^2 + \ldots + n^2) - \left(\frac{n}{2}\right)^2$
$E[X^2] = \frac{1}{n+1} \cdot \frac{n(n+1)(2n+1)}{6} = \frac{n(2n+1)}{6}$
$\text{var}(X) = \frac{n(2n+1)}{6} - \left(\frac{n}{2}\right)^2 = \frac{n(2n+1)}{6} - \frac{n^2}{4} = \frac{1}{12} n(n+2)$
For a general uniform distribution from $a$ to $b$:
$\text{var}(X) = \frac{1}{12} (b-a)(b-a+2)$

## источник

[SciPy: discrete uniform](https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.randint.html); для включённых границ $a,b$ соответствуют параметры `low=a, high=b+1`.

# Anki
TARGET DECK: math::probability
START
math_complex
FRONT: Uniform r.v. (discrete) $U(a, b)$
BACK:
- [[PMF - p_X(x)|PMF]]: $p_X(x) = \frac{1}{b-a+1} \mathbb{I}(x\in\mathbb Z,\ a \le x \le b)$
- [[CDF - F_X(x)|CDF]]: $F_X(x) = \begin{cases} 0 & x < a \\ \frac{\lfloor x \rfloor-a + 1}{b-a+1} & a \le x \le b \\ 1 & x > b \end{cases}$
- [[Expected Value E(X)|E(X)]]: $\mathbb{E}[X] = \frac{a+b}{2}$
- [[Variance V(X)|Var(x)]]: $\mathbb{V}[X] = \frac{(b-a+1)^2-1}{12}$
- [[Производящая функция моментов случайной M_X(s)|M_X(s)]]: $M_X(s) = \frac{1}{b-a+1}\sum_{k=a}^{b}e^{sk},\quad s\in\mathbb R$
- Parameters: integers $a, b$; $a \leq b$
- [[Random experiment|Experiment]]: Pick one of $a, a + 1, \ldots, b$ at random; all equally likely
- [[Sample space]]: $\{a, a + 1, \ldots, b\}$
- Random variable $X$: $X(\omega) = \omega$
- Model of: complete ignorance
FORMULA:
ADDITIONAL:
PICTURE:
> ![[Pasted image 20240423215103.png|400]]
- Special case: $a = b$ constant/deterministic r.v.
> ![[Pasted image 20240321112304.png|300]]
ID: 1711009548615
END

TARGET DECK: math::probability
START
math_complex
FRONT: Expected Value E(X) Uniform r.v. (discrete)
BACK: $E[X] = \frac{a+b}{2}$; for $a=0$, $b=n$, this is $n/2$.
FORMULA: Proof for $a=0$, $b=n$
$E[X] = 0 \cdot \frac{1}{n+1} + 1 \cdot \frac{1}{n+1} + \ldots + n \cdot \frac{1}{n+1} = \frac{1}{n+1} (0 + 1 + \ldots + n) = \frac{1}{n+1} \cdot \frac{n(n+1)}{2} = \frac{n}{2}$
ADDITIONAL:
PICTURE:
ID: 1711011427808
END

TARGET DECK: math::probability
START
math_complex
FRONT: Variance V(X) Uniform r.v. (discrete)
BACK: $\text{var}(X) = \frac{1}{12} (b-a)(b-a+2)$
FORMULA: Proof for $a=0$, $b=n$
$\text{var}(X) = E[X^2] - (E[X])^2 = \frac{1}{n+1} (0^2 + 1^2 + 2^2 + \ldots + n^2) - \left(\frac{n}{2}\right)^2$
$E[X^2] = \frac{1}{n+1} \cdot \frac{n(n+1)(2n+1)}{6} = \frac{n(2n+1)}{6}$
$\text{var}(X) = \frac{n(2n+1)}{6} - \left(\frac{n}{2}\right)^2 = \frac{n(2n+1)}{6} - \frac{n^2}{4} = \frac{1}{12} n(n+2)$
For a general uniform distribution from $a$ to $b$:
$\text{var}(X) = \frac{1}{12} (b-a)(b-a+2)$
ADDITIONAL:
PICTURE:
ID: 1711024863163
END
