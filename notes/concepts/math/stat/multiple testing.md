---
aliases:
  - Множественная проверка гипотез
  - Multiple Testing Problem
anki: false
created: "2026-09-15"
parent:
  - "[[519.22 Statistic MOC]]"
connected:
  - "[[Hypothesis testing]]"
  - "[[false discovery rate]]"
  - "[[p-hacking]]"
tags:
  - контент/определение
---

> [!tip] multiple testing
> Testing a family of hypotheses whose results are interpreted together.

A per-test significance threshold does not generally control the error rate for the family. Choose the error criterion explicitly: the probability of at least one false rejection, or [[false discovery rate|FDR]]. [[Benjamini-Hochberg procedure]] targets FDR under its assumptions.

Source: [R stats: p.adjust](https://stat.ethz.ch/R-manual/R-devel/library/stats/html/p.adjust.html).
