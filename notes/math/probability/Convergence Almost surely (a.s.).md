---
aliases: 
anki: false
created: 2024-04-11 13:27
parent: 
connected:
  - "[[Convergence]]"
tags:
  - content/empty
---

Let $(T_n)_{n\geq1}$ a sequence of r.v. and $T$ a r.v. ($T$ may be deterministic).

$$ T_n \xrightarrow{a.s.} T \text{ iff } \mathbb{P}\left[\left\{\omega : T_n(\omega) \rightarrow T(\omega)\right\}\right] = 1. $$

---

Последовательность $\xi_n$ сходится к случайному вектору $\xi$ почти наверное
$$\xi_n\xrightarrow[n\to\infty]{п. н.}\xi$$
если вероятность тех $\omega$, на которых у нас есть сходимость к числовой последовательности $\xi_n(\omega)$ к $\xi(\omega)$ равно 1
$$P\big(\omega:\xi_n(\omega)\to\xi(\omega)\big)=1$$
Другими словами, если выбрать случайное число из последовательности, то с вероятностью, равной 1, все последующие числа последовательности будут близки к $\xi$, начиная с некоторого номера $N$.

