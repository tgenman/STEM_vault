---
aliases:
  - Унарное отношение
anki: true
created: 2024-07-02 19:11
parent:
  - "[[Relation]]"
  - "[[Unary arity]]"
connected:
  - "[[Unary operation]]"
tags: []
---

> [!tip] Unary relation $\mathcal{P}$ on set $\mathcal{A}$
> is a subset $\mathcal{P} \subseteq \mathcal{A}$ that defines a property of individual elements.

# Examples
- **Even numbers**: $\mathcal{P} = \{x \in \mathbb{Z} \mid x \text{ is even}\}$
- **Positive numbers**: $\mathcal{P} = \{x \in \mathbb{R} \mid x > 0\}$
- **Prime numbers**: $\mathcal{P} = \{x \in \mathbb{N} \mid x \text{ is prime}\}$

# Anki
TARGET DECK: stem::math::common

START
math_complex
FRONT: Unary relation
BACK: A subset $\mathcal{P} \subseteq \mathcal{A}$ that defines a property of individual elements
FORMULA: For $x \in \mathcal{A}$: $x \in \mathcal{P}$ or $x \notin \mathcal{P}$
ADDITIONAL: Examples:
- Even numbers: $\{x \in \mathbb{Z} \mid x \text{ is even}\}$
- Positive numbers: $\{x \in \mathbb{R} \mid x > 0\}$
- Prime numbers: $\{x \in \mathbb{N} \mid x \text{ is prime}\}$
ID: 1747745634698
END

START
math_basic_single
FRONT: What's the difference between a unary relation and a unary operation?
BACK: A unary relation defines a property (true/false) for elements, while a unary operation transforms elements within the same set
ID: 1747745634704
END