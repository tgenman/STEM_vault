---
aliases:
anki: true
created: "2026-09-20"
parent:
  - "[[LLM-as-a-Judge]]"
connected:
  - "[[Rubric]]"
tags:
  - контент/определение
---

> [!tip] G-Eval
> **G-Eval** — формализация rubric-подхода с агрегацией оценки через вероятности токенов шкалы, а не просто текстовым score.

Метод [[LLM-as-a-Judge]] использует chain-of-thought и заполнение формы оценки (form-filling). Критерии задаёт [[Rubric]].

**G-Eval** — методология оценивания; **deepeval** — библиотека, содержащая её реализацию `GEval` и другие метрики.

## источник

«LLM-as-a-Judge, бенчмаркинг, гардрейлы», раздел 5.3.

## Anki

TARGET DECK: stem::ml::engineering

START
math_basic_single
FRONT: Что такое G-Eval?
BACK: По сути, формализация того самого rubric-подхода из раздела 3, но с конкретной методикой агрегации оценки через вероятности токенов шкалы, а не просто текстовый score.
ID: 1789915215259
END

START
math_basic_single
FRONT: Чем различаются G-Eval и deepeval?
BACK: G-Eval — методология оценивания; deepeval — библиотека, содержащая её реализацию GEval и другие метрики.
ID: 1789915215260
END
