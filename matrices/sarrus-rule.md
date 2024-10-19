# Sarrus' Rule

The **Sarrus' rule** allows getting the determinant of a matrix $3 \times 3$.

## Algorithm

For  matrix $M_{3 \times 3}$:

$$
M = \begin{bmatrix}
a & b & c
\\
d & e & f
\\
g & h & i
\end{bmatrix}
$$

1. Let matrix $\hat{M}$ be the matrix $M$ with the first and second column repeated:

$$
\hat{M} = \left[\begin{array}{ccc|cc}
a & b & c & a & b
\\
d & e & f & d & e
\\
g & h & i & g & h
\end{array}\right]
$$

2. Sum up products of three terms _diagonally adjacent_ and assign the resultant sum to $\Sigma_1$:

$$
\hat{M} = \left[\begin{array}{ccc|cc}
{\color{red}a} & {\color{green}b} & {\color{blue}c} & a & b
\\
d & {\color{red}e} & {\color{green}f} & {\color{blue}d} & e
\\
g & h & {\color{red}i} & {\color{green}g} & {\color{blue}h}
\end{array}\right]
$$

$$
\Sigma_1 = {\color{red}aei} + {\color{green}bfg} + {\color{blue}cdh}
$$

3. Sum up products of three terms _counter-diagonally adjacent_ and assign the resultant sum to $\Sigma_2$:

$$
\hat{M} = \left[\begin{array}{ccc|cc}
a & b & {\color{red}c} & {\color{green}a} & {\color{blue}b}
\\
d & {\color{red}e} & {\color{green}f} & {\color{blue}d} & e
\\
{\color{red}g} & {\color{green}h} & {\color{blue}i} & g & h
\end{array}\right]
$$

$$
\Sigma_2 = {\color{red}ceg} + {\color{green}afh} + {\color{blue}bdi}
$$

4. Subtract $\Sigma_2$ from $\Sigma_1$ to get the determinant of the matrix $M$:

$$
\det M = \Sigma_1 - \Sigma_2
$$

## Expansion

Everything can be put together as:

$$
\det M = {\color{red}aei} + {\color{green}bfg} + {\color{blue}cdh} - {\color{red}ceg} - {\color{green}afh} - {\color{blue}bdi}
$$

### Indexed Form Matrix

If matrix is represented with index notation:

$$
\begin{bmatrix}
a_{11} & a_{12} & a_{13}
\\
a_{21} & a_{22} & a_{23}
\\
a_{31} & a_{32} & a_{33}
\end{bmatrix}
$$

The sums of the products are as follows:

$$
\Sigma_1 = {\color{red}a_{11} a_{22} a_{33}} + {\color{green}a_{12} a_{23} a_{31}} + {\color{blue}a_{13} a_{21} a_{32}}
$$

$$
\Sigma_2 = {\color{red}a_{13} a_{22} a_{31}} + {\color{green}a_{11} a_{23} a_{32}} + {\color{blue}a_{12} a_{21} a_{33}}
$$

> as previously, $\det M = \Sigma_1 - \Sigma_2$


