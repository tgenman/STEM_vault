---
aliases:
  - офлайн-оценка
anki: false
created: "2026-09-20"
parent:
  - "[[LLM evaluation]]"
connected:
  - "[[Evaluation dataset]]"
  - "[[Golden set]]"
  - "[[Offline метрики]]"
  - "[[Online evaluation]]"
  - "[[Continuous evaluation]]"
tags:
  - контент/определение
  - фикс/анки
---
> [!tip] offline evaluation
> **Offline evaluation** — оценка на подготовленном наборе примеров вне живого взаимодействия с пользователями.

Определение согласовано при разборе ноутбука; это формулировка заметки, а не дословная цитата источника.

## применение

Используется для сравнения вариантов системы и регрессионных проверок после изменения промпта, модели или пайплайна. Подготовленный набор может содержать сохранённые реальные запросы.

- [[Evaluation dataset]] — состав набора и покрытие сценариев.
- [[Golden set]] — проверенные эталонные ответы или факты, когда они нужны для оценки.
- [[Offline метрики]] — показатели качества, которые можно измерять в таком режиме.

В [[LLM evaluation]] offline описывает условия оценки, а регрессионная проверка — её цель. Offline-проверки могут быть частью [[Continuous evaluation]]. Другой режим — [[Online evaluation]].

## источники

- «LLM-as-a-Judge, бенчмаркинг, гардрейлы», ноутбук `4_LLM_Judge_Benchmarking_Guardrails.ipynb`, разделы 5.1, 5.4 и 8 — применение eval-сетов и регрессионных проверок.
- [LangSmith — Evaluation types](https://docs.langchain.com/langsmith/evaluation-types) — источник ранее согласованного разделения offline/online.
