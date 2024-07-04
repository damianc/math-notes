# Summation

## Constant Term

### Constant Multiplier

$$
\sum_{n=s}^t {\color{red}k}f(n)
\quad = \quad
{\color{red}k} \sum_{n=s}^t f(n)
$$

$$
\sum_{n=s}^t \frac{f(n)}{{\color{red}k}}
\quad = \quad
\frac{\displaystyle\sum_{n=s}^t f(n)}{{\color{red}{k}}}
$$

### Constant Summand

$$
\sum_{n=s}^t {\color{red}k} + f(n)
\quad = \quad
\Delta{\color{red}k} +
\sum_{n=s}^t f(n)
$$

$$
\sum_{n=s}^t {\color{red}k} - f(n)
\quad = \quad
\Delta{\color{red}k} -
\sum_{n=s}^t f(n)
$$

$$
\sum_{n=s}^t f(n) - {\color{red}k}
\quad = \quad
\left[\sum_{n=s}^t f(n)\right] -
\Delta{\color{red}k}
$$

> $\Delta = t-s+1$

## Index Shift

$$
\sum_{n=s}^t f(n)
\quad = \quad
\sum_{n=s \pm {\color{red}p}}^{t \pm {\color{red}p}}
f(n \mp {\color{red}p})
$$

- it can be generalized - for a bijection $\lambda$ from a finite set $A$ onto a set $B$ ($\lambda: A \rightarrow B$):

$$
\sum_{n \in B} f(n)
\quad = \quad
\sum_{m \in A} f({\color{red}\lambda}(m))
$$




