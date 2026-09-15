---
aliases:
  - Размещение без повторений
  - Расстановки без повторений
anki: true
parent:
  - "[[519.101 Combinatorics MOC]]"
connected:
  - "[[Factorial]]"
  - "[[Tuple]]"
  - "[[Arrangements with repetition]]"
created: 2023-10-23 16:47
tags:
---

> [!tip] An arrangement without repetition $A_n^k$
> An arrangement without repetition of $k$ elements from an $n$-element set $A$ is an ordered $k$-[[Tuple|tuple]] $(x_1,\ldots,x_k)$ of pairwise distinct elements of $A$, where $0 \le k \le n$.

$$A_n^k= V_{n, k} = \frac{n!}{(n-k)!} = n \cdot (n-1) \cdot ... \cdot (n - k + 1) = (n)_k$$

# Example
Например, если из набора из $5$ различных книг (A, B, C, D, E) нужно выбрать и упорядочить $3$ книги, то количество способов сделать это равно 
$A_5^3=\frac{5!}{(5−3)!}=60$


# Anki
TARGET DECK: math::combinatorics
START
Math_TWO_side
FRONT:  Arrangements without repetition
Размещение без повторений
BACK: An ordered $k$-[[Tuple|tuple]] $(x_1,\ldots,x_k)$ of pairwise distinct elements chosen from an $n$-element set, where $0 \le k \le n$.
FORMULA: $$A_n^k= V_{n, k} = \frac{n!}{(n-k)!} = n \cdot (n-1) \cdot ... \cdot (n - k + 1) = (n)_k$$
ADDITIONAL:
ID: 1698069638670
END
