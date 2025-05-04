---
aliases: 
parent:
  - "[[Irregular graph]]"
connected: 
tags:
  - theorem
---

> [!note] 
For every integer n ≥ 2, there are exactly two nearly irregular graphs of order n.


### Proof
First, observe that if $G$ is a nearly irregular graph of order $n$, then $G$ cannot contain a vertex of degree $0$ and a vertex of degree $n - 1$. Thus, either each vertex of $G$ has one of the degrees $0, 1, \ldots, n - 2$ or each vertex of $G$ has one of the degrees $1, 2, \ldots, n - 1$. Furthermore, if $G$ is nearly irregular, then so is $\overline{G}$.

We show by induction that for each integer $n \geq 2$ there are exactly two nearly irregular graphs of order $n$. Since $K_2$ and $\overline{K}_2$ are nearly irregular, the result holds for $n = 2$. Assume for an integer $n \geq 3$ that there are exactly two nearly irregular graphs of order $n - 1$. Necessarily, one of these graphs is a graph $F$ with $\Delta(F) = n - 2$ and $\delta(F) = 1$ while the other is $F$ where $\Delta(F) = n - 3$ and $\delta(F) = 0$. Then $H = F + K_1$ and $H$ are nearly irregular graphs of order $n$, where $\Delta(H) = n - 2$ and $\delta(H) = 0$. We claim that these are the only nearly irregular graphs of order n. Assume, to the contrary, that there is a third graph $G$ of order $n$ that is nearly irregular. Then either $\Delta(G) = n - 1$ or $\delta(G) = 0$, say the latter. Then $G = G_1 + K_1$, where $G_1$ is the nearly irregular graph of order $n - 1$ with $\Delta(G_1) = n - 2$. However then, $G_1 \cong H$, which is a contradiction. □

#### Anki
> [!question]-
TARGET DECK: math::graph
START
Math_ONE_side
TITLE: Theorem of existence eaxctly 2 nearly irregular graphs
DESCRIPTION: For every integer $n ≥ 2$, there are exactly two nearly irregular graphs of order $n$.
FORMULA: ### Proof
First, observe that if $G$ is a nearly irregular graph of order $n$, then $G$ cannot contain a vertex of degree $0$ and a vertex of degree $n - 1$. Thus, either each vertex of $G$ has one of the degrees $0, 1, \ldots, n - 2$ or each vertex of $G$ has one of the degrees $1, 2, \ldots, n - 1$. Furthermore, if $G$ is nearly irregular, then so is $\overline{G}$.

We show by induction that for each integer $n \geq 2$ there are exactly two nearly irregular graphs of order $n$. Since $K_2$ and $\overline{K}_2$ are nearly irregular, the result holds for $n = 2$. Assume for an integer $n \geq 3$ that there are exactly two nearly irregular graphs of order $n - 1$. Necessarily, one of these graphs is a graph $F$ with $\Delta(F) = n - 2$ and $\delta(F) = 1$ while the other is $F$ where $\Delta(F) = n - 3$ and $\delta(F) = 0$. Then $H = F + K_1$ and $H$ are nearly irregular graphs of order $n$, where $\Delta(H) = n - 2$ and $\delta(H) = 0$. We claim that these are the only nearly irregular graphs of order n. Assume, to the contrary, that there is a third graph $G$ of order $n$ that is nearly irregular. Then either $\Delta(G) = n - 1$ or $\delta(G) = 0$, say the latter. Then $G = G_1 + K_1$, where $G_1$ is the nearly irregular graph of order $n - 1$ with $\Delta(G_1) = n - 2$. However then, $G_1 \cong H$, which is a contradiction. □
ADDITIONAL:
ID: 1706032218641
END






