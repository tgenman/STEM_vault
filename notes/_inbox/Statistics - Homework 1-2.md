author: **Dmitrii Bondarev** (Дмитрий Бондарев)
group: М05-321сс (**Contemporary Combinatorics**)
date: 2024-04-11


#### **Problem 1.** Let $X_1, \ldots, X_n \sim U[0,\theta]$ and let $\hat{\theta} = \max\{X_1, \ldots, X_n\}$. Find:
##### (2 points) bias of this estimator
Since $X_i \sim U[0,\theta]$:

$P(X_i \leq x) = \frac{x}{\theta}$

$F_{\hat{\theta}} = P(\hat{\theta} \leq x) = P(X_1 \leq x, \ldots, X_n \leq x) = \left(\frac{x}{\theta}\right)^n$

$f_{\hat{\theta}}(x) = \frac{d}{dx}\left(\frac{x}{\theta}\right)^n = \frac{n x^{n-1}}{\theta^n}$

$E[\hat{\theta}] = \int_0^\theta x \cdot \frac{n x^{n-1}}{\theta^n} dx = \frac{n}{\theta^n} \int_0^\theta x^n dx = \frac{n}{\theta^n} \cdot \frac{\theta^{n+1}}{n+1} = \frac{n\theta}{n+1}$

$\text{Bias}(\hat{\theta}) = E[\hat{\theta}] - \theta = \frac{n\theta}{n+1} - \theta = \theta\left(\frac{n}{n+1} - 1\right) = -\frac{\theta}{n+1}$

##### (2 points) standard error of this estimator

$E[\hat{\theta}^2] = \int_0^\theta x^2 \cdot \frac{n x^{n-1}}{\theta^n} dx = \frac{n}{\theta^n} \cdot \frac{\theta^{n+2}}{n+2} = \frac{n\theta^2}{n+2}$

$Var(\hat{\theta}) = E[\hat{\theta}^2] - (E[\hat{\theta}])^2 = \frac{n\theta^2}{n+2} - \left(\frac{n\theta}{n+1}\right)^2$

$SE(\hat{\theta}) = \sqrt{Var(\hat{\theta})} = \sqrt{\frac{n\theta^2}{n+2} - \left(\frac{n\theta}{n+1}\right)^2}$

##### (1 point) MSE of this estimator
$MSE(\hat{\theta}) = \text{bias}^2(\hat{\theta}) + \text{Var}(\hat{\theta})$

$MSE(\hat{\theta}) = \left(-\frac{\theta}{n+1}\right)^2 + \frac{n\theta^2}{n+2} - \left(\frac{n\theta}{n+1}\right)^2$

##### (1 point) Is this estimator consistent?
$\hat{\theta}_n \xrightarrow{p} \theta$

$\lim_{n \to \infty} P(|\hat{\theta}_n - \theta| \geq \epsilon) = 0, \quad \forall \epsilon > 0$

$F_{\hat{\theta}}(x) = P(\hat{\theta} \leq x) = \left(\frac{x}{\theta}\right)^n, \quad 0 \leq x \leq \theta$

$P(\hat{\theta}_n \geq \theta + \epsilon) = 0$ because $\hat{\theta}_n \leq \theta$ for all $n$.

$P(\hat{\theta}_n \leq \theta - \epsilon) = \left(\frac{\theta - \epsilon}{\theta}\right)^n$

$\lim_{n \to \infty} P(\hat{\theta}_n \leq \theta - \epsilon) = \lim_{n \to \infty} \left(\frac{\theta - \epsilon}{\theta}\right)^n = 0$

##### (1 point) Is this estimator strongly consistent?

$\hat{\theta}_n \xrightarrow{a.s.} \theta \iff P(\lim_{n \to \infty} \hat{\theta}_n = \theta) = 1$

$F_{\hat{\theta}}(x) = P(\hat{\theta} \leq x) = \left(\frac{x}{\theta}\right)^n, \quad 0 \leq x \leq \theta$


For any $\epsilon > 0$,
	-  $P(\hat{\theta}_n < \theta - \epsilon) = \left(\frac{\theta - \epsilon}{\theta}\right)^n$
        - $\lim_{n \to \infty} P(\hat{\theta}_n < \theta - \epsilon) = \lim_{n \to \infty} \left(\frac{\theta - \epsilon}{\theta}\right)^n = 0$
	- $P(\hat{\theta}_n > \theta) = 0$, as $\hat{\theta}_n \leq \theta$
        - $\lim_{n \to \infty} P(\hat{\theta}_n > \theta + \epsilon) = 0$ by definition

$P(\lim_{n \to \infty} \hat{\theta}_n = \theta) = 1$


---

#### **Problem 2.** Let $X_1, \ldots, X_n \sim U[0,\theta]$ and let $\hat{\theta} = 2\hat{X}_n = \frac{2}{n} \sum_{k=1}^n X_k$. Find:
##### (2 points) bias of this estimator
 $\hat{\theta} = 2\hat{X}_n$ 

$E[X_i] = \frac{0 + \theta}{2} = \frac{\theta}{2}$

Since $\hat{X}_n = \frac{1}{n} \sum_{k=1}^n X_k$, the expected value of $\hat{X}_n$ is:

$E[\hat{X}_n] = E\left[\frac{1}{n} \sum_{k=1}^n X_k\right] = \frac{1}{n} \sum_{k=1}^n E[X_k] = \frac{1}{n} \cdot n \cdot \frac{\theta}{2} = \frac{\theta}{2}$

$E[\hat{\theta}] = E[2\hat{X}_n] = 2E[\hat{X}_n] = 2 \cdot \frac{\theta}{2} = \theta$

$\text{Bias}(\hat{\theta}) = E[\hat{\theta}] - \theta = \theta - \theta = 0$
##### (2 points) standard error of this estimator
$\text{Var}(X_i) = \frac{(\theta - 0)^2}{12} = \frac{\theta^2}{12}$

$\text{Var}(\hat{X}_n) = \frac{1}{n^2} \sum_{k=1}^n \text{Var}(X_k) = \frac{1}{n^2} \cdot n \cdot \frac{\theta^2}{12} = \frac{\theta^2}{12n}$

$\text{Var}(\hat{\theta}) = \text{Var}(2\hat{X}_n) = 4\text{Var}(\hat{X}_n) = 4 \cdot \frac{\theta^2}{12n} = \frac{\theta^2}{3n}$

$\text{SE}(\hat{\theta}) = \sqrt{\text{Var}(\hat{\theta})} = \sqrt{\frac{\theta^2}{3n}} = \frac{\theta}{\sqrt{3n}}$

##### (1 point) MSE of this estimator

$MSE(\hat{\theta}) = \text{bias}^2(\hat{\theta}) + \text{Var}(\hat{\theta})$

$MSE(\hat{\theta}) = 0 + \frac{\theta^2}{3n} = \frac{\theta^2}{3n}$


---

#### **Problem 3.** (3 points) Let $X_1, \ldots, X_n \sim Be(p)$ and let $Y_1, \ldots, Y_m \sim Be(q)$. Find the plug-in estimator, its bias and estimated standard error:


##### Plug-in Estimator for $p$
Given $X_1, \ldots, X_n \sim Be(p)$:
$\hat{p} = \frac{1}{n} \sum_{i=1}^n X_i$

$\text{Bias}(\hat{p}) = E[\hat{p}] - p$

Since $E[\hat{p}] = p$:
$\text{Bias}(\hat{p}) = p - p = 0$

$\text{Var}(\hat{X}_n) = \frac{1}{n^2} \sum_{k=1}^n \text{Var}(X_k) = \frac{1}{n^2} \cdot n \cdot p(1-p) = \frac{p(1-p)}{n}$

$\text{SE}(\hat{p}) = \sqrt{\frac{p(1-p)}{n}}$

##### Plug-in Estimator for $p - q$
Given $Y_1, \ldots, Y_m \sim Be(q)$:

$\hat{q} = \frac{1}{m} \sum_{i=1}^m Y_i$

$\hat{p} - \hat{q} = \left(\frac{1}{n} \sum_{i=1}^n X_i\right) - \left(\frac{1}{m} \sum_{i=1}^m Y_i\right)$

$\text{Bias}(\hat{p} - \hat{q}) = E[\hat{p} - \hat{q}] - (p - q) = (p - q) - (p - q) = 0$

$\text{Var}(\hat{p} - \hat{q}) = \text{Var}(\hat{p}) + \text{Var}(\hat{q}) = \frac{p(1-p)}{n} + \frac{q(1-q)}{m}$

$\text{SE}(\hat{p} - \hat{q}) = \sqrt{\frac{p(1-p)}{n} + \frac{q(1-q)}{m}}$

---

#### **Problem 4.** (3 points) Let $X_1, \ldots, X_n$ be distinct observations (no ties). Prove that there are exactly $\binom{2n-1}{n}$ possible distinct bootstrap samples.

Number possible distinct bootstrap samples equals number combinations with repetitions:

$\bar{C_{n}^k} = \left(\binom{n}{k} \right) = \binom{n+k-1}{k} = C_{n+k-1}^k$

For case $k=n$
$\bar{C_{n}^n} = \binom{n+n-1}{n} = \binom{2n-1}{n}$

---

#### **Problem 5.** (4 points, computer experiment) Generate $n = 100$ observations from $N(0,1)$. Compute the 95% confidence band for the CDF $F(\cdot)$ using DKW inequality. Repeat this $m = 1000$ times and report the fraction of times that the 95% confidence band contains:
1. the true CDF
2. the ECDF

![[Pasted image 20240411223518.png]]