---
aliases:
  - Сочетания
  - Combinations
publish: true
anki: false
parent:
  - "[[519.101 Combinatorics]]"
created: 2023-10-23 17:03
connected:
  - "[[Factorial]]"
  - "[[Binomial coefficient]]"
  - "[[k-arrangements from n-elements]]"
---
Let $k \leq n$  and $A = \set{a_1,..., a_n}$ be a finite set

A ==k-combination== from n elements (n-element set A) is an k-element subset of A. 
No Order

No repetition:
$$
C_{n, k} = \binom{n}{k} = \frac{n!}{k!(n-k)!}
$$
With repetition:
$$
\left(\binom{n}{k} \right) = \binom{n+k-1}{k} = \frac{(n+k-1)!}{k!(n-1)!}
$$



### Anki
TARGET DECK: Math::Combinatorics
START
Math def
Title_eng: k-combination from n elements (no repetition)
Title_rus: 
Description_eng: A ==k-combination== from n elements (n-element set A) is an k-element subset of A. 
Description_rus: 
Formula_main: $$
C_{n, k} = \binom{n}{k} = \frac{n!}{k!(n-k)!}
$$
Formula_additional:
<!--ID: 1698069941441-->
END

START
Math def
Title_eng: k-combination from n elements (with repetition)
Title_rus: 
Description_eng: A ==k-combination== from n elements (n-element set A) is an k-element 
Description_rus: 
Formula_main: $$
\left(\binom{n}{k} \right) = \binom{n+k-1}{k} = \frac{(n+k-1)!}{k!(n-1)!}
$$
Formula_additional:
<!--ID: 1698070674572-->
END
