---
aliases:
  - Полный двупольный граф
publish: true
anki: true
created: 2023-11-03 16:26
parent:
  - "[[Complete graph]]"
  - "[[Bipartite graph]]"
connected:
  - "#обс/linking"
---
> [!tip] A graph ${} G {}$ is complete bipartite
if $V(G) {}$ can be partitioned into two sets $U {}$ and $W {}$ (called partite sets again) so that $uw {}$ is an edge of $G {}$ if and only if $u∈U {}$ and $w∈W$

If $|U| = s {}$ and $|W|=t {}$ , then this complete bipartite graph has 
- order ${} s+t {}$ 
- size ${} st {}$ 
- is denoted by ${} K_{s,t} {}$ (or ${} K_{t,s} {}$).

The complete bipartite graph ${} K_{1,t} {}$ is called a ==star==.
Observe that ${} K_{2,2} = C_4 {}$.
The star ${} K_{1,3} {}$ is sometimes referred to as a ==claw==.

![[Pasted image 20231103163155.png]]


> [!example] Bookmarks
> - [вики](https://ru.wikipedia.org/wiki/%D0%9F%D0%BE%D0%BB%D0%BD%D1%8B%D0%B9_%D0%B4%D0%B2%D1%83%D0%B4%D0%BE%D0%BB%D1%8C%D0%BD%D1%8B%D0%B9_%D0%B3%D1%80%D0%B0%D1%84#:~:text=%D0%9F%D0%BE%D0%BB%D0%BD%D1%8B%D0%B9%20%D0%B4%D0%B2%D1%83%D0%B4%D0%BE%D0%BB%D1%8C%D0%BD%D1%8B%D0%B9%20%D0%B3%D1%80%D0%B0%D1%84%20(%D0%B1%D0%B8%D0%BA%D0%BB%D0%B8%D0%BA%D0%B0)%20%E2%80%94,%D0%B2%D1%81%D0%B5%D0%BC%D0%B8%20%D0%B2%D0%B5%D1%80%D1%88%D0%B8%D0%BD%D0%B0%D0%BC%D0%B8%20%D0%B2%D1%82%D0%BE%D1%80%D0%BE%D0%B9%20%D0%B4%D0%BE%D0%BB%D0%B8%20%D0%B2%D0%B5%D1%80%D1%88%D0%B8%D0%BD.&text=%D0%B0%D0%B2%D1%82%D0%BE%D0%BC%D0%BE%D1%80%D1%84%D0%B8%D0%B7%D0%BC%D1%8B%20%3D&text=%D1%80%D0%B0%D0%B4%D0%B8%D1%83%D1%81%20%3D)


### Anki
> [!question]-
START
Math prop
Question_eng: A graph ${} G {}$ is complete bipartite
Question_rus: 
Answer_eng: if $V(G) {}$ can be partitioned into two sets $U {}$ and $W {}$ (called partite sets again) so that $uw {}$ is an edge of $G {}$ if and only if $u∈U {}$ and $w∈W$
Answer_rus: 
Formula_main: 
Formula_additional: If $|U| = s {}$ and $|W|=t {}$ , then this complete bipartite graph has 
 order ${} s+t$ 
 size $st$ 
 is denoted by $K_{s,t} {}$ (or ${} K_{t,s} {}$).
<!--ID: 1699165908034-->
END


> [!question]-
START
Math prop
Question_eng: Graph named Star
Question_rus: 
Answer_eng: The complete bipartite graph ${} K_{1,t} {}$ 
Answer_rus: 
Formula_main: 
Formula_additional:
<!--ID: 1699165908053-->
END

> [!question]-
START
Math prop
Question_eng: Graph called Claw
Question_rus: 
Answer_eng: The star ${} K_{1,3} {}$
Answer_rus: 
Formula_main: 
Formula_additional:
<!--ID: 1699165908065-->
END