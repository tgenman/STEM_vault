---
aliases:
  - Геометрическая вероятность
anki: false
created: 2023-10-22 16:43
parent:
  - "[[Probability]]"
connected: 
tags:
  - content/empty
---
$\mu-$ the [[517.518.112 Lebesgue measure]] on $R^n$ 
$\mathcal{B} ( R^n) : = \sigma( B_1 \times ... \times B_n, B_i\in \mathcal{B} ( R) )$ - [[517.518.113 Borel sigma-algebra]]

$\Omega\in\mathcal{B}(R^n)$ such that $\mu(\Omega)<\infty$
$\mathcal{F}=\mathcal{B}(R^n)\cap\Omega$
 $\mathbb{P}(\mathbb{A})=\frac{\mu(A)}{\mu(\Omega)}$
 


### Пример
Рассмотрим следующую задачу: Петя и Ваня приходят в столовую с 12 до 13 часов. Если Петя пришел раньше Вани, то он ждет его 15 минут и уходит. Аналогично поступает Ваня. Нужно найти вероятность того, что Петя и Ваня встретятся в столовой.

Пространство элементарных исходов составляет $\Omega=[0,1]\times[0,1]=[0,1]^2$, а событие $A=\{\Pi$ и В встретились} $\}=$ $\{(u,v):|u-v|\leq\frac14\}.$ Это множество на рисунке выделено красным цветом. Тогда

$$
\mathsf{P}(A)=\frac{\mu(A)}{\mu(\Omega)}=\frac{1-2\cdot\frac12\cdot\left(\frac34\right)^2}1=\frac7{16}
$$
![[Pasted image 20231022173713.png|300]]














