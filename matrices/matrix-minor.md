# Matrix Minor

Minor $M_{ij}$ of element $a_{ij}$ is the determinant of a matrix created by removal of _i-th_ row and _j-th_ column of the matrix the element belongs to.

For example, for matrix $A$:

$$
A = \begin{bmatrix}
a & b & c
\\
d & e & f
\\
g & h & i
\end{bmatrix}
$$

Minor of element $a_{12}$ is:

$$
M_{12} = \begin{bmatrix}
{\color{#ccc}a} & {\color{#ccc}b} & {\color{#ccc}c}
\\
d & {\color{#ccc}e} & f
\\
g & {\color{#ccc}h} & i
\end{bmatrix} = \begin{vmatrix}
d & f
\\
g & i
\end{vmatrix} = di-fg
$$

## Minor Matrix

Minor matrix $M$ is a matrix where element $a_{ij}$ is replaced with its minor $M_{ij}$.

For example, for matrix $B$:

$$
B = \begin{bmatrix}
1 & 2
\\
3 & 4
\end{bmatrix}
$$

Minors of its elements are:

$$
\begin{matrix}
M_{11} = \begin{vmatrix}
{\color{#ccc}1} & {\color{#ccc}2}
\\
{\color{#ccc}3} & {4}
\end{vmatrix} = 4
&
M_{12} = \begin{vmatrix}
{\color{#ccc}1} & {\color{#ccc}2}
\\
{3} & {\color{#ccc}4}
\end{vmatrix} = 3
\\
\ 
\\
M_{21} = \begin{vmatrix}
{\color{#ccc}1} & {2}
\\
{\color{#ccc}3} & {\color{#ccc}4}
\end{vmatrix} = 2
&
M_{22} = \begin{vmatrix}
{1} & {\color{#ccc}2}
\\
{\color{#ccc}3} & {\color{#ccc}4}
\end{vmatrix} = 1
\end{matrix}
$$

Therefore the final minor matrix $M$ is:

$$
M = \begin{bmatrix}
M_{11} & M_{12}
\\
M_{21} & M_{22}
\end{bmatrix} = \begin{bmatrix}
4 & 3
\\
2 & 1
\end{bmatrix}
$$

## JavaScript Implementation

```
function minor(M,i,j) {
  return det(minorize(M,i,j));
}

function minorize(M,i,j) {
  const rows = M.length;
  const cols = M[0].length;
  if (
    i < 1 || j < 1 ||
    i > rows || j > cols
  ) {
    throw new Error(
      `invalid index [${i}][${j}]`
    );
  }

  const m = [];
  for (let row=1; row <= rows; row++) {
    if (row === i) continue;
    const currRow = [];
    for (let col=1; col <= cols; col++) {
      if (col === j) continue;
      currRow.push(M[row-1][col-1]);
    }
    m.push(currRow);
  }
  return m;
}
```

> [`det()`](https://github.com/damianc/math-notes/blob/master/matrices/matrix-determinant.md#javascript-implementation)

