---
aliases:
  - Наименьшая 𝜎-алгебра
anki: false
created: 2023-10-22 17:47
parent:
  - "[[Special sigma-algebras]]"
connected:
  - "[[Sigma algebra of subsets of sample space]]"
tags:
  - фикс/пусто
---
Пусть $M$ - система подмножеств $\Omega$. 
==Наименьшая $\sigma$-алгебра, порожденная $M$,==  - есть $\mathscr{F}-\sigma$-алгебра, такая что не существует $\sigma$-алгебры, содержащей $M$ и содержащаяся в $\mathscr{F}$ как собственное подмножество. 
Обозначение $\sigma(M).$

### Proof Existence of $\sigma(\Sigma)$
 1. Existence of a $\sigma$-algebra:
 $2^\Omega\supset\Sigma$
 
1. Construction of the minimum $\sigma$-algebra:
$\mathcal{F} _* : = \bigcap _{\mathcal{F} \supseteq \Sigma- \sigma\text{-algebra}}\mathcal{F}$

3. $\mathcal{F}_*$ is $\sigma$-algebra:
$\bullet\Omega\in\mathcal{T}$ for every $\mathcal{F}\Rightarrow\Omega\in\mathcal{F}_*;$ 
$\bullet A\in\mathcal{F}_*\Rightarrow A\in\mathcal{F}$ for every $\mathcal{F}\Rightarrow$
 the same is true for $\overline{A}\Rightarrow\overline{A}\in\mathcal{F}_*$
$\bullet A_1,A_2,\ldots\in\mathcal{F}_*\Rightarrow A_1,A_2,\ldots\in\mathcal{F}$ 
for every $\mathscr{F}\Rightarrow A_1\cup A_2\cup\ldots\in\mathscr{F}$ 
for every $\mathcal{F}\Rightarrow A_1\cup A_2\cup\ldots\in\mathcal{F}_*$

4. $\mathcal{F}_*$ is minimum:


















