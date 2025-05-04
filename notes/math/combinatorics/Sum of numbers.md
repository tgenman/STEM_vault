---
aliases: 
anki: true
created: 2023-10-24 16:17
parent:
  - "[[Rising Sum of Binomial Coefficients]]"
connected:
---
Using formula of [[Rising Sum of Binomial Coefficients]]
$\binom nn+\binom{n+1}n+\ldots+\binom{n+m}n = \binom{n+m+1}{n+1}$

$C_n^n + C_{n+1}^n + \ldots + C_{n+m}^n = C_{n+m+1}^{n+1}$

We can calculate sum of first $n$ numbers

### Power 1
$$
1+2+3+4+\ldots+n=\binom11+\binom21+ 
\ldots+\binom n1=\binom{n+1}2=\frac{n(n+1)}2.
$$
### Power 2
$$
1^2+2^2+3^2+4^2+\ldots+n^2=\frac{(n+1)n(2n+1)}{6}.
$$
#### Proof
The sum of binomial coefficients $\binom{2}{2} + \binom{3}{2} + \ldots + \binom{n}{2}$ can be expressed as $\binom{n+1}{3}$. We can demonstrate this by showing each term of the sum corresponds to a specific formula:

$\frac{2 \cdot 1}{2} + \frac{3 \cdot 2}{2} + \ldots + \frac{n(n-1)}{2}$ can be rewritten as:

$\frac{1^2 - 1}{2} + \frac{2^2 - 2}{2} + \frac{3^2 - 3}{2} + \ldots + \frac{n^2 - n}{2}$, which simplifies to:

$\frac{1^2 + 2^2 + 3^2 + \ldots + n^2}{2} - \frac{1 + 2 + \ldots + n}{2}$.

Then, summing the squares separately, we have:

$$
\frac{1^2 + 2^2 + 3^2 + \ldots + n^2}{2} = \binom{n+1}{3} + \frac{1 + 2 + \ldots + n}{2}.
$$

Bringing the binomial coefficient and the arithmetic series together, we have:

$$
\frac{1^2 + 2^2 + 3^2 + \ldots + n^2}{2} = \frac{(n+1)n(n-1)}{6} + \frac{n(n+1)}{4}.
$$

This in turn equals:

$$
\frac{(n+1)n}{2} \left(\frac{n-1}{3} + \frac{1}{2}\right) = \frac{(n+1)n}{2} \left(\frac{2n+1}{6}\right) = \frac{(n+1)n(2n+1)}{12}.
$$

Therefore, the sum of the squares can be summarized in the format:

$$
1^2 + 2^2 + 3^2 + \ldots + n^2 = \frac{(n+1)n(2n+1)}{6}.
$$


### Anki
> [!question]- Sum of numbers for power 1
TARGET DECK: math::combinatorics
START
Math_TWO_side
TITLE: Sum of numbers for power 1
$1+2+3+4+\ldots+n=\binom11+\binom21+\ldots+\binom n1=\binom{n+1}2 =$
DESCRIPTION: $\frac{n(n+1)}2 =$
FORMULA: 
ADDITIONAL:
ID: 1706020955777
END

> [!question]- Sum of numbers for power 2
TARGET DECK: math::combinatorics
START
Math_TWO_side
TITLE: Sum of numbers for power 2
$1^2+2^2+3^2+4^2+\ldots+n^2 =$
DESCRIPTION: $\frac{(n+1)n(2n+1)}{6} =$
FORMULA: 
ADDITIONAL:
ID: 1706020955796
END

> [!question]- Sum of numbers for power 3
TARGET DECK: math::combinatorics
START
Math_TWO_side
TITLE: Sum of numbers for power 2
$1^3+2^3+3^3+4^3+\ldots+n^3 =$
DESCRIPTION: $\frac{n^2(n+1)^2}{4} =$
FORMULA: 
ADDITIONAL:
ID: 1706021072861
END






