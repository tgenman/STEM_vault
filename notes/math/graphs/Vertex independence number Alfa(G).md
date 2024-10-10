---
aliases: 
publish: true
anki: false
created: 2024-09-13 18:40
parent:
  - "[[519.173.5 Числовые характеристики графов]]"
  - "[[Vertex independence set]]"
connected:
  - "[[Clique number ω(G)]]"
  - "[[Edge independence number Alfa`(G)]]"
tags:
  - empty
---

Есть граф $G=(V,E)$ и есть множество вершин графа $W\subseteq V$. Никакие две вершины не соединены ребром. 
$$\forall x,y \in W \ (x,y) \notin E$$
Такое множество вершин $W$ называется независимым [[Vertex independence set]].


$$\alpha(G):= \max \{k:\exists W\subseteq V:|W|=k, W-\text{independent}\}$$
Это число $\alpha$ называется числом независимости графа.

#### Свойства

 $\alpha(\bar{G}) = \omega(G)$  [[Clique number ω(G)]]
$\alpha(G) = \omega(\bar{G})$