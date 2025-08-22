---
aliases:
  - Линейное преобразование
created: 2024-07-03 22:15
parent:
  - "[[512.64  Linear algebra MOC]]"
connected:
  - "[[Матрица линейного преобразования]]"
  - "#обс/linking"
tags:
  - fix/empty
anki: false
---


> [!Линейное преобразование]
> [[Bijective mapping property (function)|Отображение]] $A: V \rightarrow V$ является **линейным преобразованием** [[Vector space V|векторного пространства]], если для любых векторов $\vec{x}{,}\ \vec{y}$  этого пространства и числа $n$ верно:
> 1) $A(\vec{x}+\vec{y})=A(\vec{x}) + A(\vec{y})$;
> 2) $A(n\cdot\vec{x})=n\cdot A(\vec{x})$.

#### Аксиоматика
Отображение $A(\vec{x}) = 3 \cdot \vec{x}$ является линейным преобразованием, так как:  
1) $3(\vec{x} + \vec{y}) = 3\vec{x} + 3\vec{y}$;  
2) $3(n \cdot \vec{x}) = 3n \cdot \vec{x}$.

А вот отображение $A(\vec{x}) = \vec{x} + 5$ линейным преобразованием не является:  
1) $(\vec{x} + \vec{y}) + 5 \neq (\vec{x} + 5) + (\vec{y} + 5) = (\vec{x} + \vec{y}) + 10$;  
2) $(n\vec{x}) + 5 \neq n(\vec{x} + 5) = n\vec{x} + 5n$.




















