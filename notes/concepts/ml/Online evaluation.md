---
aliases:
  - онлайн-оценка
anki: false
created: "2026-09-20"
parent:
  - "[[LLM evaluation]]"
connected:
  - "[[Online метрики]]"
  - "[[A-B testing]]"
  - "[[Offline evaluation]]"
  - "[[Continuous evaluation]]"
  - "[[LLM-as-a-Judge]]"
tags:
  - контент/определение
  - фикс/анки
---
> [!tip] online evaluation
> **Online evaluation** — оценка работающей системы на текущем пользовательском трафике.

## применение

Наблюдать качество на реальных запросах, оценивать выборки production-логов вручную или через [[LLM-as-a-Judge]], сравнивать варианты на живом трафике.

Online evaluation не требует оценивать каждый запрос или выполнять оценку синхронно с ответом пользователю. Можно регулярно оценивать выборку логов.

- [[Online метрики]] — показатели, собираемые по данным работающей системы.
- [[A-B testing|Online A/B testing]] — один из дизайнов эксперимента, а не синоним всей online evaluation.
- [[Continuous evaluation]] — организация регулярной оценки во времени; может включать и [[Offline evaluation]].

## источники

- «LLM-as-a-Judge, бенчмаркинг, гардрейлы», разделы 5.4 и 7.1.
- [LangSmith — Evaluation types](https://docs.langchain.com/langsmith/evaluation-types).
