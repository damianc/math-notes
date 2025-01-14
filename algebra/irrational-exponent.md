# Irrational Exponent

> When exponent is an irrational number, some identities must be employeed:
>
> - $1.234\dots = 1+0.2+0.03+0.004+\cdots$
> - $k^{a+b} = k^a \cdot k^b$
> - $k^{\frac{m}{n}} = \sqrt[n]{k^m}$

Example for the $\pi$ exponent:

$$
\large
\begin{array}{rl}
k^{\pi} & = k^{3.1415\dots}
\\
\ 
\\
& = k^{3+0.1+0.04+0.001+0.0005+\cdots}
\\
\ 
\\
& = k^3 \cdot k^{0.1} \cdot k^{0.04} \cdot k^{0.001} \cdot k^{0.0005} \cdot \ \cdots
\\
\ 
\\
& = k^3 \cdot k^{\frac{1}{10}} \cdot k^{\frac{4}{100}} \cdot k^{\frac{1}{1000}} \cdot k^{\frac{5}{10000}} \cdot \ \cdots
\\
\ 
\\
& = k^3 \cdot k^{\frac{1}{10}} \cdot k^{\frac{1}{25}} \cdot k^{\frac{1}{1000}} \cdot k^{\frac{1}{2000}} \cdot \ \cdots
\\
\ 
\\
& = k^3 \cdot \sqrt[10]{k} \cdot \sqrt[25]{k} \cdot \sqrt[1000]{k} \cdot \sqrt[2000]{k} \cdot \ \cdots
\end{array}
$$

## Generalization

- having defined the $\partial p$ function:

$$
\partial p(n,i) = \lfloor n \cdot 10^i \rfloor \bmod 10
$$

- $k^n$ can be defined as:

$$
\Large
k^n = \prod_{i=0}^{\infty}
k^{\frac{\partial p(n,i)}{10^i}} \equiv \prod_{i=0}^{\infty} \sqrt[10^i]{k^{\partial p(n,i)}}
$$

> more often than not, $\infty$ can be replaced with some small number like $4$ or $10$, depending on how accurate the result is expected to be
