---
aliases:
  - Pазме­щение из n элементов по k
publish: true
anki: true
parent:
  - "[[519.101 Combinatorics]]"
created: 2023-10-23 16:47
connected:
  - "[[Factorial]]"
  - "[[Кортеж]]"
  - "[[k-combination from n elements]]"
---
Let $k \leq n$  and $A = \set{a_1,..., a_n}$ be a finite set

An ==arrangement== or ==permutation== of $n$ elements (of the set A) is an ordered n-tuple $(x_1,..., x_n)$ elements of A, where each elements occurs exactly once

A ==k-variation== from n-elements (from n-element set A) is an ==Arrangements== of some of k-element subset of A

### No repetition (число k-размещений без повторений из n объектов) Перестановка:
$$
A_n^k= V_{n, k} = \frac{n!}{(n-k)!} = n \cdot (n-1) \cdot ... \cdot (n - k + 1)
$$
$$
A_n^n = n \cdot (n-1) \cdot ... \cdot 1 = n!
$$
n-размещение без повторений из n объектов называется ==перестановкой==.

### With repetition (число k-размещений c повторениями из n объектов):
если число видов элементов равно $n$, а число мест равно $k$,
$$
\bar{A_n^k} = n \cdot n \cdot ... \cdot n = n^k
$$
$$
\bar{A_n^n} = n \cdot n \cdot ... \cdot n = n^n
$$

### Anki
TARGET DECK: Math::Combinatorics
START
Math def
Title_eng:  k-arrangements from n-elements (No repetition)
Title_rus:  число k-размещений без повторений из n объектов
Description_eng: is an ordered n-tuple $(x_1,..., x_n)$ elements of A, where each elements occurs exactly once
Description_rus:
Formula_main: $$
A_n^k= V_{n, k} = \frac{n!}{(n-k)!} = n \cdot (n-1) \cdot ... \cdot (n - k + 1)
$$
Formula_additional:
<!--ID: 1698069638670-->
END

START
Math def
Title_eng:  k-arrangements from n-elements (With repetition)
Title_rus:  число k-размещений c повторениями из n объектов
Description_eng:  is an ordered n-tuple $(x_1,..., x_n)$ elements of A, where each elements occurs any times
Description_rus:
Formula_main: $$
\bar{A_n^k} = n \cdot n \cdot ... \cdot n = n^k
$$
Formula_additional:
<!--ID: 1698069774907-->
END



