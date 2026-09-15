author: **Dmitrii Bondarev** (Дмитрий Бондарев)
group: М05-321сс (**Contemporary Combinatorics**)
date: 2024-05-30

### Problem 1
$\rho_S = \frac{12}{n^3 - n} \sum_{i=1}^n \left( i - \frac{n + 1}{2} \right) \left( T_i - \frac{n + 1}{2} \right)$
$\left( i - \frac{n + 1}{2} - T_i + \frac{n + 1}{2} \right)^2 = (i - T_i)^2$
$\sum_{i=1}^n \left[ \left( i - \frac{n + 1}{2} \right) - \left( T_i - \frac{n + 1}{2} \right) \right]^2 = \sum_{i=1}^n (i - T_i)^2$

$\rho_S = \frac{12}{n^3 - n} \sum_{i=1}^n \left( i - \frac{n + 1}{2} \right) \left( T_i - \frac{n + 1}{2} \right)$
$\left( i - \frac{n + 1}{2} \right) \left( T_i - \frac{n + 1}{2} \right) = \frac{1}{2} \left[ (i - T_i)^2 - \left( i - \frac{n + 1}{2} \right)^2 - \left( T_i - \frac{n + 1}{2} \right)^2 \right]$

$\rho_S = \frac{12}{n^3 - n} \left[ \frac{1}{2} \sum_{i=1}^n (i - T_i)^2 - \frac{1}{2} \sum_{i=1}^n \left( i - \frac{n + 1}{2} \right)^2 - \frac{1}{2} \sum_{i=1}^n \left( T_i - \frac{n + 1}{2} \right)^2 \right]$

$\sum_{i=1}^n \left( i - \frac{n + 1}{2} \right)^2 = \sum_{i=1}^n \left( T_i - \frac{n + 1}{2} \right)^2$

$\rho_S = \frac{12}{n^3 - n} \left[ \frac{1}{2} \sum_{i=1}^n (i - T_i)^2 - \sum_{i=1}^n \left( i - \frac{n + 1}{2} \right)^2 \right]$

$\sum_{i=1}^n \left( i - \frac{n + 1}{2} \right)^2 = \frac{n(n^2 - 1)}{12}$

$\rho_S = \frac{12}{n^3 - n} \left[ \frac{1}{2} \sum_{i=1}^n (i - T_i)^2 - \frac{n(n^2 - 1)}{12} \right]$

$\rho_S = \frac{6}{n(n^2 - n)} \sum_{i=1}^n (i - T_i)^2 - 1$

$\rho_S = 1 - \frac{6}{n(n^2 - n)} \sum_{i=1}^n (i - T_i)^2$

