# Matrix Multiplication

- matrices $A$ and $B$ can be multiplied only if a number of columns in $A$ equals a number of rows in $B$

$$
\large
A_{m \times {\color{green}n}} \cdot B_{{\color{green}n} \times p}
$$

- if $C$ is the resultant matrix ($A \cdot B$):
  - a number of its rows equals a number of rows in $A$
  - a number of its columns equals a number of columns in $B$

$$
\large
A_{{\color{red}m} \times n} \cdot B_{n \times {\color{blue}p}} = C_{{\color{red}m} \times {\color{blue}p}}
$$

> multiplication of matrices is not commutative, i.e., $AB \neq BA$

## Multiplication of Matrices

$$
\begin{bmatrix}
{\color{red}a_{11}} & {\color{red}a_{12}} & {\color{red}a_{13}}
\\
{\color{blue}a_{21}} & {\color{blue}a_{22}} & {\color{blue}a_{23}}
\end{bmatrix} \cdot \begin{bmatrix}
{\color{green}b_{11}} & {\color{purple}b_{12}}
\\
{\color{green}b_{21}} & {\color{purple}b_{22}}
\\
{\color{green}b_{31}} & {\color{purple}b_{32}}
\end{bmatrix} =
$$

$$
\begin{bmatrix}
{\color{red}a_{11}}{\color{green}b_{11}} +
{\color{red}a_{12}}{\color{green}b_{21}} +
{\color{red}a_{13}}{\color{green}b_{31}}
&
{\color{red}a_{11}}{\color{purple}b_{12}} +
{\color{red}a_{12}}{\color{purple}b_{22}} +{\color{red}a_{13}}{\color{purple}b_{32}}
\\
{\color{blue}a_{21}}{\color{green}b_{11}} +
{\color{blue}a_{22}}{\color{green}b_{21}} +
{\color{blue}a_{23}}{\color{green}b_{31}}
&
{\color{blue}a_{21}}{\color{purple}b_{12}} +
{\color{blue}a_{22}}{\color{purple}b_{22}} +{\color{blue}a_{23}}{\color{purple}b_{32}}
\end{bmatrix}
$$

### Example

$$
\begin{bmatrix}
{\color{red}1} & {\color{red}2} & {\color{red}3}
\\
{\color{blue}3} & {\color{blue}4} & {\color{blue}5}
\end{bmatrix} \cdot \begin{bmatrix}
{\color{green}2} & {\color{purple}4}
\\
{\color{green}3} & {\color{purple}1}
\\
{\color{green}4} & {\color{purple}2}
\end{bmatrix} =
$$

$$
\begin{bmatrix}
{\color{red}1}\cdot{\color{green}2} +
{\color{red}2}\cdot{\color{green}3} +
{\color{red}3}\cdot{\color{green}4}
&
{\color{red}1}\cdot{\color{purple}4} +
{\color{red}2}\cdot{\color{purple}1} +
{\color{red}3}\cdot{\color{purple}2}
\\
{\color{blue}3}\cdot{\color{green}2} +
{\color{blue}4}\cdot{\color{green}3} +
{\color{blue}5}\cdot{\color{green}4}
&
{\color{blue}3}\cdot{\color{purple}4} +
{\color{blue}4}\cdot{\color{purple}1} +{\color{blue}5}\cdot{\color{purple}2}
\end{bmatrix} =
$$

$$
\begin{bmatrix}
20 & 12
\\
38 & 26
\end{bmatrix}
$$

## Alternative Representation

Having the following function:

$$
\lambda\binom{R}{C} = R_1C_1 + R_2C_2 + \cdots + R_nC_n
$$

Multiplication of matrices $A$ and $B$ can be represented as follows:

$$
AB = \begin{bmatrix}
\lambda\binom{\text{A row }1}{\text{B col }1}
&
\lambda\binom{\text{A row }1}{\text{B col }2}
&
\cdots
&
\lambda\binom{\text{A row }1}{\text{B col }p}
\\
\ 
\\
\lambda\binom{\text{A row }2}{\text{B col }1}
&
\lambda\binom{\text{A row }2}{\text{B col }2}
&
\cdots
&
\lambda\binom{\text{A row }2}{\text{B col }p}
\\
\ 
\\
\vdots & \vdots & \ddots & \vdots
\\
\ 
\\
\lambda\binom{\text{A row }m}{\text{B col }1}
&
\lambda\binom{\text{A row }m}{\text{B col }2}
&
\cdots
&
\lambda\binom{\text{A row }m}{\text{B col }p}
\end{bmatrix}
$$

## JavaScript Implementation

```
function multiply(A,B) {
  const colsA = A[0].length;
  const rowsB = B.length;
  if (colsA !== rowsB) {
    throw new Error('incompatible matrices');
  }
 
  const rowsA = A.length;
  const colsB = B[0].length;
  const C = initNullMatrix(rowsA,colsB);
 
  for (let i=0; i<rowsA; i++) {
    for (let j=0; j<colsB; j++) {
      let sum = 0;
      for (let k=0; k<colsA; k++) {
        sum += A[i][k] * B[k][j];
      }
      C[i][j] = sum;
    }
  }

  return C;
}

function initNullMatrix(m,n) {
  const M = [];
  for (let i=1; i<=m; i++) {
    M.push((new Array(n)).fill(0));
  }
  return M;
}
```

