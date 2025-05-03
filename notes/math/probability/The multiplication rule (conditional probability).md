---
aliases: 
anki: true
created: 2024-03-20 16:56
parent:
  - "[[Conditional Probability]]"
connected: 
tags: []
---

> [!tip] Multiplication Rule
Assuming that all of the conditioning events have positive probability, we have
$P\left(\bigcap_{i=1}^{n} A_i\right) = P(A_1)P(A_2 | A_1)P(A_3 | A_1 \cap A_2) \cdots P\left(A_n | \bigcap_{i=1}^{n-1} A_i\right)$

![[Pasted image 20240320165827.png]]

$P(A | B) = \frac{P(A \cap B)}{P(B)}$

$P(A \cap B) = P(B) P(A | B)= P(A) P(B | A)$

$P(A^c \cap B \cap C^c) = P(A^c \cap B) P(C^c | A^c \cap B)= P(A^c) P(B | A^c) P(C^c | A^c \cap B)$

$P(A_1 \cap A_2 \cap \ldots \cap A_n) = P(A_1) \prod_{i=2}^{n} P(A_i | A_1, \ldots, A_{i-1})$

#### Anki
> [!question]- The multiplication rule (conditional probability)
TARGET DECK: Math::Probability 
START
Math_ONE_side
TITLE: The multiplication rule (conditional probability)
DESCRIPTION: 
Assuming that all of the conditioning events have positive probability, we have
$P\left(\bigcap_{i=1}^{n} A_i\right) = P(A_1)P(A_2 | A_1)P(A_3 | A_1 \cap A_2) \cdots P\left(A_n | \bigcap_{i=1}^{n-1} A_i\right)$
FORMULA: 
ADDITIONAL: 
$P(A | B) = \frac{P(A \cap B)}{P(B)}$
$P(A \cap B) = P(B) P(A | B)= P(A) P(B | A)$
$P(A^c \cap B \cap C^c) = P(A^c \cap B) P(C^c | A^c \cap B)= P(A^c) P(B | A^c) P(C^c | A^c \cap B)$
$P(A_1 \cap A_2 \cap \ldots \cap A_n) = P(A_1) \prod_{i=2}^{n} P(A_i | A_1, \ldots, A_{i-1})$
PICTURE: ![[Pasted image 20240320165827.png]]
ID: 1710943695679
END