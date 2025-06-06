---
aliases:
  - Числа Белла
anki: true
created: 2024-01-21 16:14
parent:
  - "[[Partition of a set|Разбиение множества]]"
connected:
  - "[[Числа Стирлинга II рода]]"
  - "[[519.101 Combinatorics MOC]]"
---
> [!tip] Числа Белла
Количество всевозможных способов разбить $n$ объектов на непустые группы: 
$B_n = \sum_{k=1}^n S(n,k)$

Пример при $n = 3$:
- $\{a\} \cup \{b\} \cup \{c\}$
- $\{a\} \cup \{b,c\}$
- $\{b\} \cup \{a,c\}$
- $\{c\} \cup \{a,b\}$
- $\{a, b, c\}$

$B_3 = 5$
$B_{10} = 115975$


# Anki
TARGET DECK: math::combinatorics
START
math_complex
FRONT: Числа Белла
BACK: Количество всевозможных способов разбить $n$ объектов на непустые группы:  
$B_n = \sum_{k=1}^n S(n,k)$
FORMULA: Пример при $n = 3$:
- $\{a\} \cup \{b\} \cup \{c\}$
- $\{a\} \cup \{b,c\}$
- $\{b\} \cup \{a,c\}$
- $\{c\} \cup \{a,b\}$
- $\{a, b, c\}$

$B_3 = 5$
$B_{10} = 115975$
ADDITIONAL:
ID: 1705843070286
END













