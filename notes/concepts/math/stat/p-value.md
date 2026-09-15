---
aliases: 
anki: false
created: 2024-06-18 19:51
parent:
  - "[[Hypothesis testing]]"
connected:
  - "[[False negative]]"
  - "[[False positive]]"
tags:
  - контент/определение
---

> [!tip] p-value
> Under the specified null model, the probability of a test statistic at least as incompatible with that model as the observed statistic.

For a simple null and a statistic where larger values are more extreme,
$$
p=P_{H_0}(T(X)\ge T(x_{\mathrm{obs}})).
$$
Other alternatives use the appropriate tail or extremeness rule. The value lies in $[0,1]$.

A p-value is not $P(H_0\mid X)$, not the probability that the result arose “by chance”, and not an effect size. A threshold such as $0.05$ is a chosen [[significance level]], not part of the definition.

Sources: [NIST: p-values](https://itl.nist.gov/div898/handbook/prc/section1/prc131.htm), [ASA statement](https://www.amstat.org/asa/files/pdfs/p-valuestatement.pdf).
