author: **Dmitrii Bondarev** (Дмитрий Бондарев)
group: М05-321сс (**Contemporary Combinatorics**)
date: 2024-05-29

### Problem 1. 
#### 1.1 Find $\xi_i$
$T(X) = \sum_{i=1}^r \frac{(\nu_i - np_i)^2}{np_i}$
$\xi_i^2 = \frac{(\nu_i - np_i)^2}{np_i}$
$\xi_i = \frac{\nu_i - np_i}{\sqrt{np_i}}$

#### 1.2 Show that $\xi = (\xi_1, \ldots, \xi_r)$ is degenerate, i.e. $\exists b : \xi^\top b = 0$
Consider $b = (1, 1, \ldots, 1)$. Then
$\xi^\top b = \sum_{i=1}^r \xi_i = \sum_{i=1}^r \frac{\nu_i - np_i}{\sqrt{np_i}}$
Since $\sum_{i=1}^r \nu_i = n$ and $\sum_{i=1}^r np_i = n$
$\sum_{i=1}^r (\nu_i - np_i) = n - n = 0$
$\sum_{i=1}^r \frac{\nu_i - np_i}{\sqrt{np_i}} = 0$
$\xi^\top b = 0$
This proves that $\xi = (\xi_1, \ldots, \xi_r)$ is degenerate.

#### 1.3 Use CLT to prove that $\xi_i$ has normal distribution and find its parameters
By the Central Limit Theorem:
$\nu_i \sim \mathcal{N}(np_i, np_i(1 - p_i))$
Normalize:
$\xi_i = \frac{\nu_i - np_i}{\sqrt{np_i}} \approx \frac{\mathcal{N}(np_i, np_i(1 - p_i)) - np_i}{\sqrt{np_i}} = \mathcal{N}\left(0, \frac{np_i(1 - p_i)}{np_i}\right) = \mathcal{N}(0, 1 - p_i)$
Thus, $\xi_i \sim \mathcal{N}(0, 1)$


#### 1.4 Find $\mathbb{E}[\xi_i \xi_j]$ for $i = j$ and $i \neq j$
Case $i = j$
Express $\xi_i$:
$\xi_i = \frac{\nu_i - np_i}{\sqrt{np_i}}$

Since $\nu_i \sim \text{Binomial}(n, p_i)$, we have:
$\mathbb{E}[\nu_i] = np_i, \quad \text{Var}(\nu_i) = np_i(1 - p_i)$

Thus:
$\mathbb{E}[\xi_i^2] = \mathbb{E}\left[\left(\frac{\nu_i - np_i}{\sqrt{np_i}}\right)^2\right] = \frac{1}{np_i} \mathbb{E}[(\nu_i - np_i)^2] = \frac{np_i(1 - p_i)}{np_i} = 1 - p_i$

Case $i \neq j$
For $\mathbb{E}[\xi_i \xi_j]$:
$\mathbb{E}[\xi_i \xi_j] = \mathbb{E}\left[\left(\frac{\nu_i - np_i}{\sqrt{np_i}}\right) \left(\frac{\nu_j - np_j}{\sqrt{np_j}}\right)\right]$

Since $\text{Cov}(\nu_i, \nu_j) = -np_i p_j$:
$\mathbb{E}[\xi_i \xi_j] = \frac{\text{Cov}(\nu_i, \nu_j)}{\sqrt{np_i} \sqrt{np_j}} = \frac{-np_i p_j}{\sqrt{np_i} \sqrt{np_j}} = -\sqrt{p_i p_j}$

$$
\mathbb{E}[\xi_i \xi_j] = 
\begin{cases} 
1 - p_i, & \text{if } i = j, \\
-\sqrt{p_i p_j}, & \text{if } i \neq j
\end{cases}
$$


---

### Problem 2
Hypotheses:
- $H_0$: $X \sim U[0, 9]$
- $H_1$: $X \not\sim U[0, 9]$

Total observations: $N = 800$
Expected frequency for each interval: $E_i = \frac{800}{10} = 80$

 $\chi^2$ Test Statistic Calculation:
$\chi^2 = \sum_{i=0}^{9} \frac{(O_i - E_i)^2}{E_i} = \frac{(74-80)^2}{80} + \frac{(92-80)^2}{80} + \frac{(83-80)^2}{80} + \frac{(79-80)^2}{80} + \frac{(80-80)^2}{80}$
$+ \frac{(73-80)^2}{80} + \frac{(77-80)^2}{80} + \frac{(75-80)^2}{80} + \frac{(76-80)^2}{80} + \frac{(91-80)^2}{80} =$
$= 0.45 + 1.8 + 0.1125 + 0.0125 + 0 + 0.6125+$
$+ 0.1125 + 0.3125 + 0.2 + 1.5125 = 5.125$

Comparison with Critical Value:
Degrees of freedom: $df = 10 - 1 = 9$
Critical value at $\alpha = 0.05$ and $df = 9$: $16.919$

Since $\chi^2 = 5.125 < 16.919$, we fail to reject $H_0$.

---
### Problem 3
Hypotheses
$H_0: \mu_x = \mu_y$
$H_1: \mu_x \ne \mu_y$

Means
$\overline{X} = \frac{\sum X_i}{n} = \frac{-2.82}{10} = -0.282$
$\overline{Y} = \frac{\sum Y_i}{n} = \frac{-1.67}{10} = -0.167$

Variances
$s_x^2 = \frac{\sum (X_i - \overline{X})^2}{n-1} = \frac{8.797}{9} = 0.978$
$s_y^2 = \frac{\sum (Y_i - \overline{Y})^2}{n-1} = \frac{6.531}{9} = 0.726$

Pooled Variance
$s_p^2 = \frac{(n_x - 1)s_x^2 + (n_y - 1)s_y^2}{n_x + n_y - 2} = \frac{8.802 + 6.534}{18} = 0.852$

Standard Error
$SE = \sqrt{s_p^2 \left( \frac{1}{n_x} + \frac{1}{n_y} \right)} = \sqrt{0.852 \left( \frac{2}{10} \right)} = 0.413$

Test Statistic
$t = \frac{\overline{X} - \overline{Y}}{SE} = \frac{-0.282 - (-0.167)}{0.413} = -0.278$

Critical Value
For $\alpha = 0.05$ and $df = 18$, the critical value $t_{0.025, 18} \approx 2.101$.
Since $|t| = 0.278 < 2.101$, we fail to reject $H_0$.

At the $\alpha = 0.05$ level, there is no significant difference between the means of $X$ and $Y$.

---

### Problem 4
$$
\begin{array}{cccccc}
i & X_i & Y_i & d_i = X_i - Y_i & |d_i| & \text{Rank} \\
1 & 176 & 168 & 8 & 8 & 3 \\
2 & 163 & 215 & -52 & 52 & 11 \\
3 & 152 & 172 & -20 & 20 & 7 \\
4 & 155 & 200 & -45 & 45 & 10 \\
5 & 156 & 191 & -35 & 35 & 9 \\
6 & 178 & 197 & -19 & 19 & 5.5 \\
7 & 160 & 183 & -23 & 23 & 8 \\
8 & 164 & 174 & -10 & 10 & 4 \\
9 & 169 & 176 & -7 & 7 & 1.5 \\
10 & 155 & 155 & 0 & 0 & \text{(ignored)} \\
11 & 122 & 115 & 7 & 7 & 1.5 \\
12 & 144 & 163 & -19 & 19 & 5.5 \\
\end{array}
$$

$W^ = 3 + 1.5 = 4.5$

$W^- = 11 + 7 + 10 + 9 + 5.5 + 8 + 4 + 1.5 + 5.5 = 61.5$
$W = \min(W^+, W^-) = 4.5$


$T = \frac{W}{\sqrt{\frac{1}{6} n (n + 1) (2n + 1)}}$

With $n = 11$:
$T = \frac{4.5}{\sqrt{\frac{1}{6} \cdot 11 \cdot 12 \cdot 23}} = \frac{4.5}{22.49} \approx 0.2$

For $\alpha = 0.05$ (two-tailed), critical value $\approx 1.96$.
Since $|0.2| \le 1.96$, we fail to reject the null hypothesis.

---

### Problem 5
#### Find $c$ so that test has size $\alpha$
$T(X) \sim \mathcal{N}\left(0, \frac{1}{n}\right)$
$\sqrt{n} T(X) \sim \mathcal{N}(0, 1)$
$P(\sqrt{n} T(X) > \sqrt{n} c) = \alpha$

Let $z_\alpha$ be the $1 - \alpha$ quantile of $\mathcal{N}(0, 1)$:
$\sqrt{n} c = z_\alpha$
$c = \frac{z_\alpha}{\sqrt{n}}$

#### Find test power $W$
Rejected region $R = \{X : T(X) > c\}$, where $T(X) = \frac{1}{n} \sum_{i=1}^n X_i$ and $c = \frac{z_\alpha}{\sqrt{n}}$.

- Under $H_0$: $T(X) \sim \mathcal{N}(0, \frac{1}{n})$
- Under $H_1$: $T(X) \sim \mathcal{N}(1, \frac{1}{n})$

$W = P(T(X) > c \mid H_1) = P\left( \frac{T(X) - 1}{\sqrt{1/n}} > \frac{c - 1}{\sqrt{1/n}} \right)$

$W = P\left( Z > \frac{c - 1}{\sqrt{1/n}} \right)$

---
### Problem 6
#### 6. 1 Compute likelihood ratio $\Lambda(X)$
 $H_0$: 
$L(\theta_0) = \left( \frac{1}{\sqrt{2\pi\sigma^2}} \right)^n \exp\left( -\frac{1}{2\sigma^2} \sum_{i=1}^n (X_i - \theta_0)^2 \right)$

 $H_1$: 
$L(\hat{\theta}) = \left( \frac{1}{\sqrt{2\pi\sigma^2}} \right)^n \exp\left( -\frac{1}{2\sigma^2} \sum_{i=1}^n (X_i - \bar{X})^2 \right)$

$\Lambda(X) = \frac{L(\theta_0)}{L(\hat{\theta})} = \exp\left( -\frac{n (\bar{X} - \theta_0)^2}{2\sigma^2} \right)$

#### 6.2 Compute $\lambda(X) = 2 \log \Lambda(X)$, find its distribution

$\lambda(X) = 2 \log \Lambda(X) = -\frac{n (\bar{X} - \theta_0)^2}{\sigma^2}$

 $H_0$: 
$\frac{n (\bar{X} - \theta_0)^2}{\sigma^2} \sim \chi^2(1) \quad \Rightarrow \quad \lambda(X) \sim -\chi^2(1)$

#### 6.3 Specify rejection region $R = \{X : \lambda(X) > c\}$ using test size $\alpha$. Introduce change of variables such that the test statistic in new variables follows standard normal distribution. Specify the rejection region $R$ in new variables.

$P(\lambda(X) > c \mid H_0) = \alpha \quad \Rightarrow \quad c = -\chi^2_{1-\alpha}(1)$
$R = \left\{ X : \frac{n (\bar{X} - \theta_0)^2}{\sigma^2} > \chi^2_{1-\alpha}(1) \right\}$

Change of Variables
$Z = \frac{\sqrt{n}(\bar{X} - \theta_0)}{\sigma}$

 $H_0$: 
$Z \sim \mathcal{N}(0, 1)$
$R = \left\{ Z : Z^2 > \chi^2_{1-\alpha}(1) \right\} = \left\{ Z : |Z| > z_{1-\alpha/2} \right\}$
$R = \left\{ X : \left| \frac{\sqrt{n}(\bar{X} - \theta_0)}{\sigma} \right| > z_{1-\alpha/2} \right\}$