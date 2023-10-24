---
aliases: 
publish: true
anki: false
created: 2023-10-24 16:17
parent:
  - "[[Rising Sum of Binomial Coefficients]]"
connected: []
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
$$\begin{aligned}
&\binom22+\binom32+\ldots+\binom n2=\binom{n+1}3 \\
&\frac{2\cdot1}{2}+\frac{3\cdot2}{2}+\ldots+\frac{n(n-1)}{2}= \\
&\frac{1^{2}-1}{2}+\frac{2^{2}-2}{2}+\frac{3^{2}-3}{2}+\ldots+\frac{n^{2}-n}{2}= \\
&\frac{1^2+2^2+3^2+\ldots+n^2}2-\frac{1+2+\ldots+n}2 \\
&\frac{1^2+2^2+3^2+\ldots+n^2}2=\binom{n+1}3+\frac{1+2+\ldots+n}2 \\
&\frac{1^2+2^2+3^2+\ldots+n^2}2=\binom{n+1}3+\frac{1+2+\ldots+n}2= \\
&\frac{(n+1)n(n-1)}6+\frac{n(n+1)}4= \\
&\frac{(n+1)n}2(\frac{n-1}3~+~\frac12)~=~\frac{(n+1)n}2(\frac{2n+1}6)~= \\
&\frac{(n+1)n(2n+1)}{12} \\
&1^2+2^2+3^2+\ldots+n^2=\frac{(n+1)n(2n+1)}6
\end{aligned}$$
$$\begin{aligned}
&\frac{1^2+2^2+3^2+\ldots+n^2}2=\binom{n+1}3+\frac{1+2+\ldots+n}2= \\
&\frac{(n+1)n(n-1)}6+\frac{n(n+1)}4= \\
&\frac{(n+1)n}2(\frac{n-1}3~+~\frac12)~=~\frac{(n+1)n}2(\frac{2n+1}6)~= \\
&\frac{(n+1)n(2n+1)}{12} \\
&1^2+2^2+3^2+\ldots+n^2=\frac{(n+1)n(2n+1)}6
\end{aligned}$$











