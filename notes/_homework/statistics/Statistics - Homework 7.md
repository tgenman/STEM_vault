author: **Dmitrii Bondarev** (Дмитрий Бондарев)
group: М05-321сс (**Contemporary Combinatorics**)
date: 2024-05-29

### Problem 1
#### 1.1 Find $\xi_i$ Probability that there is a thief in your apartment if there is an alarm: $p(t = 1|a = 1)$

$p(t = 1|a = 1) = \frac{p(a = 1|t = 1) \cdot p(t = 1)}{p(a = 1)}$

$p(a = 1|t = 1) = p(a = 1|t = 1, e = 0) \cdot p(e = 0) + p(a = 1|t = 1, e = 1) \cdot p(e = 1) =$
$= 1 \cdot 0.99 + 1 \cdot 0.01 = 1$


$\begin{aligned} p(a = 1) &= p(a = 1|t = 0, e = 0) \cdot p(t = 0) \cdot p(e = 0) \\ &\quad + p(a = 1|t = 0, e = 1) \cdot p(t = 0) \cdot p(e = 1) \\ &\quad + p(a = 1|t = 1, e = 0) \cdot p(t = 1) \cdot p(e = 0) \\ &\quad + p(a = 1|t = 1, e = 1) \cdot p(t = 1) \cdot p(e = 1)\end{aligned}$

$\begin{aligned} p(a = 1) &= 0 \cdot 0.9998 \cdot 0.99 + 0.1 \cdot 0.9998 \cdot 0.01 \\ &\quad + 1 \cdot 0.0002 \cdot 0.99 + 1 \cdot 0.0002 \cdot 0.01 \\ &= 0 + 0.0009998 + 0.000198 + 0.000002 \\ &= 0.0011998 \end{aligned}$

$p(t = 1|a = 1) = \frac{1 \cdot 0.0002}{0.0011998} \approx 0.1667$


#### 1.2 Probability that there is a thief in your apartment if there is an alarm and you hear an announcement about an earthquake on the radio: $p(t = 1|a = 1, r = 1)$

$p(t=1|a=1, r=1) = \frac{p(a=1, r=1|t=1) \cdot p(t=1)}{p(a=1, r=1)}$

$p(a=1, r=1|t=1) = p(a=1|t=1, e=0) \cdot p(r=1|e=0) \cdot p(e=0) +$ 
$+ p(a=1|t=1, e=1) \cdot p(r=1|e=1) \cdot p(e=1) =$
$= 1 \cdot 0 \cdot 0.99 + 1 \cdot 0.5 \cdot 0.01 = 0.005$

$p(a=1, r=1) = \sum_{t} \sum_{e} p(a=1, r=1|t, e) \cdot p(t) \cdot p(e)$

$\begin{aligned} p(a=1, r=1) &= 0 \cdot 0.9998 \cdot 0.99 + 0.1 \cdot 0.5 \cdot 0.9998 \cdot 0.01\\ &+ 1 \cdot 0 \cdot 0.0002 \cdot 0.99 + 1 \cdot 0.5 \cdot 0.0002 \cdot 0.01 \\ &= 0 + 0.05 \cdot 0.9998 \cdot 0.01 + 0 + 0.0001 \cdot 0.0002 \\ &= 0.0004999 + 0.000001 \\ &= 0.0005009 \end{aligned}$

$p(t=1|a=1, r=1) = \frac{0.005 \cdot 2 \cdot 10^{-4}}{0.0005009} \approx 0.001998$

---

### Problem 2
Prior:
$\theta \sim \mathcal{N}(a, b^2)$

Likelihood:
$f(X_1, \ldots, X_n | \theta) = \prod_{i=1}^n \frac{1}{\sqrt{2\pi\sigma^2}} \exp\left(-\frac{(X_i - \theta)^2}{2\sigma^2}\right)$

Posterior (using Bayes' theorem):
$\pi(\theta | X_1, \ldots, X_n) \propto \left(\prod_{i=1}^n \exp\left(-\frac{(X_i - \theta)^2}{2\sigma^2}\right)\right) \exp\left(-\frac{(\theta - a)^2}{2b^2}\right)$

$\pi(\theta | X_1, \ldots, X_n) \propto \exp\left(-\frac{1}{2\sigma^2} \left( \sum_{i=1}^n (X_i^2 - 2X_i\theta + \theta^2) \right) - \frac{1}{2b^2} (\theta^2 - 2a\theta + a^2)\right)$

$\pi(\theta | X_1, \ldots, X_n) \propto \exp\left(-\frac{1}{2} \left( \left(\frac{n}{\sigma^2} + \frac{1}{b^2}\right)\theta^2 - 2 \left(\frac{\sum_{i=1}^n X_i}{\sigma^2} + \frac{a}{b^2}\right)\theta + \text{const}\right)\right)$

Identify parameters for the normal posterior:
$\tau^2 = \left( \frac{n}{\sigma^2} + \frac{1}{b^2} \right)^{-1}$
$\bar{\theta} = \tau^2 \left( \frac{\sum_{i=1}^n X_i}{\sigma^2} + \frac{a}{b^2} \right) = \left( \frac{1}{\frac{1}{b^2} + \frac{n}{\sigma^2}} \right) \left( \frac{a}{b^2} + \frac{\sum_{i=1}^n X_i}{\sigma^2} \right)$

Thus, the posterior distribution is:
$\theta | X_1, \ldots, X_n \sim \mathcal{N}(\bar{\theta}, \tau^2)$

---

### Problem 3
#### 3.1 Consider a prior $\lambda \sim Gamma(\alpha, \beta)$. Show that the posterior is also a Gamma, find its parameters.
$L(\lambda \mid X_1, \ldots, X_n) = \lambda^{\sum_{i=1}^n X_i} e^{-n \lambda}$

Prior:
$p(\lambda) = \frac{\beta^\alpha}{\Gamma(\alpha)} \lambda^{\alpha-1} e^{-\beta \lambda}$

Posterior:
$p(\lambda \mid X_1, \ldots, X_n) \propto \lambda^{\alpha + \sum_{i=1}^n X_i - 1} e^{-(\beta + n)\lambda}$

$Gamma\left(\alpha + \sum_{i=1}^n X_i, \beta + n\right)$

#### 3.2 Find the posterior mean, show that it is a weighted sum of MLE and prior mean.
Posterior mean for $Gamma(\alpha', \beta')$:
$\mathbb{E}[\lambda \mid X_1, \ldots, X_n] = \frac{\alpha + \sum_{i=1}^n X_i}{\beta + n}$

$\hat{\lambda}_{\text{MLE}} = \frac{1}{n} \sum_{i=1}^n X_i$

$\mathbb{E}[\lambda] = \frac{\alpha}{\beta}$

Posterior mean as a weighted sum:
$\mathbb{E}[\lambda \mid X_1, \ldots, X_n] = \frac{\beta}{\beta + n} \mathbb{E}[\lambda] + \frac{n}{\beta + n} \hat{\lambda}_{\text{MLE}}$

#### 3.3 Find the Jeffreys’ prior, find parameters of the posterior if the prior is Jeffreys’ prior.
Jeffreys' prior:
$p(\lambda) \propto \frac{1}{\sqrt{\lambda}} \implies \lambda \sim Gamma\left(\frac{1}{2}, 0\right)$

Posterior with Jeffreys' prior:

$p(\lambda \mid X_1, \ldots, X_n) \propto \lambda^{\sum_{i=1}^n X_i - \frac{1}{2}} e^{-n \lambda}$

$Gamma\left(\sum_{i=1}^n X_i + \frac{1}{2}, n\right)$