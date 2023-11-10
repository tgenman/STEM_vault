---
aliases: Уменьшение размерности (обобщение)
publish: true
---

Собирает конкретные признаки в абстракции более высокого уровня

![[Pasted image 20230503141121.png|300]]
Сегодня используют для:
-   Рекомендательные Системы (★)
-   Красивые визуализации
-   Определение тематики и поиска похожих документов
-   [Анализ фейковых изображений](https://vas3k.blog/blog/390/)
-   Риск-менеджмент

Популярные алгоритмы: 
- [Метод главных компонент](https://ru.wikipedia.org/wiki/%D0%9C%D0%B5%D1%82%D0%BE%D0%B4_%D0%B3%D0%BB%D0%B0%D0%B2%D0%BD%D1%8B%D1%85_%D0%BA%D0%BE%D0%BC%D0%BF%D0%BE%D0%BD%D0%B5%D0%BD%D1%82) (PCA), 
- [Сингулярное разложение](https://ru.wikipedia.org/wiki/%D0%A1%D0%B8%D0%BD%D0%B3%D1%83%D0%BB%D1%8F%D1%80%D0%BD%D0%BE%D0%B5_%D1%80%D0%B0%D0%B7%D0%BB%D0%BE%D0%B6%D0%B5%D0%BD%D0%B8%D0%B5) (SVD), 
- [Латентное размещение Дирихле](https://ru.wikipedia.org/wiki/%D0%9B%D0%B0%D1%82%D0%B5%D0%BD%D1%82%D0%BD%D0%BE%D0%B5_%D1%80%D0%B0%D0%B7%D0%BC%D0%B5%D1%89%D0%B5%D0%BD%D0%B8%D0%B5_%D0%94%D0%B8%D1%80%D0%B8%D1%85%D0%BB%D0%B5) (LDA), 
- [Латентно-семантический анализ](https://ru.wikipedia.org/wiki/%D0%92%D0%B5%D1%80%D0%BE%D1%8F%D1%82%D0%BD%D0%BE%D1%81%D1%82%D0%BD%D1%8B%D0%B9_%D0%BB%D0%B0%D1%82%D0%B5%D0%BD%D1%82%D0%BD%D0%BE-%D1%81%D0%B5%D0%BC%D0%B0%D0%BD%D1%82%D0%B8%D1%87%D0%B5%D1%81%D0%BA%D0%B8%D0%B9_%D0%B0%D0%BD%D0%B0%D0%BB%D0%B8%D0%B7) (LSA, pLSA, GLSA), 
- [t-SNE](https://en.wikipedia.org/wiki/T-distributed_stochastic_neighbor_embedding) (для визуализации)


![[Pasted image 20230503212515.png]]

Инструмент на удивление хорошо подошел для определения тематик текстов (Topic Modelling). Мы смогли абстрагироваться от конкретных слов до уровня смыслов даже без привлечения учителя со списком категорий. Алгоритм назвали [Латентно-семантический анализ](https://habr.com/post/110078/) (LSA), и его идея была в том, что частота появления слова в тексте зависит от его тематики: в научных статьях больше технических терминов, в новостях о политике — имён политиков. Да, мы могли бы просто взять все слова из статей и кластеризовать, как мы делали с ларьками выше, но тогда мы бы потеряли все полезные связи между словами, например, что _батарейка_ и _аккумулятор_, означают одно и то же в разных документах.

Точность такой системы — полное дно, даже не пытайтесь.

Нужно как-то объединить слова и документы в один признак, чтобы не терять эти скрытые (латентные) связи. Отсюда и появилось название метода. Оказалось, что [Сингулярное разложение](https://ru.wikipedia.org/wiki/%D0%A1%D0%B8%D0%BD%D0%B3%D1%83%D0%BB%D1%8F%D1%80%D0%BD%D0%BE%D0%B5_%D1%80%D0%B0%D0%B7%D0%BB%D0%BE%D0%B6%D0%B5%D0%BD%D0%B8%D0%B5) (SVD) легко справляется с этой задачей, выявляя для нас полезные тематические кластеры из слов, которые встречаются вместе.



#### Bookmarks
- [Как уменьшить количество измерений и извлечь из этого пользу](https://habr.com/post/275273/)
- [Алгоритм LSA для поиска похожих документов](https://netpeak.net/ru/blog/algoritm-lsa-dlya-poiska-pohozhih-dokumentov/)
- [Как работают рекомендательные системы](https://habr.com/company/yandex/blog/241455/)


**Connected with:**
- subtype of [[Unsupervised Learning]]



created: 2023-05-03 14:10