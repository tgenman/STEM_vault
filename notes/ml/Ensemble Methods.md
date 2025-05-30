---
aliases:
  - Ансамблевые методы
created: 2023-05-03 21:44
parent:
  - "[[004.85 Machine Learning (notion)|ML]]"
---

«Куча глупых деревьев учится исправлять ошибки друг друга»

![[Pasted image 20230503214528.png|300]]

Сегодня используют для:
-   Всего, где подходят классические алгоритмы (но работают точнее)
-   Поисковые системы (★)
-   Компьютерное зрение
-   Распознавание объектов

Популярные алгоритмы:
- [[Стейкинг (ансамблевые методы)]]
- [[Беггинг (ансамблевые методы)]]
- [[Бустинг (ансамблевые методы)]] 




Оказывается, если взять несколько не очень эффективных методов обучения и обучить исправлять ошибки друг друга, качество такой системы будет аж сильно выше, чем каждого из методов по отдельности.

Причём даже лучше, когда взятые алгоритмы максимально нестабильны и сильно плавают от входных данных. Поэтому чаще берут Регрессию и Деревья Решений, которым достаточно одной сильной аномалии в данных, чтобы поехала вся модель. А вот Байеса и K-NN не берут никогда — они хоть и тупые, но очень стабильные.







