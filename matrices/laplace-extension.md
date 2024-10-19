# Laplace Extension

The **Laplace extension** allows getting the determinant of a matrix.

## Algorithm

1. Pick terms of the first row of a matrix $M_{n \times n}$ (nonetheless, it can be other row or even column)
2. Multiply every term by its minor
3. Multiply every resultant product by the positional factor $(-1)^{i+j}$

$$
R = \\{
(a_{1j} \cdot M_{1j}) \cdot (-1)^{1+j}
\ |\  1 \le j \le n
\\}
$$

4. Sum up everything

$$
\det M = \sum_{t \in R} t
$$

## Example

For matrix $M_{3 \times 3}$:

$$
M = \begin{bmatrix}
a_{11} & a_{12} & a_{13}
\\
a_{21} & a_{22} & a_{23}
\\
a_{31} & a_{32} & a_{33}
\end{bmatrix}
$$

1. Pick terms of the first row of the matrix $M$:

$$
\large
R = \\{
a_{11}, a_{12}, a_{13}
\\}
$$

> we can pick terms of other row (or even column) - it does not have to be the first one

2. Multiply every term by its minor:

$$
\large
R_m = \\{
{\color{red}m_1},
{\color{green}m_2},
{\color{blue}m_3}
\\}
$$

where:

$$
\begin{array}{rl}
{\color{red}m_1} = a_{11} \times M_{11} & = a_{11} \times \begin{vmatrix}
a_{22} & a_{23}
\\
a_{32} & a_{33}
\end{vmatrix}
\\
& = a_{11}(a_{22}a_{33}-a_{23}a_{32})
\end{array}
$$

$$
\begin{array}{rl}
{\color{green}m_2} = a_{12} \times M_{12} & = a_{12} \times \begin{vmatrix}
a_{21} & a_{23}
\\
a_{31} & a_{33}
\end{vmatrix}
\\
& = a_{12}(a_{21}a_{33}-a_{23}a_{31})
\end{array}
$$

$$
\begin{array}{rl}
{\color{blue}m_3} = a_{13} \times M_{13} & = a_{13} \times \begin{vmatrix}
a_{21} & a_{22}
\\
a_{31} & a_{32}
\end{vmatrix}
\\
& = a_{13}(a_{21}a_{32}-a_{22}a_{31})
\end{array}
$$

3. Multiply every resultant product by the positional factor $(-1)^{1+j}$:

$$
\large
R_p = \\{
{\color{red}p_1},
{\color{green}p_2},
{\color{blue}p_3}
\\}
$$

where:

$$
\begin{array}{rl}
{\color{red}p_1} & = {\color{red}m_1} \times (-1)^{1+1} = {\color{red}m_1}
\\
& = a_{11}(a_{22}a_{33}-a_{23}a_{32})
\end{array}
$$

$$
\begin{array}{rl}
{\color{green}p_2} & = {\color{green}m_2} \times (-1)^{1+2} = {\color{green}-m_2}
\\
& = -a_{12}(a_{21}a_{33}-a_{23}a_{31})
\end{array}
$$

$$
\begin{array}{rl}
{\color{blue}p_3} & = {\color{blue}m_3} \times (-1)^{1+3} = {\color{blue}m_3}
\\
& = a_{13}(a_{21}a_{32}-a_{22}a_{31})
\end{array}
$$

4. Sum up everything to get the determinant of the matrix $M$:

$$
\begin{array}{rl}
\det M & = \displaystyle\sum_{p \in R_p} p = {\color{red}p_1} + {\color{green}p_2} + {\color{blue}p_3}
\\
\ 
\\
& = \ \ \ \ {\color{red}a_{11}(a_{22}a_{33}-a_{23}a_{32})}
\\
& \ \ \ \ {\color{green}-\ a_{12}(a_{21}a_{33}-a_{23}a_{31})}
\\
& \ \ \ \ {\color{blue}+\ a_{13}(a_{21}a_{32}-a_{22}a_{31})}
\end{array}
$$

