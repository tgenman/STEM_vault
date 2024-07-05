---
aliases:
  - MAPE
publish: true
anki: false
created: 2024-06-19 13:35
parent:
  - "[[Loss function]]"
connected:
  - "#обс/linking"
tags:
  - empty
---

Mean absolute percentage error, относительная ошибка.

$$ \text{MAPE}(y, \hat{y}) = \frac{1}{N} \sum_{i=1}^{N} \left| \frac{\hat{y}_{i} - y_{i}}{y_{i}} \right| $$

Часто используется в задачах прогнозирования (например, погоды, загруженности дорог, кассовых сборов фильмов, цен), когда ответы могут быть различными по порядку величины, и при этом мы бы хотели верно угадать порядок, то есть мы не хотим штрафовать модель за предсказание 2000 вместо 1000 в разы сильней, чем за предсказание 2 вместо 1.
