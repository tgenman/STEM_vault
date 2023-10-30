---
aliases:
  - Линейное преобразование
publish: true
anki: false
created: 2023-10-30 20:25
parent:
  - "[[512.64  Linear algebra MOC]]"
connected:
  - "[[Матрица линейного преобразования]]"
---
#### Определение
> [!Линейное преобразование]
> [[Bijective mapping property|Отображение]] $A: V \rightarrow V$ является **линейным преобразованием** [[Vector space V|векторного пространства]], если для любых векторов $\vec{x}{,}\ \vec{y}$  этого пространства и числа $n$ верно:
> 1) $A(\vec{x}+\vec{y})=A(\vec{x}) + A(\vec{y})$;
> 2) $A(n\cdot\vec{x})=n\cdot A(\vec{x})$.

#### Аксиоматика
$$
\begin{aligned}
&\text{Отображение }A(\vec{x})=3\cdot\vec{x}\text{ является линейным преобразованием, так как:} \\
&\text{1)}3(\vec{x}+\vec{y})=3\vec{x}+3\vec{y}; \\
&\text{2)}3(n\cdot\vec{x})=3n\cdot\vec{x}.
\end{aligned}
$$

$$\begin{aligned}&\text{А вот отображение }A(\vec{x})=\vec{x}+5\text{ линейным преобразованием не является};\\&\text{ا》}(\vec{x}+\vec{y})+5\neq(\vec{x}+5)+(\vec{y}+5)=(\vec{x}+\vec{y})+10;\\&\text{2)}(n\vec{x})+5\neq n(\vec{x}+5)=n\vec{x}+5n.\end{aligned}$$



















