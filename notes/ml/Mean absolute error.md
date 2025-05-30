---
aliases:
  - MAE
anki: false
created: 2024-06-19 13:30
parent:
  - "[[Loss function]]"
connected:
  - "#обс/linking"
tags:
  - empty
---
Появляется при замене [[Euclidian norm (L2)]]  нормы в [[Mean squared error|MSE]] на [[Manhattan norm (L1)]] :

$$ \text{MAE}(y, \hat{y}) = \frac{1}{N} \sum_{i=1}^{N} | y_{i} - \hat{y}_{i} | $$

Можно заметить, что в MAE по сравнению с MSE существенно меньший вклад в ошибку будут вносить примеры, сильно удалённые от ответов модели. Дело тут в том, что в MAE мы считаем модуль расстояния, а не квадрат, соответственно, вклад больших ошибок в MSE получается существенно больше. Такая функция потерь уместна в случаях, когда вы пытаетесь обучить регрессию на данных с большим количеством выбросов в таргете.

Иначе на эту разницу можно посмотреть так: [[Mean squared error|MSE]] приближает [[Expected Value E(X)]]  условного распределения $y \mid x$, а MAE — [[Median|медиану]].
