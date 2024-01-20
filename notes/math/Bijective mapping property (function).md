---
aliases:
  - Биекция
  - Взаимно однозначное отображение
  - Bijection
publish: true
anki: false
parent:
  - "[[Однозначное отображение]]"
  - "[[Function (math)]]"
connected:
  - "[[Injective mapping property (function)]]"
  - "[[Surjective mapping property (function)]]"
  - "[[Равномощность множеств]]"
---

> [!tip] A function is bijective 
if it is both [[Injective mapping property (function)|injective]] and [[Surjective mapping property (function)|surjective]].
 $\forall a \in A \exists b \in B: f(a) = b$ и $\forall b \in B \exists a \in A: f(b) = a$.



A function is bijective if it is both injective and surjective. When a function $f : A \rightarrow B$ has both the injective and surjective properties, it defines a one-to-one correspondence between the numbers of the source set $A$ and the numbers of the target set $B$. This means for every input value $x$, there is exactly one corresponding output value $y$, and for every output value $y$, there is exactly one input value $x$ such that $f(x) = y$. An example of a bijective function is the function $f: \mathbb{R} \rightarrow \mathbb{R}$ defined by $f(x) = x^3$ (see Figure 1.17). For every input $x$ in the source set $\mathbb{R}$, the corresponding output $y$ is given by $y = f(x) = x^3$. For every output value $y$ in the target set $\mathbb{R}$, the corresponding input value $x$ is given by $x = \sqrt[3]{y}$.

A function is not bijective if it lacks one of the required properties. Examples of non-bijective functions are $f(x) = \sqrt{x}$, which is not surjective and $f(x) = x^2$, which is neither injective nor surjective.

Counting solutions

Another way to understand the injective, surjective, and bijective properties of functions is to think about the solutions to the equation $f(x) = b$, where $b$ is a number in the target set $B$. The function $f$ is injective if the equation $f(x) = b$ has at most one solution for every number $b$. The function $f$ is surjective if the equation $f(x) = b$ has at least one solution for every number $b$. If the function $f$ is bijective then it is both injective and surjective, which means the equation $f(x) = b$ has exactly one solution.



