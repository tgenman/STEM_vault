---
aliases:
  - Сигма-алгебра подмножеств элементарных исходов
publish: true
anki: false
created: 2023-10-22 14:13
parent:
  - "[[Probability space]]"
  - "[[Algebra of subsets of sample space]]"
connected:
  - "[[Special sigma-algebras]]"
  - "[[512.54 Group Theory MOC]]"
---
по сути является расширением над [[Algebra of subsets of sample space|алгеброй]] $\mathcal{A}$ на [[Infinity set|бесконечных множествах]] 

Система множеств $\mathcal{F}$ называется $\sigma$-algebra , если выполняются следующие 3 свойства ($A$ is [[Event|an event]]  if $A \in \mathcal{F}$ ):
- $\Omega \in \mathcal{F}$ 
- $A \in \mathcal{F} \Rightarrow \bar{A} = \Omega \text{\\} A \in \mathcal{F}$ 
	- $\emptyset\in\mathcal{F}$ т.к. $\bar{\Omega} = \emptyset \in \mathcal{F}$ 
- $A_1, A_2,... \in \mathcal{F} \Rightarrow \bigcup_{i=1}^\infty A_i,\bigcap_{i=1}^\infty A_i\in\mathcal{F}$ 
	- достаточно только одного. Второе выводится через [[Первый закон де Моргана|законы де Моргана]]
	- т.е. замкнута относительно операций $\cap$, $\cup$, (\\ , $\bigtriangleup$ )





