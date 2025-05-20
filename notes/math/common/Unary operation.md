---
aliases:
  - Унарная операция
anki: true
created: 2024-01-29 20:22
parent:
  - "[[Operation on elements of set]]"
  - "[[Unary arity]]"
connected:
  - "[[Unary relation]]"
  - "[[Логическая унарная функция]]"
tags: []
---

> [!tip] Unary operation on set $\mathcal{A}$
> is a [[Operation on elements of set|Operation on elements of set]] $f: \mathcal{A} \to \mathcal{A}$ that maps one element to another element in the same set.

A unary operation takes a single element from a set and transforms it into another element of the same set. It is a special case of an [[Operation on elements of set|n-ary operation]] where $n=1$.

# Examples
- [[Negation]] on [[Whole numbers Z (zahlen)|Integers]] integers $\mathbb{Z}$: $-: \mathbb{Z} \to \mathbb{Z}$, where $x \mapsto -x$
- **Absolute value**: $|\cdot|: \mathbb{Z} \to \mathbb{N}$, where $x \mapsto |x|$
- **Square**: $(\cdot)^2: \mathbb{R} \to \mathbb{R}$, where $x \mapsto x^2$
- [[Logical negation]] : $\neg: \{0,1\} \to \{0,1\}$, where $x \mapsto \neg x$

# Properties
- **[[Idempotence]]**: Operation $f$ is idempotent if $f(f(a)) = f(a)$ for all $a \in \mathcal{A}$
- **[[Involution]]**: Operation $f$ is an involution if $f(f(a)) = a$ for all $a \in \mathcal{A}$
- Can be [[Function composition|composed]]: If $f$ and $g$ are unary operations, then $g \circ f$ is also a unary operation

# Anki
TARGET DECK: stem::math::common
START
math_complex
FRONT: Unary Operation (def)
BACK: A function $f: \mathcal{A} \to \mathcal{A}$ that maps one element to another element in the same set
FORMULA: For $x \in \mathcal{A}$, $f(x) \in \mathcal{A}$
ADDITIONAL: 
Examples:
- Negation: $-x$ on $\mathbb{Z}$
- Absolute value: $|x|$ on $\mathbb{Z}$
- Square: $x^2$ on $\mathbb{R}$
ID: 1747745634680
END

START
math_basic_single
FRONT: What is a unary operation on set $\mathcal{A}$?
BACK: A function $f: \mathcal{A} \to \mathcal{A}$ that maps one element to another element in the same set
ID: 1747745634685
END

START
math_basic_single
FRONT: Unary Operation (prop)
BACK: 
1. Idempotence: $f(f(a)) = f(a)$ for all $a \in \mathcal{A}$
2. Involution: $f(f(a)) = a$ for all $a \in \mathcal{A}$
3. Composition: If $f$ and $g$ are unary operations, then $g \circ f$ is also a unary operation
ID: 1747745634691
END











