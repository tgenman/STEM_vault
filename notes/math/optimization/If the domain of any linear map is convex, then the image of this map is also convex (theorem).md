---
aliases: 
anki: true
created: 2024-10-27 21:57
parent:
  - "[[Convex Set]]"
  - "[[Function (math)]]"
connected: 
tags:
  - theorem
---

> [!tip] Theorem
If the [[Domain Dom(f) or Preimage|domain]]  of any [[Function (math)|linear map]]  is convex, then the [[Range Ran(f) or Image Im(f)|image]]  of this map is also convex.

#### Proof
- Let $\mathcal{X}$ be a convex set and $x, y \in \mathcal{X}$.
- Let $f$ be a linear map: $f(x) = A x + b$.
- Show that $\alpha f(x) + (1-\alpha) f(y) \in f(\mathcal{X})$, where $\alpha \in [0, 1]$.
Indeed, $\alpha f(x) + (1-\alpha) f(y) = \alpha (A x + b) + (1-\alpha) (A y + b)=$
$= A (\alpha x + (1-\alpha) y) + b = f(z),$
where $z = \alpha x + (1-\alpha) y \in \mathcal{X}$.

# Anki
TARGET DECK: math::optimization
START
Math_ONE_side
TITLE: If the [[Domain Dom(f) or Preimage|domain]]  of any [[Function (math)|linear map]]  is convex, then the [[Range Ran(f) or Image Im(f)|image]]  of this map is
DESCRIPTION: also convex.
ADDITIONAL:
Let $\mathcal{X}$ be a convex set and $x, y \in \mathcal{X}$.
Let $f$ be a linear map: $f(x) = A x + b$.
Show that $\alpha f(x) + (1-\alpha) f(y) \in f(\mathcal{X})$, where $\alpha \in [0, 1]$.
Indeed, $\alpha f(x) + (1-\alpha) f(y) = \alpha (A x + b) + (1-\alpha) (A y + b)=$
$= A (\alpha x + (1-\alpha) y) + b = f(z),$
where $z = \alpha x + (1-\alpha) y \in \mathcal{X}$.
ID: 1734969268996
END