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
\sum_{n=1}^{|S|} S_n
$$

<!--
- a set defined with set-builder notation:

$$
\sum_{ n \in \\{ i:\ i \in [a,b] \\} }
x_n
\quad = \quad
\sum_{n=a}^b x_n
$$
-->

## Subtracting with Sigma

- $\color{green}{a-b-c-d}$

$$
\begin{array}{c}
x_1 - \displaystyle\sum_{i=2}^{k}\ x_i
\\
\=
x_1 - x_2 - x_3 - x_4 - \cdots - x_k
\end{array}
$$

- $\color{green}{-a+b-c+d}$

$$
\begin{array}{c}
\displaystyle\sum_{i=1}^k\ x_i \cdot (-1)^i
\\
\=
-x_1 + x_2 - x_3 + x_4 \cdots x_k
\end{array}
$$

- $\color{green}{a-b+c-d}$

$$
\begin{array}{c}
\displaystyle\sum_{i=1}^k\ x_i \cdot (-1)^{i+1}
\\
\=
x_1 - x_2 + x_3 - x_4 \cdots x_k
\end{array}
$$

- $\color{green}{a+b-c+d}$

$$
\begin{array}{c}
2x_1 - \displaystyle\sum_{i=1}^k\ x_i \cdot (-1)^{i+1}
\\
\=
x_1 + x_2 - x_3 + x_4 \cdots x_k
\end{array}
$$

## Sigma-Sums Addition/Subtraction

$$
\left[
\sum_{n=s}^t f(n)
\right] \pm \left[
\sum_{n=s}^t g(n)
\right] = \sum_{n=s}^t
f(n) \pm g(n)
$$

$$
\color{green}{
(a+b) \pm (c+d) =
(a \pm c) + (b \pm d)
}
$$

- different intervals of the same length, i.e., $t_1-s_1 = t_2-s_2$:

$$
\left[
\sum_{i=s_1}^{t_1} x_i
\right] \pm \left[
\sum_{j=s_2}^{t_2} y_j
\right] = \sum_{i=s_1}^{t_1}
x_i y_{i+\Delta}
$$

$$
\iff \Delta = s_2 - s_1
$$

## Sigma-Sums Multiplication

$$
\left(
{\color{red}{\sum_{i=s_1}^{t_1}}\ \ x_i}
\right) \left(
{\color{blue}{\sum_{j=s_2}^{t_2}}\ \ y_j}
\right) =
{\color{red}{\sum_{i=s_1}^{t_1}}}
\ \ {\color{blue}{\sum_{j=s_2}^{t_2}}}
\ \ {\color{red} x_i} {\color{blue} y_j}
$$

$$
\color{green}{
(a+b)(c+d) = (ac+ad)+(bc+bd)
}
$$

## Sigma-Sums Swap

$$
{\color{red}{\sum_{i=s_1}^{t_1}}}
\ \ {\color{blue}{\sum_{j=s_2}^{t_2}}}
\ \ {\large{x_{i,j}}} =
{\color{blue}{\sum_{j=s_2}^{t_2}}}
\ \ {\color{red}{\sum_{i=s_1}^{t_1}}}
\ \ {\large{x_{i,j}}}
$$

$$
\begin{array}{c}
\color{green}{
(x_{1,2}+x_{1,3})+(x_{2,2}+x_{2,3}) =
}
\\
\color{green}{
(x_{1,2}+x_{2,2})+(x_{1,3}+x_{2,3})
}
\end{array}
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

#### Splitting a Sum Into Its Odd and Even Parts

- for even indexes:

$$
\sum_{n=2s}^{2t+1} x_n =
\sum_{n=s}^t x_{2n} +
\sum_{n=s}^t x_{2n+1}
$$

$$
\color{green}{
x_2 + x_3 + x_4 + x_5 =
(x_2 + x_4) + (x_3 + x_5)
}
$$

- for odd indexes:

$$
\sum_{n=2s+1}^{2t} x_n =
\sum_{n=s+1}^t x_{2n} +
\sum_{n=s+1}^t x_{2n-1}
$$

$$
\color{green}{
x_1 + x_2 + x_3 + x_4 =
(x_2 + x_4) + (x_1 + x_3)
}
$$

### Commutativity and Associativity

$$
\begin{array}{ll}
\displaystyle\sum_{k \leq j \leq i \leq n}
a_{i,j} & =
\displaystyle\sum_{i=k}^n
\displaystyle\sum_{j=k}^i
a_{i,j}
\\
& = \displaystyle\sum_{j=k}^n
\displaystyle\sum_{i=j}^n
a_{i,j}
\\
& = \displaystyle\sum_{j=0}^{n-k}
\displaystyle\sum_{i=k}^{n-j} a_{i+j,i}
\end{array}
$$

### Functions

#### Exponential

The exponential of a sum is the product of the exponential of the summands.

> it also applies for base other than $e$

$$
{\Large e^{
\Sigma_{n=s}^t\ f(n)
}} = \prod_{n=s}^t {\large e^{f(n)}}
$$

$$
\color{green}{
c^{a+b} = c^a \cdot c^b
}
$$

$$
{\Large e^{
f(s)-\Sigma_{n=s+1}^t\ f(n)
}} =
{\large e^{f(s)}} \cdot
\prod_{n=s+1}^t {\large \frac{1}{e^{f(n)}}}
$$

$$
\color{green}{
c^{a-b} = \frac{c^a}{c^b}
}
$$

#### Logarithm

The logarithm of a product is the sum of the logarithms of the factors.

$$
\sum_{n=s}^t \log_b(f(n)) =
\log_b\left(\prod_{n=s}^t f(n)\right)
$$

$$
\color{green}{
\log_n(a) + \log_n(b) = \log_n(ab)
}
$$

$$
\log_b(f(s)) - \sum_{n=s+1}^t
\log_b(f(n)) =
\log_b \left(
f(s) \cdot
\prod_{n=s+1}^t \frac{1}{f(n)}
\right)
$$

$$
\color{green}{
\log_n(a) - \log_n(b) = \log_n\left(\frac{a}{b}\right)
}
$$

#### Bijection $f: A \to B$

$$
\sum_{x \in A} f(x) =
\sum_{y \in B} y
$$

$$
\color{green}
\begin{array}{c}
A_1 + A_2 = B_1 + B_2
\\
\iff
\\
A = \\{ x_i\ |\ i \in \Bbb{N}, x_i \in \Bbb{R} \\}
\\
B = \\{ y_i\ |\ i \in \Bbb{N}, y_i = f(x_i) \\}
\end{array}
$$

$$
\sum_{y \in B} f^{-1}(y) =
\sum_{x \in A} x
$$

$$
\color{green}
\begin{array}{c}
B_1 + B_2 = A_1 + A_2
\\
\iff
\\
B = \\{ y_i\ |\ i \in \Bbb{N}, y_i \in \Bbb{R} \\}
\\
A = \\{ x_i\ |\ i \in \Bbb{N}, x_i = f^{-1}(y_i) \\}
\end{array}
$$

#### Function $f$ From $\Bbb{Z} \times \Bbb{Z}$

$$
\sum_{m=0}^k
\sum_{n=0}^m
f(m,n) =
\sum_{m=0}^k
\sum_{n=m}^k
f(n,m)
$$

$$
\color{green}
\begin{array}{l}
f(0,0) + \Bigl(f(1,0) + f(1,1)\Bigr) +
\\
\Bigl(f(2,0) + f(2,1) + f(2,2)\Bigr) =
\\
\Bigl(f(0,0) + f(1,0) + f(2,0)\Bigr) +
\\
\Bigl(f(2,1) + f(1,1)\Bigr) + f(2,2)
\end{array}
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



