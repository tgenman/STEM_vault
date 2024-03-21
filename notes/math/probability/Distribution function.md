---
aliases:
  - Функция распределения
publish: true
anki: false
created: 2023-10-29 20:19
parent:
  - "[[Distribution of r.v.]]"
connected:
  - "[[Function (math)]]"
tags:
  - empty
---

$$
F:\mathbb{R}\to[0,1],\quad F(x)=\mathbb{P}((-\infty,x])
$$

### Properties
1. F is nondecreasing,
2. $\lim_{x\to-\infty}F(x)=0$, $\lim_{x\to\infty}F(x)=1$,
3. F is right-continuous.

### Доказательство
1. $\lim_{x\to-\infty}F(x)=\lim_{x\to-\infty}\mathbb{P}((-\infty,x])$
Т.к. $(-\infty,x]\downarrow\varnothing$, то по теореме о непрерывности вероятностной меры в $0{:}$

$$
\lim_{x\to-\infty}\mathsf{P}(-\infty,~x])=\mathsf{P}(\varnothing)=0.
$$

Далее, по той же теореме о непрерывности вероятностной меры в $0,\lim_{x\to+\infty}F(x)=\lim_{x\to+\infty}\mathbb{P}((-\infty,x])=$

2. Пусть $x\to x_0+0.$ Тогда $(-\infty,x]\downarrow(-\infty,x_0]$ и по теореме о непрерывности вероятностной меры в 0 $\mathbb{P}((-\infty,x])\to\mathbb{P}((\infty,x_0])$

3. Пусть $x>y.$ Тогда $(-\infty,x]\supset(-\infty,y]\Rightarrow\mathbb{P}((-\infty,x])\geq\mathbb{P}(-\infty,y])\Rightarrow F(x)\geq F(y)$

Замечание: Функция распределения не обязательно непрерывна слева, т.к $(-\infty,x]\xrightarrow{x\to x_0-0}(-\infty,x_0)$,а значит $\mathsf{P}((-\infty,\:x])\to\mathsf{P}((-\infty,\:x_0])-\mathsf{P}(\{x_0\})$









