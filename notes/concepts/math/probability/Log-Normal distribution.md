---
aliases: 
anki: false
created: 2024-04-24 11:47
parent:
  - "[[Distribution of r.v. MOC]]"
  - "[[General Random Variables]]"
  - "[[Normal distribution]]"
connected: 
tags: 
---

> [!tip] Log-normal $\operatorname{LogNormal}(\mu,\sigma^2)$
> $X=e^Z$ where $Z\sim\mathcal N(\mu,\sigma^2)$ and $\sigma>0$.

- [[PDF - f_X(x)|PDF]]: $f_X(x)=\frac{1}{x\sigma\sqrt{2\pi}}\exp[-(\ln x-\mu)^2/(2\sigma^2)]$ for $x>0$, and zero otherwise.
- [[CDF - F_X(x)|CDF]]: $F_X(x)=\Phi((\ln x-\mu)/\sigma)$ for $x>0$, and zero for $x\le0$. Here $\Phi$ is the standard normal CDF.
- [[Expected Value E(X)|Mean]]: $e^{\mu+\sigma^2/2}$.
- [[Variance V(X)|Variance]]: $(e^{\sigma^2}-1)e^{2\mu+\sigma^2}$.

![[Pasted image 20240424115351.png|300]]
![[Pasted image 20240424115428.png|300]]

Source: [R stats: log-normal](https://stat.ethz.ch/R-manual/R-devel/library/stats/html/Lognormal.html).
