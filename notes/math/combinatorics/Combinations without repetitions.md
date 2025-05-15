---
aliases:
  - Комбинации без повторений
anki: true
parent:
  - "[[Set (math)]]"
created: 2023-10-23 17:03
connected:
  - "[[Factorial]]"
  - "[[Binomial coefficient]]"
---

> [!tip] Combinations without repetitions
- Не интересует порядок. Интересует только состав.
- Сочетания  - это в точности [[Set (math)|подмножества]]  из $k$ элементов заданного множества из $n$ элементов
- an k-element subset of A. 

$$C_{n}^k = \binom{n}{k} = \frac{A_n^k}{k!} = \frac{n!}{k!(n-k)!}$$

Connected with [[Permutations with repetitions]]
$$C_n^k = P(k, n-k)$$

# Anki
TARGET DECK: math::combinatorics
START
Math_TWO_side
TITLE:  Combinations without repetitions
DESCRIPTION: A ==k-combination== from n elements (n-element set A) is an k-element subset of A. 
- Не интересует порядок. Интересует только состав.
- Сочетания  - это в точности [[Set (math)|подмножества]]  из $k$ элементов заданного множества из $n$ элементов
- an k-element subset of A. 
FORMULA: $$C_{n}^k = \binom{n}{k} = \frac{A_n^k}{k!} = \frac{n!}{k!(n-k)!}$$
ADDITIONAL: Connected with [[Permutations with repetitions]]
$$C_n^k = P(k, n-k)$$
ID: 1698069941441
END
