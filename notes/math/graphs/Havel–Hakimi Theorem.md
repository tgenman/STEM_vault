---
aliases: 
publish: true
anki: false
created: 2023-11-15 13:49
parent:
  - "[[Graphical sequence]]"
connected:
  - "[[Theorem about 2-switches transformations of graphical sequence]]"
tags:
  - theorem
---

#### Definition
> [!note] Havel–Hakimi Theorem
A sequence $s: d_1, d_2, \ldots, d_n$ of nonnegative integers with $\Delta = d_1 \geq d_2 \geq \cdots \geq d_n$ and $\Delta \geq 1$ is graphical if and only if the sequence
$$s_1: d_2 - 1, d_3 - 1, \ldots, d_{\Delta + 1} - 1, d_{\Delta + 2}, \ldots, d_n$$
is [[Graphical sequence|graphical]].


#### Proof
First, assume that $s_1$ is graphical. Then there exists a graph $G_{1}$ of order $n-1$ such that $s_1$ is a degree sequence of $G_1.$ Thus, the vertices of $G_{1}$ can be labeled as $v_2,v_3,\ldots,v_n$ so that

$$
\left.\deg_{G_1}v_i\quad=\quad\left\{\begin{array}{ll}d_i-1&\quad\mathrm{if~}2\leq i\leq\Delta+1\\d_i&\quad\mathrm{if~}\Delta+2\leq i\leq n.\end{array}\right.\right.
$$

A new graph $G$ can now be constructed by adding a new vertex $v_1$ to $G_1$ together with the $\Delta$ edges $v_1v_i$ for $2\leq i\leq\Delta+1.$ Since $\deg_Gv_i=d_i$ for $1\leq i\leq n, $ it follows that $s: \Delta= d_1, d_2, \ldots , d_n$ is a degree sequence of $G$ and so $s$ is graphical.

Conversely, let $s$ be a graphical sequence. By Theorem 1.10, there exists a graph $G$ of order $n$ having degree sequence $s$ with $V(G)=\{v_1,v_2,\ldots,v_n\}$ such that $\deg v_i=d_i$ for all $i\left ( 1\leq i\leq n\right ) $ where $N_G( v_1) = \{ v_2, v_3, \ldots , v_{\Delta+ 1}\} .$ Then $G-v_1$ has degree sequence $s_1.$

#### Illistration of algorithm
$s:5,3,3,3,3,2,2,2,1,1,1.$
After one application of Theorem (deleting $5$ from $s$ and subtracting 1 from the next five terms), we obtain
$s_1^{\prime}:2,2,2,2,1,2,2,1,1,1.$
Reordering this sequence, we have
$s_1:2,2,2,2,2,2,1,1,1,1.$
Continuing in this manner, we get
$s_2^{\prime}:1,1,2,2,2,1,1,1,1$ $s_2:2,2,2,1,1,1,1,1$
$s_3^{\prime}=s_3:1,1,1,1,1,1,1$
$s_4^{\prime}:0,1,1,1,1,1$
$s_4:1,1,1,1,1,1,0$ 
$s_5^{\prime}:0,1,1,1,1,0$ 
$s_5:1,1,1,1,0,0$ 
$s_6^{\prime}:0,1,1,0,0 {}$
$s_6:1,1,0,0,0$ 
$s_7^{\prime}=s_7:0,0,0,0.$

![[Pasted image 20231115140330.png]]

 ![[Pasted image 20231115140410.png]]






