---
aliases:
  - EVT
  - Теорема Вейерштрасса
anki: true
created: 2023-07-07 10:02
parent:
  - "[[Continuous function]]"
connected:
  - "[[Intermediate Value Theorem (IVT)]]"
  - "[[Compact set]]"
  - "[[supremum X (sup X)]]"
  - "[[infimum X (inf X)]]"
tags:
  - theorem
---

> [!tip] Extreme Value Theorem (EVT)
> If $f$ is [[Continuous function|continuous]] on a closed and bounded interval $[a,b]$, then $f$ attains both its maximum and minimum values on $[a,b]$.

## Statement

Let $f: [a,b] \rightarrow \mathbb{R}$ be a continuous function on the closed interval $[a,b]$. Then:

1. There exists $c \in [a,b]$ such that $f(c) \geq f(x)$ for all $x \in [a,b]$ (global maximum)
2. There exists $d \in [a,b]$ such that $f(d) \leq f(x)$ for all $x \in [a,b]$ (global minimum)

In other words: $f([a,b])$ is bounded and both $\sup f([a,b])$ and $\inf f([a,b])$ are attained.

## Key Conditions

- **[[Continuous function|Continuity]]**: $f$ must be continuous on $[a,b]$
- **Closed interval**: The domain must be closed (includes endpoints)
- **Bounded interval**: The domain must be bounded (finite length)

Without any of these conditions, the theorem may fail.

## Examples

**Example 1**: $f(x) = x^2$ on $[0,2]$ attains its minimum at $x=0$ and maximum at $x=2$.

**Example 2**: $f(x) = \frac{1}{x}$ on $(0,1]$ (open at 0) has no maximum value as $x \to 0^+$.

# Anki

TARGET DECK: stem::math::calculus
START
math_basic_single
FRONT: Extreme Value Theorem (EVT) - conditions
What conditions must a function satisfy to guarantee it attains maximum and minimum values?
BACK: Function must be **continuous** on a **closed and bounded** interval $[a,b]$
ID: 1755880831676
END

TARGET DECK: stem::math::calculus
START
math_complex
FRONT: Extreme Value Theorem (EVT)
BACK: If $f$ is continuous on a closed and bounded interval $[a,b]$, then $f$ attains both its maximum and minimum values on $[a,b]$
FORMULA: $\exists c,d \in [a,b]: f(c) = \max_{x \in [a,b]} f(x)$ and $f(d) = \min_{x \in [a,b]} f(x)$
ADDITIONAL: Key conditions:
- Continuity on $[a,b]$ 
- Closed interval (includes endpoints)
- Bounded interval (finite length)
Without these conditions, theorem may fail
PICTURE:
PROOF:
ID: 1755880831680
END

TARGET DECK: stem::math::calculus
START
math_basic_single
FRONT: Why does EVT fail on open intervals?
Give an example where a continuous function on an open interval doesn't attain its extrema.
BACK: $f(x) = \frac{1}{x}$ on $(0,1]$ has no maximum as $x \to 0^+$. The supremum exists but is not attained.
ID: 1755880831683
END
