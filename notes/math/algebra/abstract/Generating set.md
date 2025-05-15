---
aliases:
  - Генрирующее множество
  - Порождающее множество
anki: true
created: 2025-05-10 17:26
parent:
  - "[[512.5 General Algebra MOC]]"
connected:
  - "[[Rank of Group]]"
  - "[[Minimal Generating Set]]"
  - "[[Minimum Generating Set]]"
tags:
---

> [!tip] A generating set $S$ of a group $G$ 
is a subset $S \subseteq G$ such that every element $g \in G$ can be expressed as a finite product of elements from $S$ and their inverses. This is denoted as $G = \langle S \rangle$.

# Example of Minimal and Minimum Generating Sets
Consider the group of symmetries of a hexagon:

![[Pasted image 20250510191007.png|150]]
$$ \text{Hex} = \{ 1, r, r^2, r^3, r^4, r^5, f, rf, r^2f, r^3f, r^4f, r^5f \} $$
The set can be divided into:
- [[Rotating transformation|rotations]]: $\{ 1, r, r^2, r^3, r^4, r^5 \}$
- [[Reflecting transformation|reflections]] : $\{ f, rf, r^2f, r^3f, r^4f, r^5f \}$

The generating sets are:
- $\langle r, f \rangle$ is a [[Minimum Generating Set|minimum]] (and hence minimal) generating set.
- $\langle r^2, r^3, f \rangle$ is a [[Minimal Generating Set|minimal]] (but not minimum) generating set.

A generating set $S$ is:
- $\textcolor{blue}{minimal}$ if removing any element makes it no longer generate.
- $\textcolor{red}{minimum}$  if it is minimal and $|S| \leq |T|$ for all other generating sets $T$.

For any generating set $S$ of $G$,
$\textcolor{red}{minimum}  \Rightarrow \textcolor{blue}{minimal}$ but $\textcolor{blue}{minimal} \nRightarrow \textcolor{red}{minimum}$

# Anki
TARGET DECK: stem::math::algebra
START
Math_TWO_side
TITLE: Generating Set
DESCRIPTION: A subset $S \subseteq G$ such that every element $g \in G$ can be expressed as a finite product of elements from $S$ and their inverses. This is denoted as $G = \langle S \rangle$.
FORMULA: $G = \langle S \rangle$
ADDITIONAL:
ID: 1746894805000
END

TARGET DECK: stem::math::algebra
START
Math_ONE_side
TITLE: Example of Minimal vs Minimum Generating Sets: Hexagon Group
DESCRIPTION:The hexagon symmetry group has: 
>- $\langle r, f \rangle$ is a minimum (and hence minimal) generating set.
>- $\langle r^2, r^3, f \rangle$ is a minimal (but not minimum) generating set.
>For any generating set $S$ of $G$,
>$\textcolor{red}{minimum}  \Rightarrow \textcolor{blue}{minimal}$ but $\textcolor{blue}{minimal} \nRightarrow \textcolor{red}{minimum}$
FORMULA: 
ADDITIONAL: A generating set $S$ is:
>- minimal if removing any element makes it no longer generate.
>- minimum if it is minimal and $|S| \leq |T|$ for all other generating sets $T$.
PICTURE: ![[Pasted image 20250510191007.png]]
ID: 1746895007048
END










