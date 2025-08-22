---
aliases:
  - Формула Байеса
  - Bayes’ Theorem
anki: true
created: 2023-12-09 19:23
parent:
  - "[[Conditional Probability]]"
connected:
  - "[[Total Probability Theorem]]"
  - "[[Возможные миры]]"
tags:
  - content/theorem
---

> [!tip] Bayes' Rule
Вероятность $P(A_i|B)$ события $A_i$ при условии, что событие $B$ произошло:
$P(A_i|B) = \frac{P(B|A_i)P(A_i)}{\sum_{j=1}^{k} P(B|A_j)P(A_j)}.$

$P(A_i)$ - initial beliefs [[Prior probability]]
$P(B|A_i)$ - prior [[Свидетельство]]
$P(A_i|B)$ - revised beliefs [[Апостериорная вероятность]]

![[Pasted image 20240320170930.png|300]]


#### Proof
Если применить теорему умножения вероятностей разными способами:

$$ P(A \cap B_i) = P(A|B_i)P(B_i) = P(B_i|A)P(A), $$

то с учетом формулы полной вероятности можно получить требуемое выражение:

$$ P(B_i|A) = \frac{P(A|B_i)P(B_i)}{P(A)} = \frac{P(A|B_i)P(B_i)}{\sum_{j=1}^{k} P(A|B_j)P(B_j)}. $$

Утверждение доказано.

#### Example
Пример. Студент решает задачу с к вариантами ответа. Если студент знает, как решать задачу, он дает правильный ответ. Если нет — может угадать с вероятностью $\frac{1}{k}$. Какая вероятность того, что студент знает решение задачи, при условии, что был дан правильный ответ. Пусть $p \in [0,1]$ — вероятность, что студент знает решение задачи. Событие $B_1$ соответствует ситуации, в которой студент знает решение задачи, а $B_2$ — не знает. Тогда:

$$ P(B_1) = p, \quad P(B_2) = 1 - p, \quad P(A|B_1) = 1, \quad P(A|B_2) = \frac{1}{k}. $$

Теперь можно применить формулу Байеса:

$$ P(B_1|A) = \frac{p}{p + \frac{1}{k}(1 - p)}. $$

# Anki
TARGET DECK: math::probability  
START
Math_TWO_side
FRONT: Bayes' Rule
BACK: Вероятность $P(A_i|B)$ события $A_i$ при условии, что событие $B$ произошло:
$P(A_i|B) = \frac{P(B|A_i)P(A_i)}{\sum_{j=1}^{k} P(B|A_j)P(A_j)}.$
$P(A_i)$ - initial beliefs [[Prior probability]]
$P(B|A_i)$ - prior [[Свидетельство]]
$P(A_i|B)$ - revised beliefs [[Апостериорная вероятность]]
FORMULA: Если применить теорему умножения вероятностей разными способами:
$P(A \cap B_i) = P(A|B_i)P(B_i) = P(B_i|A)P(A)$
то с учетом формулы полной вероятности можно получить требуемое выражение:
$P(B_i|A) = \frac{P(A|B_i)P(B_i)}{P(A)} = \frac{P(A|B_i)P(B_i)}{\sum_{j=1}^{k} P(A|B_j)P(B_j)}$
ADDITIONAL: ![[Pasted image 20240320170930.png]]
ID: 1702152670494
END







