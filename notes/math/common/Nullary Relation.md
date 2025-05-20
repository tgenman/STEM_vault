---
aliases:
  - Нульарное отношение
anki: true
created: 2025-05-20 14:47
parent:
  - "[[Nullary arity]]"
  - "[[Relation]]"
connected:
  - "[[Nullary Operation]]"
tags: []
---

> [!tip] Nullary relation on set $\mathcal{A}$
> is a property of the entire set $\mathcal{A}$ that evaluates to either true or false.

A **nullary relation** on a set $\mathcal{A}$ is a relation that takes no arguments and represents a property of the entire set. It can be viewed as a function $f: \{\emptyset\} \to \{\text{true}, \text{false}\}$ that evaluates whether the set as a whole has a certain property.

# Examples
- "Set $\mathcal{A}$ is non-empty": $\exists x \in \mathcal{A}$
- "Set $\mathcal{A}$ is finite": $|\mathcal{A}| < \aleph_0$
- "Set $\mathcal{A}$ is countable": $|\mathcal{A}| \leq |\mathbb{N}|$
- "Set $\mathcal{A}$ is closed under an operation": $\forall x,y \in \mathcal{A}: x * y \in \mathcal{A}$

# Properties
1. A nullary relation is deterministic - it always returns the same truth value for a given set
2. It can be viewed as a special case of an n-ary relation where n = 0
3. Often used in mathematical logic and set theory to describe global properties of sets

# Anki
TARGET DECK: stem::math::common
START
math_complex
FRONT: Nullary relation
BACK: A relation that takes no arguments and represents a property of the entire set, evaluating to either true or false
FORMULA: $f: \{\emptyset\} \to \{\text{true}, \text{false}\}$
ADDITIONAL: Examples:
- "Set is non-empty": $\exists x \in \mathcal{A}$
- "Set is finite": $|\mathcal{A}| < \aleph_0$
- "Set is countable": $|\mathcal{A}| \leq |\mathbb{N}|$
ID: 1747745634710
END

START
math_basic_single
FRONT: What type of relation evaluates a property of an entire set without taking any arguments?
BACK: Nullary relation
ID: 1747745634715
END
