# Matrix Cofactors

A cofactor of element $a_{ij}$ is its minor multiplied by positional factor $(-1)^{i+j}$:

$$
\large
C_{ij} = (-1)^{i+j} \cdot M_{ij}
$$

For example for matrix $M$, cofactor of the element $a_{11}$ is $C_{11}$:


$$
M = \begin{bmatrix}
1 & 2 & 3
\\
4 & 5 & 6
\\
7 & 8 & 9
\end{bmatrix}
$$

$$
\begin{array}{rl}
C_{11} & = (-1)^{1+1} \cdot \begin{vmatrix}
5 & 6
\\
8 & 9
\end{vmatrix}
\\
& = (-1)^2 \cdot (5 \cdot 9 - 6 \cdot 8)
\\
& = 1 \cdot (45-48)
\\
& = 1 \cdot (-3) = -3
\end{array}
$$

## Cofactor Matrix 
Cofactor matrix is a matrix that consists of cofactors of all elements of the original matrix:

$$
\begin{array}{rl}
A_c & = \begin{bmatrix}
C_{11} & C_{12} & \cdots
\\
C_{21} & C_{22} & \cdots
\\
\vdots & \vdots & \ddots
\end{bmatrix}
\\
\ 
\\
& = \begin{bmatrix}
(-1)^2 \cdot M_{11} & (-1)^3 \cdot M_{12} & \cdots
\\
(-1)^3 \cdot M_{21} & (-1)^4 \cdot M_{22} & \cdots
\\
\vdots & \vdots & \ddots
\end{bmatrix}
\\
\ 
\\
& = \begin{bmatrix}
M_{11} & -M_{12} & \cdots
\\
-M_{21} & M_{22} & \cdots
\\
\vdots & \vdots & \ddots
\end{bmatrix}
\end{array}
$$

## Positional Factor

- for **odd** rows:
  - **odd** columns have **positive** _positional factor_
  - **even** columns have **negative** _positional factor_
- for **even** rows:
  - **odd** columns have **negative** _positional factor_
  - **even** columns have **positive** _positional factor_

 The very first _positional factor_ is positive and other ones are distributed so that they form a checkerboard:
 
 $$
 \begin{bmatrix}
 {\color{green}+} & {\color{red}-} &  {\color{green}+} & {\color{red}-} & \cdots
 \\
{\color{red}-} &  {\color{green}+} & {\color{red}-} & {\color{green}+} & \cdots
\\
 {\color{green}+} & {\color{red}-} &  {\color{green}+} & {\color{red}-} & \cdots
 \\
 {\color{red}-} &  {\color{green}+} & {\color{red}-} & {\color{green}+} & \cdots
 \\
 \vdots & \vdots & \vdots & \vdots & \ddots
 \end{bmatrix}
 $$

 ## JavaScript Implementation

```
function cofactor(M,i,j) {
  const m = minor(M,i,j);
  return (-1)**(i+j) * m;
}

function cofactors(M) {
  return M.map((row,i) => {
    return row.map((_,j) => {
      return cofactor(M,i+1,j+1);
    });
  });
}
```

> [`minor()`](https://github.com/damianc/math-notes/blob/master/matrices/matrix-minor.md#javascript-implementation)
