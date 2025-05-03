---
aliases: Формула полной вероятности
anki: true
created: 2023-12-09 19:16
parent:
  - "[[Conditional Probability|Условная вероятность]]"
connected:
  - "[[Bayes' Rule|Формула Байеса]]"
tags:
  - theorem
---

> [!tip] Total Probability Theorem
Let $A_1, \ldots, A_n$ be disjoint events that form a partition of the sample space (each possible outcome is included in exactly one of the events $A_1, \ldots, A_n$) and assume that $P(A_i) > 0$, for all $i$. Then, for any event $B$, we have
$P(B) = P(A_1 \cap B) + \ldots + P(A_n \cap B)$
$= P(A_1)P(B | A_1) + \ldots + P(A_n)P(B | A_n) = \sum_{i=1}^{k} P(A|B_i)P(B_i)$

![[Pasted image 20240320170930.png|300]]

###### Proof
Исходя из свойств вероятности:
$P(A) = P(A \cap B_1) + P(A \cap B_2) + \ldots + P(A \cap B_k)$

Требуемое утверждение может быть получено с помощью теоремы умножения $P(A \cap B_i) = P(A|B_i)P(B_i)$:
$P(A) = P(A \cap B_1) + P(A \cap B_2) + \ldots + P(A \cap B_k) =$
$= P(A|B_1)P(B_1) + P(A|B_2)P(B_2) + \ldots + P(A|B_k)P(B_k)$


###### Example
Определение. Данные при голосовании использовались пары: если в определенную урну положили черный шар, то это значит голос "ПРОТИВ" белый — "ЗА" данного кандидата.

Пример. Пусть даны три урны: в первой из них находится 3 черных и 2 белых шара, во второй — 1 черный и 3 белых. Из первой урны наугад достают два шара и кладут их внутрь второй урны. После этого шары во второй урне тщательно перемешиваются и из нее извлекается 1 шар. Найти вероятность того, что этот шар — белый.

В результате первого вытягивания реализуется одно из трех событий $B_1, B_2, B_3$. Событие $B_1$ состоит в том, что вытащили два черных шара, $B_2$ — в том, что вытащили два черных, $B_3$ — в том, что вытащили один белый и один черный шар.

Согласно классическому определению вероятности:

$$ P(B_1) = \frac{1}{10}, P(B_2) = \frac{3}{10}, P(B_3) = \frac{6}{10}. $$

Из 13 черных шаров были вытащены 2 черных шара, то во второй урне после перемешивания окажутся 5 белых и переработанных 3 черных шара вероятность вытащить белый шар по условию, что произошло событие $B_1$ равно $P(A|B_1) = \frac{5}{8}$. Аналогично можно получить вероятности $P(A|B_2) = \frac{3}{6}$ и $P(A|B_3) = \frac{4}{6}$.

Согласно формуле полной вероятности, искомая вероятность равна

$$ P(A) = \frac{1}{10} \cdot \frac{5}{8} + \frac{3}{10} \cdot \frac{3}{6} + \frac{6}{10} \cdot \frac{4}{6}. $$

#### Anki
> [!question]- Total Probability Theorem
TARGET DECK: Math::Probability
START
Math_ONE_side
TITLE: Total Probability Theorem
DESCRIPTION: Let $A_1, \ldots, A_n$ be disjoint events that form a partition of the sample space (each possible outcome is included in exactly one of the events $A_1, \ldots, A_n$) and assume that $P(A_i) > 0$, for all $i$. Then, for any event $B$, we have
FORMULA: $P(B) = P(A_1 \cap B) + \ldots + P(A_n \cap B)$
$= P(A_1)P(B | A_1) + \ldots + P(A_n)P(B | A_n) = \sum_{i=1}^{k} P(A|B_i)P(B_i)$
ADDITIONAL: ![[Pasted image 20240320170930.png]]
ID: 1702152660415
END












