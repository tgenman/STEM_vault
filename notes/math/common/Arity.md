---
aliases:
  - Арность
  - Valency
  - Местность
anki: true
created: 2025-05-20 14:22
parent:
  - "[[510.22 Set theory]]"
connected: 
tags:
---

> [!tip] Arity
> is the number of arguments that a function, operation, or relation takes.

For a function $f$, if it takes $n$ arguments, we say it has arity $n$ or is $n$-ary.

# Types of Arity

| Arity | Name                       | [[Operation on elements of set\|Operation]] Example | [[Relation]] Example                           |
| ----- | -------------------------- | --------------------------------------------------------- | ---------------------------------------------- |
| 0     | [[Nullary arity\|Nullary]] | Constant: $f() = 5$                                       | Property of entire set: "set $A$ is non-empty" |
| 1     | [[Unary arity\|Unary]]     | $-x$, $\neg x$, $f(x) = x^2$                              | "x is even", "x > 0", "x ∈ A"                  |
| 2     | [[Binary arity]]           | $x + y$, $x \cdot y$, $\max(x, y)$                        | $x < y$, $x = y$, $x \perp y$                  |
| 3     | [[Ternary arity\|Ternary]] | $f(x,y,z) = \text{if } x \text{ then } y \text{ else } z$ | $x + y > z$                                    |
| n     | [[n-ary arity\|n-ary]]     | $f(x_1, x_2, \dots, x_n)$                                 | $x_1 + \dots + x_n = 0$                        |


# Anki
TARGET DECK: stem::math::common

START
math_basic_double
FRONT: Arity (valency)
BACK: is the number of arguments that a function, operation, or relation takes.
ID: 1747745634669
END
