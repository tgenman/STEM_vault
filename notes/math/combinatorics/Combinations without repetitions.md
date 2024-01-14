---
aliases:
  - Комбинации без повторений
publish: true
anki: false
parent:
  - "[[Set (math)]]"
created: 2023-10-23 17:03
connected:
  - "[[Factorial]]"
  - "[[Binomial coefficient]]"
---

> [!tip] Combinations without repetitions
> - Не интересует порядок. Интересует только состав.
> - Сочетания  - это в точности [[Set (math)|подмножества]]  из $k$ элементов заданного множества из $n$ элементов
> - an k-element subset of A. 

$$C_{n}^k = \binom{n}{k} = \frac{A_n^k}{k!} = \frac{n!}{k!(n-k)!}$$

Connected with [[Permutations with repetitions]]
$$C_n^k = P(k, n-k)$$

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
