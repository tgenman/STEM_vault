---
aliases:
  - Попарная независимость
anki: true
created: 2023-12-09 19:01
parent:
  - "[[Independence]]"
connected:
  - "[[Независимость в совокупности]]"
---

> [!tip] $A_1, \ldots , A_k$ попарно независимы
если независимы друг относительно друга любые два события из этого множества.
$P(A \cap B) = P(A)P(B)$.


#### Proof
Пусть в некотором пространстве элементарных исходов $\Omega$ заданы два события $A$ и $B$, причем $B$ не является пустым. Условие того, что событие $A$ не зависит от события $B$, имеет следующий вид:
$$P(A|B) = P(A)$$
Грубо говоря, знание о том, что произошло непустое событие $B$ не даёт никакой новой информации о том, произошло ли событие $A$.

Более удобно (которая не зависит от того, является ли $B$ пустым событием) формулировку условия независимости событий $A$ и $B$ можно получить с помощью теоремы умножения:
$$P(A \cap B) = P(A|B)P(B) = P(A)P(B)$$

Однако, существует более сильное свойство независимости событий — [[Независимость в совокупности]].


# Anki
TARGET DECK: math::probability
START
Math_TWO_side
FRONT: $A_1, \ldots , A_k$ попарно независимы
BACK: если независимы друг относительно друга любые два события из этого множества.
$P(A \cap B) = P(A)P(B)$.
FORMULA: $$P(A|B) = P(A)$$
ADDITIONAL: $$P(A \cap B) = P(A|B)P(B) = P(A)P(B)$$
ID: 1710931451050
END














