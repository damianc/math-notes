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

## Subtracting

$$
x_1 - \sum_{i=2}^{k} x_i =
x_1 - x_2 - x_3 - x_4 - \cdots - x_k
$$

$$
\sum_{i=1}^k (-1)^i x_i =
-x_1 + x_2 - x_3 + x_4 \cdots x_k
$$

$$
\sum_{i=1}^k (-1)^{i+1} x_i =
x_1 - x_2 + x_3 - x_4 \cdots x_k
$$

$$
2x_1 - \sum_{i=1}^k (-1)^{i+1} x_i =
x_1 + x_2 - x_3 + x_4 \cdots x_k
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

$$
\color{green}{
a+b+c+d
\ \ =\ \ 
d+c+b+a
}
$$

### Splitting a Sum

$$
\sum_{n=s}^t f(n)
\quad = \quad
\sum_{n=s}^j f(n) +
\sum_{n=j+1}^t f(n)
$$

$$
\color{green}{
a+b+c+d
\ \ =\ \ 
[a+b] + [c+d]
}
$$

- a variant with subtracting sum:

$$
\sum_{n=a}^b f(n)
\quad = \quad
\sum_{n=0}^b f(n) -
\sum_{n=0}^{a-1} f(n)
$$

$$
\color{green}{
c+d
\ \ =\ \ 
[a+b+c+d] - [a+b]
}
$$

### Integral Calculus

$$
{\Large \int} \left[
\sum_{i=1}^n f_i(x)
\right]
\ dx =
\sum_{i=1}^n \int f_i(x)\ dx
$$

$$
\color{green}{
{\tiny \int} f(x)+g(x)\ dx =
{\tiny \int} f(x)\ dx +
{\tiny \int} g(x)\ dx
}
$$

$$
\frac{\partial}{\partial x}
\left[
\sum_{i=1}^n f_i(x)
\right] =
\sum_{i=1}^n
{\small\frac{\partial}{\partial x}}
f_i(x)
$$

$$
\color{green}{
[f(x)+g(x)]' = f'(x) + g'(x)
}
$$



