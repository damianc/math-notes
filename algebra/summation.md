# Summation

- explicit boundaries:

$$
\sum_{n=s}^t x_n
\quad = \quad
x_s + x_{s+1} + x_{s+2} + \cdots + x_t
$$

- boundaries as inequality:

$$
\sum_{a \leq n \leq b} x_n
\quad = \quad
\sum_{n=a}^b x_n
$$

- summing terms of a set:

$$
\sum_{n \in S} n
\quad = \quad
\sum_{n=1}^{\overline{\overline S}} S_n
$$

- a set defined with set-builder notation:

$$
\sum_{ n \in \\{ i:\ i \in [a,b] \\} }
x_n
\quad = \quad
\sum_{n=a}^b x_n
$$

## Identities

### Constant Term

#### Constant Multiplier

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

#### Constant Summand

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

### Index Shift

$$
\sum_{n=s}^t f(n)
\quad = \quad
\sum_{n=s \pm {\color{red}p}}^{t \pm {\color{red}p}}
f(n \mp {\color{red}p})
$$

- it can be generalized - for a bijection ${\color{red}\lambda}$ from a finite set $A$ onto a set $B$:

$$
\sum_{n \in B} f(n)
\quad = \quad
\sum_{m \in A} f({\color{red}\lambda}(m))
$$

> ${\color{red}\lambda}: A \rightarrow B$

### Direction of Summation

The sum from the first term up to the last is equal to the sum from the last down to the first.

$$
\sum_{n=s}^t f(n)
\quad = \quad
\sum_{n=0}^{t-s} f(t-n)
$$

$$
\sum_{n=0}^t f(n)
\quad = \quad
\sum_{n=0}^t f(t-n)
$$

### Splitting a Sum

$$
\sum_{n=s}^t f(n)
\quad = \quad
\sum_{n=s}^j f(n) +
\sum_{n=j+1}^t f(n)
$$

- a variant with subtracting sum:

$$
\sum_{n=a}^b f(n)
\quad = \quad
\sum_{n=0}^b f(n) -
\sum_{n=0}^{a-1} f(n)
$$



