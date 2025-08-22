---
aliases:
  - Наибольший общий делитель
  - НОД
  - GCD
anki: false
created: 2024-06-03 10:44
parent:
  - "[[511 Numbers Theory MOC]]"
connected:
  - "[[Least Common Multiple LCM]]"
tags:
  - fix/empty
---

![[Algoritmy_1_896ef556d4.svg]]

[[Алгоритм Евклида]]

```
GCD(a, b):
    while a > 0 and b > 0:
        if a >= b:
            a = a % b
        else:
            b = b % a
    return max(a,b)
```