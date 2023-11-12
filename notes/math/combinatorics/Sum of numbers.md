---
aliases: 
publish: true
anki: true
created: 2023-10-24 16:17
parent:
  - "[[Rising Sum of Binomial Coefficients]]"
connected:
---
Using formula of [[Rising Sum of Binomial Coefficients]]
$\binom{m+n+1}{m+1}=\binom mm+\binom{m+1}m+\ldots+\binom{m+n}m.$

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
TARGET DECK: Math::Combinatorics
START
Math prop
Question_eng: Sum of numbers for power 1
Question_rus: 
Answer_eng: $$
1+2+3+4+\ldots+n=\binom11+\binom21+ 
\ldots+\binom n1=\binom{n+1}2=\frac{n(n+1)}2.
$$
Answer_rus: 
Formula_main: 
Formula_additional:
<!--ID: 1698689128873-->
END

START
Math prop
Question_eng: Sum of numbers for power 2
Question_rus: 
Answer_eng: $$
1^2+2^2+3^2+4^2+\ldots+n^2=\frac{(n+1)n(2n+1)}{6}.
$$
Answer_rus: 
Formula_main: The sum of squares of the first $n$ natural numbers can be written as a sum of binomial coefficients:

$$\binom{2}{2} + \binom{3}{2} + \ldots + \binom{n}{2} = \binom{n+1}{3}$$

This can be expressed in a more familiar arithmetic sequence by rewriting each term:

$$\frac{2 \cdot 1}{2} + \frac{3 \cdot 2}{2} + \ldots + \frac{n(n-1)}{2} = \frac{1^2 - 1}{2} + \frac{2^2 - 2}{2} + \frac{3^2 - 3}{2} + \ldots + \frac{n^2 - n}{2}$$

By separating the summation of squares and the arithmetic sum, we have:

$$\frac{1^2 + 2^2 + 3^2 + \ldots + n^2}{2} - \frac{1 + 2 + \ldots + n}{2}$$

Now we isolate the sum of the squares on the left side of the equation:

$$\frac{1^2 + 2^2 + 3^2 + \ldots + n^2}{2} = \binom{n+1}{3} + \frac{1 + 2 + \ldots + n}{2} = \frac{(n+1)n(n-1)}{6} + \frac{n(n+1)}{4}$$

By combining terms under a common denominator, we obtain:

$$\frac{(n+1)n}{2} \left(\frac{n-1}{3} + \frac{1}{2}\right) = \frac{(n+1)n}{2} \left(\frac{2n+1}{6}\right) = \frac{(n+1)n(2n+1)}{12}$$

Therefore, the sum of the squares equals:

$$1^2 + 2^2 + 3^2 + \ldots + n^2 = \frac{(n+1)n(2n+1)}{6}$$

Formula_additional:
<!--ID: 1698689128880-->
END









