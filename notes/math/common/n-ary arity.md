---
aliases:
  - n-ary
  - n-местность
  - Polyadic
anki: true
created: 2025-05-20 14:50
parent:
  - "[[Arity]]"
connected:
  - "[[Operation on elements of set]]"
  - "[[Relation]]"
tags:
---

> [!tip] n-ary arity
> is a property of a function, operation, or relation that takes n arguments, where n is any non-negative integer.

For a function $f$, if it takes $n$ arguments, we say it has arity $n$ or is n-ary: $f: A^n \to B$ where $A^n = \underbrace{A \times A \times \cdots \times A}_{n \text{ times}}$.

# Types and Examples

## n-ary Operations
An n-ary operation on a set $A$ is a function $f: A^n \to A$ that maps n elements to one element in the same set.

Examples:
- Sum of n numbers: $f(x_1,\ldots,x_n) = \sum_{i=1}^n x_i$
- Product of n numbers: $f(x_1,\ldots,x_n) = \prod_{i=1}^n x_i$
- Maximum of n numbers: $f(x_1,\ldots,x_n) = \max(x_1,\ldots,x_n)$

## n-ary Relations
An n-ary relation on a set $A$ is a subset $R \subseteq A^n$ that defines a relationship between n-tuples of elements.

Examples:
- Ordered n-tuples: $(x_1,\ldots,x_n) \in R \iff x_1 \leq x_2 \leq \cdots \leq x_n$
- Sum to zero: $(x_1,\ldots,x_n) \in R \iff \sum_{i=1}^n x_i = 0$
- All equal: $(x_1,\ldots,x_n) \in R \iff x_1 = x_2 = \cdots = x_n$

# Properties

n-ary operations can have properties:
1. Symmetry: Result unchanged under permutation of arguments
2. Associativity: Various forms of grouping give same result
3. Distributivity over operations of lower arity

n-ary relations can be:
1. Symmetric: Closed under permutations
2. Monotonic: Preserves order in some sense
3. Decomposable into relations of lower arity

# Special Cases
- n = 0: [[Nullary arity]]
- n = 1: [[Unary arity]]
- n = 2: [[Binary arity]]
- n = 3: [[Ternary arity]]

# Anki
TARGET DECK: stem::math::common
> START
math_complex
FRONT: n-ary arity
BACK: A property of a function, operation, or relation that takes n arguments
FORMULA: For a function $f: A^n \to B$ where $A^n = \underbrace{A \times A \times \cdots \times A}_{n \text{ times}}$
ADDITIONAL: Examples:
- Operations: sum $(x_1+\cdots+x_n)$, product $(x_1\cdots x_n)$
- Relations: "all ordered", "sum to zero"
END

> START
math_basic_double
FRONT: What is the arity of function $f(x_1,\ldots,x_n) = \sum_{i=1}^n x_i$?
BACK: n-ary (arity n)
END 