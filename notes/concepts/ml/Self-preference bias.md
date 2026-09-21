---
aliases:
  - "Self-enhancement bias"
anki: true
created: "2026-09-20"
parent:
  - "[[LLM-as-a-Judge]]"
connected:
  - "[[Blind evaluation]]"
tags:
  - контент/определение
  - фикс/анки
---

> [!tip] self-preference bias
> **Self-preference (self-enhancement) bias** — судья завышает оценку ответам, сгенерированным моделью его же семейства.

## проверка

Зафиксировать вопрос и сопоставимые по качеству ответы двух моделей. Качество предварительно проверить по человеческой оценке или reference-based метрике.

Использовать [[LLM-as-a-Judge]] того же семейства, что одна из моделей, и сравнить распределения оценок. Повторить сравнение при скрытых и явно указанных источниках ответов — [[Blind evaluation]].

## иллюстрация

![[llm-judge-self-preference-bias.png]]

Синтетический пример.

## источник

«LLM-as-a-Judge, бенчмаркинг, гардрейлы», раздел 4.2 и вводная часть раздела 4.

## Anki

TARGET DECK: stem::ml::engineering

START
math_complex
FRONT: Что такое self-preference bias у LLM-судьи?
BACK: Судья завышает оценку ответам, сгенерированным моделью его же семейства.
FORMULA:
PICTURE: ![[llm-judge-self-preference-bias.png]]
ADDITIONAL: Синтетический пример.
PROOF:
END
