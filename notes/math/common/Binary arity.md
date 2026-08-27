---
aliases:
  - Binary
  - Двухместность
anki: true
created: 2025-05-20 14:30
parent:
  - "[[Arity]]"
connected:
  - "[[Binary operation]]"
  - "[[Binary relation]]"
  - "[[Function (math)]]"
tags: []
---

> [!tip] Binary arity
> is a property of a function, operation, or relation that takes exactly two arguments.

For a function $f$, if it takes two arguments, we say it has arity 2 or is binary: $f: A \times A \to B$.

# Types and Examples

## Binary Operations
A binary operation on a set $A$ is a function $f: A \times A \to A$ that maps two elements to one element in the same set.

Examples:
- Addition: $+: \mathbb{R} \times \mathbb{R} \to \mathbb{R}$, where $(x,y) \mapsto x + y$
- Multiplication: $\cdot: \mathbb{R} \times \mathbb{R} \to \mathbb{R}$, where $(x,y) \mapsto x \cdot y$
- Maximum: $\max: \mathbb{R} \times \mathbb{R} \to \mathbb{R}$, where $(x,y) \mapsto \max(x,y)$

## Binary Relations
A binary relation on a set $A$ is a subset $R \subseteq A \times A$ that defines a relationship between pairs of elements.

Examples:
- Equality: $(x,y) \in R \iff x = y$
- Less than: $(x,y) \in R \iff x < y$
- Divisibility: $(x,y) \in R \iff x \text{ divides } y$

# Properties

Binary operations often have important properties:
1. [[Commutative identity]]: $f(a,b) = f(b,a)$
2. [[Associative identity]]: $f(f(a,b),c) = f(a,f(b,c))$
3. [[Identity element]]: $\exists e: f(a,e) = f(e,a) = a$
4. [[Inverse element]]: $\exists b: f(a,b) = f(b,a) = e$

Binary relations can have properties:
1. [[Reflexive]]: $(a,a) \in R$
2. [[Symmetry]]: $(a,b) \in R \implies (b,a) \in R$
3. [[Transitive]]: $(a,b) \in R \land (b,c) \in R \implies (a,c) \in R$

# Anki
TARGET DECK: stem::math::common
> START
math_complex
FRONT: Binary arity
BACK: A property of a function, operation, or relation that takes exactly two arguments
FORMULA: For a function $f: A \times A \to B$
ADDITIONAL: Examples:
- Operations: addition $(x+y)$, multiplication $(x \cdot y)$
- Relations: equality $(x=y)$, less than $(x<y)$
END

> START
math_basic_double
FRONT: What is the arity of function $f(x,y) = x + y$?
BACK: Binary (arity 2)
END 