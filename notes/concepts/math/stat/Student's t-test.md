---
aliases:
  - t-тест Стьюдента
  - T критерий Стьюдента
anki: false
created: "2026-09-15"
parent:
  - "[[519.22 Statistic MOC]]"
connected:
  - "[[Hypothesis testing]]"
  - "[[Sample mean]]"
  - "[[Standard error]]"
tags:
  - контент/определение
---

> [!tip] Student's t-test
> A hypothesis test whose statistic is compared with a Student $t$ reference distribution under the null model.

## one-sample mean

For an independent sample from a normal population with unknown variance, testing $H_0:\mu=\mu_0$ uses
$$
t=\frac{\bar X-\mu_0}{s/\sqrt n},\qquad \mathrm{df}=n-1.
$$
The rejection region depends on whether the alternative is one-sided or two-sided. Other t-tests, such as paired and two-sample tests, have different constructions and assumptions.

Source: [NIST: tests for a population mean](https://www.itl.nist.gov/div898/handbook/prc/section2/prc22.htm).
