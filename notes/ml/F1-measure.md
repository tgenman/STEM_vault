---
aliases:
  - F1-мера
publish: true
anki: false
created: 2024-06-18 21:10
parent:
  - "[[Метрика качества]]"
  - "[[Confusion matrix]]"
connected:
  - "[[Recall]]"
  - "[[Precision]]"
tags:
  - empty
---


Как мы уже отмечали ранее, модели очень удобно сравнивать, когда их качество выражено одним числом. В случае пары Precision-Recall существует популярный способ скомпоновать их в одну метрику - взять их [[Среднее гармоническое|среднее гармоническое]] . 

$$F_1 = \frac{2}{\frac{1}{Recall} + \frac{1}{Precision}} = \frac{2\ Recall \cdot Precision}{Recall + Precision} = \frac{TP}{TP + \frac{FP + FN}{2}}$$


#### $F_\beta$ мера
Стоит иметь в виду, что F1-мера предполагает одинаковую важность Precision и Recall, если одна из этих метрик для вас приоритетнее, то можно воспользоваться : $$F_\beta = (\beta^2 + 1)\ \frac{Recall \cdot Precision}{\beta^2 Recall + Precision}$$
