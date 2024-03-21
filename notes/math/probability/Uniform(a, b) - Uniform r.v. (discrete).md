---
aliases: 
publish: true
anki: false
created: 2024-03-21 11:20
parent:
  - "[[Discrete Random Variable]]"
connected: 
tags:
---

> [!tip] Uniform r.v. (discrete)
> - Parameters: integers $a, b$; $a \leq b$
> - [[Random experiment|Experiment]]: Pick one of $a, a + 1, \ldots, b$ at random; all equally likely
> - [[Sample space]]: $\{a, a + 1, \ldots, b\}$
> - Random variable $X$: $X(\omega) = \omega$
> - Model of: complete ignorance

![[Pasted image 20240321112128.png|500]]

- Special case: $a = b$ constant/deterministic r.v.
![[Pasted image 20240321112304.png|300]]


#### [[Expected Value E(X)]]
$E[X] = 0 \cdot \frac{1}{n+1} + 1 \cdot \frac{1}{n+1} + \ldots + n \cdot \frac{1}{n+1} = \frac{1}{n+1} (0 + 1 + \ldots + n) = \frac{1}{n+1} \cdot \frac{n(n+1)}{2} = \frac{n}{2}$
$E[X] = \frac{n}{2}$



#### Anki
> [!question]- Uniform r.v. (discrete)
TARGET DECK: Math::Probability
START
Math_ONE_side
TITLE: Uniform r.v. (discrete)
DESCRIPTION: 
> - Parameters: integers $a, b$; $a \leq b$
> - [[Random experiment|Experiment]]: Pick one of $a, a + 1, \ldots, b$ at random; all equally likely
> - [[Sample space]]: $\{a, a + 1, \ldots, b\}$ 
> - Random variable $X$: $X(\omega) = \omega$
> - Model of: complete ignorance
FORMULA: 
ADDITIONAL:
PICTURE:
> ![[Pasted image 20240321112128.png|500]]
> - Special case: $a = b$ constant/deterministic r.v.
> ![[Pasted image 20240321112304.png|300]]
ID: 1711009548615
END

> [!question]- Expected Value E(X) Uniform r.v. (discrete)
TARGET DECK: Math::Probability 
START
Math_ONE_side
TITLE: Expected Value E(X) Uniform r.v. (discrete)
DESCRIPTION: $E[X] = \frac{n}{2}$
FORMULA: $E[X] = 0 \cdot \frac{1}{n+1} + 1 \cdot \frac{1}{n+1} + \ldots + n \cdot \frac{1}{n+1} = \frac{1}{n+1} (0 + 1 + \ldots + n) = \frac{1}{n+1} \cdot \frac{n(n+1)}{2} = \frac{n}{2}$
ADDITIONAL:
PICTURE:
ID: 1711011427808
END
