---
aliases:
  - "MinHash signature"
anki: false
created: "2026-09-20"
parent:
  - "[[дедупликация документов]]"
connected:
  - "[[Shingling]]"
  - "[[Locality Sensitive Hashing]]"
tags:
  - контент/определение
  - фикс/анки
---
> [!tip] MinHash
> Построение компактного отпечатка документа по шинглам.

Отпечаток создаётся через хеш-функции; похожие документы имеют похожие отпечатки. Шинглами могут служить символьные триграммы ([[Shingling]]), а поиск кандидатов выполняет [[Locality Sensitive Hashing|LSH]].
