# Matrix Determinant

> Determinant of a matrix can be obtained with the [**Laplace expansion**](https://github.com/damianc/math-notes/blob/master/matrices/laplace-expansion.md).
>
> For matrix $3 \times 3$ [**Sarrus' rule**](https://github.com/damianc/math-notes/blob/master/matrices/sarrus-rule.md) can be used.

## Matrix 1x1

$$
\begin{vmatrix}a\end{vmatrix} = a
$$

## Matrix 2x2

$$
\begin{vmatrix}
a & b
\\
c & d
\end{vmatrix} = ad-bc
$$

## Matrix 3x3

$$
M_{3 \times 3} = \begin{bmatrix}
a & b & c
\\
d & e & f
\\
g & h & i
\end{bmatrix}
$$

$$
\begin{array}{rl}
\det M_{3 \times 3} = & a(ei-fh)\ -
\\
& b(di-fg)\ +
\\
& c(dh-eg)
\end{array}
$$

## Matrix 4x4

$$
M_{4 \times 4} = \begin{bmatrix}
a & b & c & d
\\
e & f & g & h
\\
i & j & k & l
\\
m & n & o & p
\end{bmatrix}
$$

$$
\begin{array}{rl}
\det M_{4 \times 4} = & (af-be)(kp-lo)\ +
\\
& (ah-de)(jo-kn)\ +
\\
& (bg-cf)(ip-lm)\ +
\\
& (ce-ag)(jp-ln)\ +
\\
& (ch-dg)(in-jm)\ +
\\
& (df-bh)(io-km)
\end{array}
$$


