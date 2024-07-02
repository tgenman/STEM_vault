---
aliases:
  - Полнота
  - True positive rate TPR
publish: true
anki: false
created: 2024-06-18 20:50
parent:
  - "[[Метрика качества]]"
  - "[[Confusion matrix]]"
connected:
  - "[[Precision]]"
tags:
  - empty
---


скольким больным наша модель поставила правильный диагноз.

$Recall = \frac{TP}{TP + FN}$

Хороша для устранения [[False negative]] (ошибка 2го рода) 

![[6_3_c4ba781675.png]]

> [!tip] TPR (true positive rate) 
это полнота, доля положительных объектов, правильно предсказанных положительными:
$TPR = \frac{TP}{P} = \frac{TP}{TP + FN}$

