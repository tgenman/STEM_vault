---
aliases:
  - Перестановки без неподвижных точек
publish: true
anki: true
created: 2023-10-30 20:35
parent:
  - "[[k-arrangements from n-elements]]"
connected: []
---
$$d_n=n!\left(1-\frac{1}{1!}+\frac{1}{2!}-\ldots+(-1)^n\frac{1}{n!}\right)$$

$$
d_n\sim\frac{n!}e
$$


#### Proof
$$
\begin{aligned}
&\begin{aligned}d_n=|U|-\sum_i|A_i|+\sum_{i,j}|A_i\cap A_j|+...\end{aligned} \\
&\begin{aligned}\textsf{If}S\subset\{1,\ldots,n\}\textsf{ let }M=\cap_{j\in S}A_j.\end{aligned} \\
&M\text{ is the set of permutations }\pi\text{ with} \\
&\begin{aligned}\pi(j)&=j\text{ for all }j\in S.&\textsf{Then }|M|&=\end{aligned} \\
&\begin{aligned}A_{n-|S|}=(n-|S|)!.\end{aligned} \\
\\
&\mathsf{Hence}\sum_{S\subset\{1,...,n\},|S|=k}|\cap_{j\in S}A_j|= \\
&=\binom nk\cdot(n-k)!=\frac{n!}{(n-k)!k!}(n-k)!=\frac{n!}{k!}.
\end{aligned}
$$

$$\begin{aligned}

&\begin{aligned}d_n=|U|-\sum_i|A_i|+\sum_{i,j}|A_i\cap A_j|+ ...\end{aligned} \\
&\begin{aligned}=&n!-\frac{n!}{1!}+\frac{n!}{2!}-\ldots+(-1)^n\frac{n!}{n!}=\end{aligned} \\
&\begin{aligned}&=n!\left(1-\frac{1}{1!}+\frac{1}{2!}-\ldots+(-1)^n\frac{1}{n!}\right)\end{aligned} \\

\end{aligned}$$

### Anki
TARGET DECK: Math::Combinatorics  
START
Math prop
Question_eng: Derangements
Question_rus: Перестановки без неподвижных точек
Answer_eng: $$d_n=n!\left(1-\frac{1}{1!}+\frac{1}{2!}-\ldots+(-1)^n\frac{1}{n!}\right)$$
Answer_rus: 
Formula_main: Proof
$$
\begin{aligned}
&\begin{aligned}d_n=|U|-\sum_i|A_i|+\sum_{i,j}|A_i\cap A_j|+...\end{aligned} \\
&\begin{aligned}\textsf{If}S\subset\{1,\ldots,n\}\textsf{ let }M=\cap_{j\in S}A_j.\end{aligned} \\
&M\text{ is the set of permutations }\pi\text{ with} \\
&\begin{aligned}\pi(j)&=j\text{ for all }j\in S.&\textsf{Then }|M|&=\end{aligned} \\
&\begin{aligned}A_{n-|S|}=(n-|S|)!.\end{aligned} \\
\\
&\mathsf{Hence}\sum_{S\subset\{1,...,n\},|S|=k}|\cap_{j\in S}A_j|= \\
&=\binom nk\cdot(n-k)!=\frac{n!}{(n-k)!k!}(n-k)!=\frac{n!}{k!}.
\end{aligned}
$$

$$\begin{aligned}

&\begin{aligned}d_n=|U|-\sum_i|A_i|+\sum_{i,j}|A_i\cap A_j|+ ...\end{aligned} \\
&\begin{aligned}=&n!-\frac{n!}{1!}+\frac{n!}{2!}-\ldots+(-1)^n\frac{n!}{n!}=\end{aligned} \\
&\begin{aligned}&=n!\left(1-\frac{1}{1!}+\frac{1}{2!}-\ldots+(-1)^n\frac{1}{n!}\right)\end{aligned} \\

\end{aligned}$$

Formula_additional:
<!--ID: 1698688139448-->
END

START
Math prop
Question_eng: Approximate value of Derangements
Question_rus: 
Answer_eng: $$d_n\sim\frac{n!}e$$
Answer_rus: 
Formula_main: 
Formula_additional:
<!--ID: 1698688139452-->
END




$$d_n\sim\frac{n!}e$$



