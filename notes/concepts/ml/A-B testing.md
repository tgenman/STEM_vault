---
aliases:
  - "A/B testing"
  - "A/B-тестирование"
  - "online A/B testing"
anki: false
created: "2026-09-20"
parent:
  - "[[LLM evaluation]]"
connected:
  - "[[Evaluation dataset]]"
  - "[[Golden set]]"
  - "[[minimum detectable effect]]"
tags:
  - контент/определение
  - фикс/анки
---

> [!tip] A/B testing
> **A/B testing** — случайное распределение пользователей или запросов между вариантами для сравнения результатов.

## применение

Эксперимент на живом трафике требует достаточной выборки, времени накопления данных и инфраструктуры распределения по вариантам. Проверка на [[Golden set|golden]] / [[Evaluation dataset|eval-сете]] позволяет предварительно выявить регрессии.

Размер выборки связан с [[minimum detectable effect|MDE]]: меньший эффект труднее отличить от шума.

## источник

«LLM-as-a-Judge, бенчмаркинг, гардрейлы», раздел 5.4.
