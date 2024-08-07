---
aliases:
  - Размещение без повторений
  - Расстановки без повторений
publish: true
anki: true
parent:
  - "[[519.101 Combinatorics MOC]]"
connected:
  - "[[Factorial]]"
  - "[[Tuple]]"
  - "[[Arrangements with repetition]]"
created: 2023-10-23 16:47
---

> [!tip] An arrangement without repetition
 is an ordered $n$-[[Tuple|tuple]] $(x_1,..., x_n)$ elements of $A$, where each elements occurs exactly once

$$A_n^k= V_{n, k} = \frac{n!}{(n-k)!} = n \cdot (n-1) \cdot ... \cdot (n - k + 1) = (n)_k$$

#### Example
Например, если из набора из $5$ различных книг (A, B, C, D, E) нужно выбрать и упорядочить $3$ книги, то количество способов сделать это равно 
$A_5^3=\frac{5!}{(5−3)!}=60$


#### Anki
> [!question]- Arrangements without repetition
TARGET DECK: Math::Combinatorics
START
Math_TWO_side
TITLE:  Arrangements without repetition
Размещение без повторений
DESCRIPTION:  is an ordered $n$-[[Tuple|tuple]] $(x_1,..., x_n)$ elements of $A$, where each elements occurs exactly once
FORMULA: $$A_n^k= V_{n, k} = \frac{n!}{(n-k)!} = n \cdot (n-1) \cdot ... \cdot (n - k + 1) = (n)_k$$
ADDITIONAL:
ID: 1698069638670
END

