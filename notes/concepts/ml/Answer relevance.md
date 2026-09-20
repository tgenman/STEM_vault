---
aliases:
  - "Answer relevancy"
  - "релевантность ответа"
anki: true
created: "2026-09-20"
parent:
  - "[[LLM evaluation]]"
connected:
  - "[[Faithfulness]]"
  - "[[Rubric]]"
  - "[[LLM-as-a-Judge]]"
tags:
  - контент/определение
---

> [!tip] answer relevance / relevancy
> **Answer relevance** — соответствие ответа заданному вопросу.

## пример шкалы

- **1** — ответ не по существу вопроса.
- **5** — ответ точно отвечает на вопрос.

Шкалу задаёт [[Rubric]]. Оценка [[LLM-as-a-Judge]] по шкале 1–5 — один из способов измерения критерия.

В отличие от [[Faithfulness]], relevance проверяет соответствие вопросу, а не подтверждённость контекстом.

## источник

«LLM-as-a-Judge, бенчмаркинг, гардрейлы», разделы 3.3, 5.2 и 5.3.

## Anki

TARGET DECK: stem::ml::engineering

START
math_basic_single
FRONT: Что оценивает answer relevance?
BACK: Насколько ответ отвечает на заданный вопрос.
ID: 1789916214926
END

START
math_basic_single
FRONT: Какие крайние якоря заданы для relevance в judge-промпте урока?
BACK: 1 — ответ не по существу вопроса; 5 — ответ точно отвечает на вопрос.
ID: 1789916214927
END
