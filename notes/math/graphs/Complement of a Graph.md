---
aliases: 
publish: true
anki: true
created: 2023-11-03 17:21
parent:
  - "[[519.171.4 Operations on Graphs]]"
connected:
  - "[[Self-complementary graph]]"
  - "[[Complement of Set]]"
---

> [!tip] The complement $\bar{G}$ of a graph G 
is that graph with vertex set $V(G)$ such that two vertices are [[Adjacent in graph|adjacent]] adjacent in $\bar{G}$ if and only if these vertices are not adjacent in $G$.

$$E(\bar{G}) = \binom{V(G)}{2} \text{\\} E(G)$$

Any [[519.175.1 Isomorphic Graphs|isomorphism]] from a graph $G$ to a graph $H$ is also an isomorphism from $\bar{G}$ to $\bar{H}$. 
Consequently, $\bar{G} \not \cong \bar{H}$ if and only if $G \not \cong H$.

If $G$ is a graph of order $n$ and size $m$, then $\bar{G}$ is a graph of order $n$ and size $\binom n2 - m$. 

The complement $K_n$ of the complete graph $K_n$ is the [[Empty graph|empty graph]] of order $n$.

![[Pasted image 20231103173134.png]]



### Anki
> [!question]-
TARGET DECK: Math::Graph
START
Math def
TITLE: The complement $\bar{G}$ of a graph G 
TITLE_rus: 
DESCRIPTION: is that graph with vertex set $V(G)$ such that two vertices are [[Adjacent in graph|adjacent]] adjacent in $\bar{G}$ if and only if these vertices are not adjacent in $G$.
DESCRIPTION_rus: 
Formula_main: ![[Pasted image 20231103173134.png]]
Formula_additional:If $G$ is a graph of order $n$ and size $m$, then $\bar{G}$ is a graph of order $n$ and size $\binom n2 - m$. 
The complement $K_n$ of the complete graph Kn is the [[Empty graph|empty graph]] of order $n$.
<!--ID: 1699132151354-->
END









