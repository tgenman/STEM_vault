---
aliases:
  - FDR
  - Ожидаемая доля ложных открытий
anki: false
created: "2026-09-15"
parent:
  - "[[519.22 Statistic MOC]]"
connected:
  - "[[multiple testing]]"
  - "[[Benjamini-Hochberg procedure]]"
  - "[[False positive]]"
tags:
  - контент/определение
---

> [!tip] false discovery rate
> The expected fraction of false rejections among all rejected hypotheses, taking that fraction as zero when there are no rejections.

$$
\operatorname{FDR}=\mathbb{E}\left[\frac{V}{\max(R,1)}\right],
$$
where $V$ counts false rejections and $R$ counts all rejections.

FDR is an error criterion, not a correction algorithm or a guarantee about the realized fraction in one study.

Source: [R stats: p.adjust](https://stat.ethz.ch/R-manual/R-devel/library/stats/html/p.adjust.html).
