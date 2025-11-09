# Kronecker Product

The **Kronecker product** takes every term of matrix $A$ and multiplies matrix $B$ by it.

$$
A_{m \times n} \otimes B_{p \times q} = \begin{bmatrix}
a_{11}B & a_{12}B & \cdots & a_{1n}B
\\
a_{21}B & a_{22}B & \cdots & a_{2n}B
\\
\vdots & \vdots & \ddots & \vdots
\\
a_{m1}B & a_{m2}B & \cdots & a_{mn}B
\end{bmatrix}_{pm \times qn}
$$

## Examples

### Example 1

$$
\begin{bmatrix}
1 & 2
\end{bmatrix} \otimes \begin{bmatrix}
\alpha & \beta
\\
\gamma & \delta
\end{bmatrix}
$$

$$
= \begin{bmatrix}
1\begin{bmatrix}
\alpha & \beta
\\
\gamma & \delta
\end{bmatrix} & 2\begin{bmatrix}
\alpha & \beta
\\
\gamma & \delta
\end{bmatrix}
\end{bmatrix}
$$

$$
= \left[\begin{array}{cc|cc}
\alpha & \beta & 2\alpha & 2\beta
\\
\gamma & \delta & 2\gamma & 2\delta
\end{array}\right]
$$

### Example 2

$$
\begin{bmatrix}
1 & 2
\\
3 & 4
\end{bmatrix} \otimes \begin{bmatrix}
0 & 5
\\
4 & 10
\end{bmatrix}
$$

$$
= \begin{bmatrix}
1\begin{bmatrix}
0 & 5
\\
4 & 10
\end{bmatrix} & 2\begin{bmatrix}
0 & 5
\\
4 & 10
\end{bmatrix}
\\
\ 
\\
3\begin{bmatrix}
0 & 5
\\
4 & 10
\end{bmatrix} & 4\begin{bmatrix}
0 & 5
\\
4 & 10
\end{bmatrix}
\end{bmatrix}
$$

$$
= \left[\begin{array}{cc|cc}
0 & 5 & 0 & 10
\\
4 & 10 & 8 & 20
\\
\hline
0 & 15 & 0 & 20
\\
12 & 30 & 16 & 40
\end{array}\right]
$$
