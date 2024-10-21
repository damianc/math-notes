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

## JavaScript Implementation

```
function det(M,R=1) {
  const rows = M.length;
  const cols = M[0].length;
  if (rows !== cols) {
    throw new Error('square matrix must be passed');
  }

  if (M.length === 1) return M[0][0];
  if (M.length === 2) {
    const [[a,b],[c,d]] = M;
    return a*d-b*c;
  }

  // Sarrus' rule for matrix 3x3
  if (M.length === 3) {
    const [
      [a,b,c],
      [d,e,f],
      [g,h,i]
    ] = M;
    const s1 = a*e*i+b*f*g+c*d*h;
    const s2 = a*f*h+b*d*i+c*e*g;
    return s1-s2;
  }

  // Laplace expansion for matrix 4x4 and more
  const r = M[R-1].map((v,j) => {
    const col = j+1;
    const p = (-1)**(R+col);
    const m = minor(M,R,col);
    return p * v * m;
  });
  return r.reduce((a,c) => a+c,0);
}
```

> [`minor()`](https://github.com/damianc/math-notes/blob/master/matrices/matrix-minor.md#javascript-implementation)

