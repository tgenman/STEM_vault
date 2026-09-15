---
aliases:
  - BH procedure
  - Процедура Бенджамини — Хохберга
anki: false
created: "2026-09-15"
parent:
  - "[[519.22 Statistic MOC]]"
connected:
  - "[[multiple testing]]"
  - "[[false discovery rate]]"
tags:
  - контент/алгоритм
---

> [!tip] Benjamini-Hochberg procedure
> A step-up multiple-testing procedure for controlling [[false discovery rate|FDR]].

For $m$ p-values and target $q\in(0,1)$:

1. Sort $p_{(1)}\le\cdots\le p_{(m)}$.
2. Find $k=\max\{i:p_{(i)}\le iq/m\}$.
3. Reject hypotheses corresponding to the first $k$ p-values. If the set is empty, reject none.

The standard guarantee holds for independent valid p-values. Dependent tests require checking the relevant dependence assumptions; arbitrary dependence is not covered by this statement.

Source: [R simulator: BH procedure](https://stat.ethz.ch/CRAN/web/packages/simulator/vignettes/fdr.html).
