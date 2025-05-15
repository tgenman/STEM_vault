---
aliases:
  - Линия
anki: true
created: 2024-07-03 22:13
tags: 
parent:
  - "[[512.64  Linear algebra MOC]]"
  - "[[514 Geometry MOC]]"
connected:
  - "[[Plane]]"
  - "[[Point]]"
  - "[[Line segment]]"
---

> [!tip] Line
Suppose $x_1, x_2$ are two points in $\mathbb{R^n}$. 
Then the line passing through them is defined as follows:
$x = \theta x_1 + (1 - \theta)x_2, \theta \in \mathbb{R}$

![[line.svg]]
Figure 1: Illustration of a line between two vectors $x_1$ and $x_2$



#### Other forms
###### implicit equation
$\Large x + y = 1$
###### parametric form
$\Large l: \{ (x, y, z) \in R^3 | (x, y, z) = p_0 + t \vec{v}, t \in R \}$
###### Symmetric form
$\large  x = p_{ox} + tv_x$
$\Large l: \{ \frac{x - p_{ox}}{v_x} = \frac{x - p_{oy}}{v_y} = \frac{x - p_{oz}}{v_z} \}$


# Anki
TARGET DECK: math::optimization
START
Math_ONE_side
TITLE: Line (opt def)
DESCRIPTION: Suppose $x_1, x_2$ are two points in $\mathbb{R^n}$. 
Then the line passing through them is defined as follows:
FORMULA: $x = \theta x_1 + (1 - \theta)x_2, \theta \in \mathbb{R}$
ADDITIONAL:
PICTURE: ![[line.svg]]
ID: 1734761672999
END

TARGET DECK: math::optimization
START
Math_ONE_side
TITLE: Line. implicit equation
DESCRIPTION:
FORMULA: $\Large x + y = 1$
ID: 1734761884853
END

TARGET DECK: math::optimization
START
Math_ONE_side
TITLE: Line. parametric form
FORMULA: $\Large l: \{ (x, y, z) \in R^3 | (x, y, z) = p_0 + t \vec{v}, t \in R \}$
ID: 1734761884869
END

TARGET DECK: math::optimization
START
Math_ONE_side
TITLE: Line. Symmetric form
FORMULA: $\large  x = p_{ox} + tv_x$
$\Large l: \{ \frac{x - p_{ox}}{v_x} = \frac{x - p_{oy}}{v_y} = \frac{x - p_{oz}}{v_z} \}$
ID: 1734761884874
END
