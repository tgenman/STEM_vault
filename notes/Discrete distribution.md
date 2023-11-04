---
aliases: 
publish: true
anki: false
created: 2023-10-29 20:38
parent:
  - "[[Distribution in R]]"
connected:
  - "#обс/linking"
tags:
  - empty
---
- $X=\{x_1,x_2,\ldots\}\subset\mathbb{R}-$ finite or countably infinite
-  $\mathbb{P}(\{x_k\})=p_k>0$ for all $k$, $\mathbb{P}(X)=1$ P - discrete distribution

Последовательность $\{p_n\}_{n\in\mathbb{N}}$ называется дискретным распредением вероятностей на (не более чем счетном) множестве $X$, если $p_k= \mathbb{P} ( \{ x_k\} ) , X= \{ x_k, k\in \mathbb{N} \} ,$ $\sum_kp_k=1.$

Иными словами, в дискретном случае вся вероятность сосредоточена не более чем в счетном числе точек. Найдем функцию распределения дискретного распределения вероятностей $\{p_n\}_{n\in\mathbb{N}}.$ Пусть $x\in\mathbb{R}.$ Пусть, кроме того, $k\in\mathbb{N}-$ такое число, что $x\in[x_{k-1},x_k)$, где $x_0=-\infty.$ Тогда

$$
F(x)=\mathsf{P}((-\infty,x])=\sum_{i<k}\mathsf{P}(\{x_i\})+\mathsf{P}((-\infty,x]\backslash\{x_i,i<k\})=\sum_{i<k}p_i.
$$















