---
aliases:
  - Размещение без повторений
  - Расстановки без повторений
publish: true
anki: false
parent:
  - "[[519.101 Combinatorics]]"
connected:
  - "[[Factorial]]"
  - "[[Tuple]]"
  - "[[Arrangements with repetition]]"
created: 2023-10-23 16:47
---

> [!tip] An arrangement without repetition
 is an ordered ${} n$-[[Tuple|tuple]] $(x_1,..., x_n) {}$ elements of $A$, where each elements occurs exactly once

$$A_n^k= V_{n, k} = \frac{n!}{(n-k)!} = n \cdot (n-1) \cdot ... \cdot (n - k + 1)$$

#### Example
Например, если из набора из $5 {}$ различных книг (A, B, C, D, E) нужно выбрать и упорядочить $3 {}$ книги, то количество способов сделать это равно 
$A_5^3=\frac{5!}{(5−3)!}=60 {}$


> [!info]+
> ```dataview 
> TABLE without id
> map(file.outlinks, (link) => "[[" + meta(link).path + "]]") AS "Исходящие",
> map(file.inlinks, (link) => "[[" + meta(link).path + "]]") AS "Входящие"
> WHERE file.name = this.file.name
> ```



#### Anki
TARGET DECK: Math::Combinatorics
START
Math def
Title_eng:  k-arrangements from n-elements (No repetition)
Title_rus:  число k-размещений без повторений из n объектов
Description_eng: is an ordered n-tuple ${} (x_1,..., x_n)$ elements of A, where each elements occurs exactly once
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
