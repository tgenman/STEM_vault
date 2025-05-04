---
aliases:
  - Линейность матожидания
anki: true
created: 2024-03-21 12:13
parent:
  - "[[Expected Value E(X)]]"
connected:
  - "[[Linearity]]"
tags:
---

 > [!tip] Linearity of expectation
 $E[aX + b] = aE[X] + b$

###### Proof
$E[Y] = \sum_{x} g(x)p_X(x) = \sum_{x} (ax + b)p_X(x) = a\sum_{x} xp_X(x) + b\sum_{x} p_X(x) = aE[X] + b$

# Anki
> [!question]- Linearity of expectation
TARGET DECK: math::probability
START
Math_ONE_side
TITLE: Linearity of expectation
DESCRIPTION:  $E[aX + b] = aE[X] + b$
FORMULA: 
ADDITIONAL: Proof
$E[Y] = \sum_{x} g(x)p_X(x) = \sum_{x} (ax + b)p_X(x) = a\sum_{x} xp_X(x) + b\sum_{x} p_X(x) = aE[X] + b$
PICTURE:
ID: 1711012599423
END

