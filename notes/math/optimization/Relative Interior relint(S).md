---
aliases:
  - Относительная внутренность
anki: true
created: 2024-12-21 19:08
parent:
  - "[[Interior int(S)]]"
  - "[[519.853.3 Convex optimization MOC]]"
connected:
  - "[[Affine hull - aff(S)]]"
  - "[[Convex set]]"
  - "[[Open Ball]]"
tags:
  - content/definition
---

> [!tip] Relative Interior $\text{relint}(S)$ of set $S$
> is the interior of $S$ relative to its [[Affine hull - aff(S)|affine hull]].
> $$\text{relint}(S) = \{x \in S \mid \exists \varepsilon > 0, \; B(x, \varepsilon) \cap \text{aff}(S) \subseteq S\}$$
> where $B(x, \varepsilon)$ is the [[Open Ball|open ball]] and $\text{aff}(S)$ is the [[Affine hull - aff(S)|affine hull]] of $S$.


## Key Properties

- **Non-empty for convex sets**: Any non-empty [[Convex set|convex set]] has non-empty relative interior
- **Relative to affine hull**: Interior computed within the [[Affine hull - aff(S)|affine hull]], not the entire space
- **Dimension independence**: Works for sets of any dimension within their affine hull
- **Subset relation**: $\text{relint}(S) \subseteq \text{int}(S)$ when $\text{aff}(S) = \mathbb{R}^n$

## Difference between Interior and Relative Interior

![[rel_int.svg]]

**Key distinction**: 
- **[[Interior int(S)|Interior]]** requires neighborhood in the full space $\mathbb{R}^n$
- **Relative interior** only requires neighborhood within the [[Affine hull - aff(S)|affine hull]]

## Examples

### Line Segment in $\mathbb{R}^2$
- Set: $S = \{(t, 0) : t \in [0,1]\}$ (line segment on x-axis)
- **Interior**: $\text{int}(S) = \emptyset$ (no 2D neighborhood exists)
- **Relative interior**: $\text{relint}(S) = \{(t, 0) : t \in (0,1)\}$ (open interval)

### Triangle in $\mathbb{R}^3$
- Set: $S = $ triangle in plane $z = 0$
- **Interior**: $\text{int}(S) = \emptyset$ (no 3D neighborhood)
- **Relative interior**: $\text{relint}(S) = $ interior of triangle within the plane

### Full-dimensional Sets
- When $\text{aff}(S) = \mathbb{R}^n$: $\text{relint}(S) = \text{int}(S)$


# Anki

TARGET DECK: stem::math::optimization
START
math_basic_double
FRONT: Relative Interior $\text{relint}(S)$
BACK: Interior of set $S$ computed within its affine hull, not the entire space
ID: 1755936086713
END

TARGET DECK: stem::math::optimization
START
math_basic_single
FRONT: Interior vs Relative Interior
When do they differ?
BACK: When the set doesn't span the full space - relative interior works within the affine hull
ID: 1755936086715
END

TARGET DECK: stem::math::optimization
START
math_complex
FRONT: Relative Interior Properties
BACK: Interior computed within affine hull rather than full space
FORMULA: $\text{relint}(S) = \{x \in S \mid \exists \varepsilon > 0, \; B(x, \varepsilon) \cap \text{aff}(S) \subseteq S\}$
ADDITIONAL: Every non-empty convex set has non-empty relative interior
PICTURE: ![[rel_int.svg]]
ID: 1755936086717
END
