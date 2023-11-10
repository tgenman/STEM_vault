---
aliases: 
publish: true
anki: true
created: 2023-11-04 22:05
parent:
  - "[[Degree Sequence]]"
connected:
  - "[[2-switch]]"
  - "[[Theorem about 2-switches transformations of graphical sequence]]"
tags:
  - theorem
---

> [!note] Theorem about 2-switches transformations of degree sequence
If ${} G$ and $H$ are two graphs with the same [[Degree Sequence]], then $H$ can be transformed into $G {}$ by a (possibly empty) sequence of [[2-switch]]

### Proof
We proceed by induction on the order ${} n$ of $G$ and $H.$ If $n\leq 4,$ then the result is immediate. For a given integer $n\geq5$, assume that every two graphs of order $n-1$ with the same degree sequence can be transformed into each other by a sequence of 2-switches. Let $s:d_1,d_2,\ldots,d_n$ be a graphical sequence with $\Delta=d_1\geq d_2\geq\cdots\geq d_n$ and let $\mathcal{G}_s$ be the set of all graphs $F$ with degree sequence $s$ such that $V(F)=\{v_1,v_2,\ldots,v_n\}$ where $\deg v_i=d_i$ for $1\leq i\leq n.\quad {}$ Let ${} W= \{ v_2, v_3, \ldots , v_{\Delta+ 1}\} .\quad$ Let ${} G$ and $H$ be two graphs in $\mathcal{G}_s.$ By Theorem $1.10,G$ can be transformed into a graph $G_1\in\mathcal{G}_s$ such that $N_{G_1}(v_1)=W$ and $H$ can be transformed into a graph $H_1\in\mathcal{G}_s$ such that $N_{H_1}(v_1)=W.$ Since $G_1- v_1$ and $H_1- v_1$ are two graphs of order $n-1$ with the same degree sequence, it follows by the induction hypothesis that $G_1-v_1$ can be transformed into $H_1-v_1$ by a sequence of 2-switches. Hence $G_{1}$ can be transformed into $H_{1}$ by a sequence of 2-switches and so $G$ can be transformed into $H$ by a sequence of 2-switches.

### Anki
> [!question]-
START
Math prop
Question_eng: Theorem about 2-switches transformations of degree sequence
Question_rus: 
Answer_eng: If ${} G$ and $H$ are two graphs with the same [[Degree Sequence]], then $H$ can be transformed into $G {}$ by a (possibly empty) sequence of [[2-switch]]
Answer_rus: 
Formula_main: 
Formula_additional: ### Proof
We proceed by induction on the order ${} n$ of $G$ and $H.$ If $n\leq 4,$ then the result is immediate. For a given integer $n\geq5$, assume that every two graphs of order $n-1$ with the same degree sequence can be transformed into each other by a sequence of 2-switches. Let $s:d_1,d_2,\ldots,d_n$ be a graphical sequence with $\Delta=d_1\geq d_2\geq\cdots\geq d_n$ and let $\mathcal{G}_s$ be the set of all graphs $F$ with degree sequence $s$ such that $V(F)=\{v_1,v_2,\ldots,v_n\}$ where $\deg v_i=d_i$ for $1\leq i\leq n.\quad {}$ Let ${} W= \{ v_2, v_3, \ldots , v_{\Delta+ 1}\} .\quad$ Let ${} G$ and $H$ be two graphs in $\mathcal{G}_s.$ By Theorem $1.10,G$ can be transformed into a graph $G_1\in\mathcal{G}_s$ such that $N_{G_1}(v_1)=W$ and $H$ can be transformed into a graph $H_1\in\mathcal{G}_s$ such that $N_{H_1}(v_1)=W.$ Since $G_1- v_1$ and $H_1- v_1$ are two graphs of order $n-1$ with the same degree sequence, it follows by the induction hypothesis that $G_1-v_1$ can be transformed into $H_1-v_1$ by a sequence of 2-switches. Hence $G_{1}$ can be transformed into $H_{1}$ by a sequence of 2-switches and so $G$ can be transformed into $H$ by a sequence of 2-switches.
<!--ID: 1699170574046-->
END












