---
aliases: 
anki: false
created: 2024-04-24 18:49
parent:
  - "[[Functions of random variables]]"
connected: 
tags: []
---

- $Z := X + Y$ with the probability density function given by $f_Z(z) = \int_{-\infty}^{\infty} f_{X,Y}(x, z - x) \, dx$ for $X,Y\geq 0$ this is equal to $\int_{0}^{z} f_{X,Y}(x, z - x) \, dx$.

- $Z := |X - Y|$ with the probability density function given by $f_Z(z) = 2 \int_{0}^{\infty} f_{X,Y}(x, z + x) \, dx$.

- $Z := \frac{X}{Y}$ with the probability density function given by $$f_Z(z) = \int_{-\infty}^{\infty} |y| f_{X,Y}(yz, y) \, dy$$ which is also represented as $$\int_{-\infty}^{\infty} |y| f_X(yz) f_Y(y) \, dy$$.
