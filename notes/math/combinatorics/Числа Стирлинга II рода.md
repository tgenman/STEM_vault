---
aliases: 
created: 2024-01-21 16:14
parent:
  - "[[Partition of a set|Разбиение множества]]"
connected:
  - "[[519.101 Combinatorics MOC]]"
  - "[[Bell numbers]]"
---

> [!tip] Числа Стирлинга второго рода $S(n, k)$
Количество всех способов разбить $n$ объектов на $k$ непустых групп
$S_n^m = \frac{1}{m!} \left[ m^n - \binom{m}{1} (m - 1)^n + \ldots + (-1)^k \binom{m}{k} (m - k)^n + \ldots + (-1)^{m-1} \binom{m}{m-1} \right].$


Обозначение: $S(n, k)$ или $\left\{ \begin{matrix} n \\ k \end{matrix} \right\}$

Пример при $n = 3$, $k = 2$:
- $\{a\} \cup \{b,c\}$
- $\{b\} \cup \{a,c\}$
- $\{c\} \cup \{a,b\}$

$S(3,2) = 3$
$S(10,5) = 42525$

# Anki
TARGET DECK: math::combinatorics
START
Math_TWO_side
FRONT: Числа Стирлинга второго рода $S(n, k)$
BACK: Количество всех способов разбить $n$ объектов на $k$ непустых групп
$S_n^m = \frac{1}{m!} \left[ m^n - \binom{m}{1} (m - 1)^n + \ldots + (-1)^k \binom{m}{k} (m - k)^n + \ldots + (-1)^{m-1} \binom{m}{m-1} \right].$
Обозначение: $S_n^k$ или $\left\{ \begin{matrix} n \\ k \end{matrix} \right\}$

Пример при $n = 3$, $k = 2$:
- $\{a\} \cup \{b,c\}$
- $\{b\} \cup \{a,c\}$
- $\{c\} \cup \{a,b\}$

$S(3,2) = 3$
$S(10,5) = 42525$
FORMULA: 
ADDITIONAL:
ID: 1705843330675
END













