---
aliases: 
publish: true
anki: false
created: 2023-11-05 15:04
parent:
  - "[[Surjective mapping property (function)]]"
connected:
  - "[[Number of Surjections]]"
---
Consider $X=\{x_1,\ldots,x_l\}$, $Y=\{y_1,\ldots,y_n\}$
How many surjections are there from$X$  to $Y?$ 

if
- $l < n$ - $S(x, y) = 0$
- $l = n$ - $S(x, y) = n!$
- $l > n$ - $S(x, y) = \sum_{k=0}^n(-1)^k\binom{n}k\cdot(n-k)^l$ 

### Proof
Let $U$ be the set of all the mappings
from $X$ to $Y,A_i$ 一 mappings $f$ such that $y_i\not\in\operatorname{Im}f.$
The number of surjections is equal to $|\overline{A_1}\cap\ldots\cap\overline{A_n}|$

$|\overline{A_1}\cap\ldots\cap\overline{A_n}| =|U|-\sum_i|A_i|+ \sum_{i,j}|A_i \cap A_j|\cdots$
If $S\subset\{1,\ldots,n\}$  Iet  $M=\cap_{j\in S}A_j$
$M$ is the set of mappings $f$ with $f(X)\cap M=\emptyset.$
There are exactly $(n-|S|)^l$  such mappings.
Hence $\sum_{S\subset\{1,...,n\},|S|=k}|\cap_{j\in S}A_j|= \binom{n}{k}\cdot(n-k)^{l}$

The answer is $\left|U\right| - \sum_i \left|A_i\right| + \sum_{k=0}^n (-1)^k \binom{n}{k} \cdot (n-k)^l$.












