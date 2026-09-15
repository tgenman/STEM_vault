---
aliases:
  - Регрессионная функция
anki: false
created: "2026-09-15"
parent:
  - "[[519.22 Statistic MOC]]"
connected:
  - "[[Conditional expectation]]"
  - "[[Regression (machine learning)]]"
  - "[[Parametric model]]"
  - "[[Nonparametric model]]"
tags:
  - контент/определение
---

> [!tip] regression function
> We call $r(x) = \mathbb{E}[Y|X = x]$ the regression function.

## сохранённый контекст

Suppose we observe pairs of data $(X_1, Y_1), \ldots, (X_n, Y_n)$.
Perhaps $X_i$ is the blood pressure of subject $i$ and $Y_i$ is how long they live.
$X$ is called a predictor or regressor or feature or independent variable.
$Y$ is called the outcome or the response variable or the dependent variable.

If we assume that $r \in \mathcal{F}$ where $\mathcal{F}$ is finite dimensional — the set of straight lines for example — then we have a parametric regression model.
If we assume that $r \in \mathcal{F}$ where $\mathcal{F}$ is not finite dimensional then we have a nonparametric regression model.

The goal of predicting $Y$ for a new patient based on their $X$ value is called prediction.
If $Y$ is discrete (for example, live or die) then prediction is instead called classification. [[Classification ML]]

If our goal is to estimate the function $r$, then we call this regression or curve estimation. Regression models are sometimes written as

> [!note]
> Последнее предложение исходного фрагмента обрывается; окончание не восстановлено.

Перенесено из [[519.22 Statistic MOC]]; первоисточник формулировки не установлен.
