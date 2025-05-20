---
aliases:
  - Ternary
  - Трехместность
anki: true
created: 2025-05-20 14:45
parent:
  - "[[Arity]]"
connected:
  - "[[Ternary operation]]"
  - "[[Ternary relation]]"
  - "[[Function (math)]]"
tags: []
---

> [!tip] Ternary arity
> is a property of a function, operation, or relation that takes exactly three arguments.

For a function $f$, if it takes three arguments, we say it has arity 3 or is ternary: $f: A \times A \times A \to B$.

# Types and Examples

## Ternary Operations
A ternary operation on a set $A$ is a function $f: A \times A \times A \to A$ that maps three elements to one element in the same set.

Examples:
- Conditional operation: $f(c,x,y) = \begin{cases} x & \text{if } c \text{ is true} \\ y & \text{otherwise} \end{cases}$
- Triple sum: $f(x,y,z) = x + y + z$
- Color mixing: RGB color combination $(r,g,b) \mapsto \text{color}$

## Ternary Relations
A ternary relation on a set $A$ is a subset $R \subseteq A \times A \times A$ that defines a relationship between triples of elements.

Examples:
- "Between" relation: $(x,y,z) \in R \iff x < y < z$
- Collinearity of points: $(A,B,C) \in R \iff A,B,C \text{ are collinear}$
- Triangle inequality: $(x,y,z) \in R \iff x + y > z$

# Properties

Ternary operations can have properties:
1. Symmetry in arguments: $f(x,y,z) = f(y,x,z)$ etc.
2. Associativity-like: $f(f(x,y,z),u,v) = f(x,f(y,z,u),v)$
3. Distributivity over binary operations

Ternary relations can be:
1. Cyclic: $(x,y,z) \in R \implies (y,z,x) \in R$
2. Totally symmetric: Any permutation of $(x,y,z) \in R$ is in $R$
3. Transitive-like: Various forms possible

# Anki
TARGET DECK: stem::math::common
> START
math_complex
FRONT: Ternary arity
BACK: A property of a function, operation, or relation that takes exactly three arguments
FORMULA: For a function $f: A \times A \times A \to B$
ADDITIONAL: Examples:
- Operations: conditional $(if,then,else)$, triple sum $(x+y+z)$
- Relations: "between", collinearity
END

> START
math_basic_double
FRONT: What is the arity of function $f(x,y,z) = x + y + z$?
BACK: Ternary (arity 3)
END 