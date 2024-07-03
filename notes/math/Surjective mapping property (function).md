---
aliases:
  - Сурьекция
  - Onto function mapping
publish: true
anki: false
parent:
  - "[[Function (math)]]"
connected:
  - "[[Bijective mapping property (function)]]"
---

> [!tip] A function is surjective
 if its [[Range Ran(f) or Image Im(f)]]  is equal to its  [[Codomain of a function]]/target set.
 every number in the target set is a possible output of the function for some input.
 $\forall y \in Y \; \exists x \in X \; (y = f(x))$

![[Pasted image 20240117211310.png|200]]
![[Pasted image 20240117210559.png|300]]


For example, the function $f : \mathbb{R} \rightarrow \mathbb{R}$ defined by $f(x) = x^3$ is surjective: for every number $y$ in the target set $\mathbb{R}$, there is an input $x$, namely $x = \sqrt[3]{y}$, such that $f(x) = y$. The function $f(x) = x^3$ is surjective since its image is equal to its target set, $\text{Im}(f) = \mathbb{R}$, as shown in Figure 1.17.

On the other hand, the function $f : \mathbb{R} \rightarrow \mathbb{R}$ defined by the equation $f(x) = x^2$ is not surjective since its image is only the nonnegative numbers $\mathbb{R}_+$ and not the whole set of real numbers (see Figure 1.16). The outputs of this function do not include the negative numbers of the target set, because there is no real number $x$ that can be used as an input to obtain a negative output value.

![[Pasted image 20240117211755.png|200]]
For the function $f(x) = x^3$ the image is equal to the target set of the function, $\text{Im}(f) = \mathbb{R}$, therefore the function $f$ is surjective. The function $f$ maps two different inputs $x_1 \neq x_2$ to two different outputs $f(x_1) \neq f(x_2)$, so $f$ is injective. Since $f$ is both injective and surjective, it is a $bijective$ function.






