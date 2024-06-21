# Barycentric Coordinates

Is a point $P$ within a triangle $\triangle_{ABC}$?

**SOLUTION**

$$
\begin{array}{l}
\Delta = (y_B-y_C)(x_A-x_C)+(x_C-x_B)(y_A-y_C)
\\
\Lambda(v,h) = v(x_P-x_C) + h(y_P-y_C)
\\
\\
\lambda_1 = \frac{1}{\Delta}[\Lambda(y_B-y_C,x_C-x_B)]
\\
\lambda_2 = \frac{1}{\Delta}[\Lambda(y_C-y_A,x_A-x_C)]
\\
\lambda_3 = 1 - \lambda_1 - \lambda_2
\\
\\
P \text{ is {\color{green} within} } \triangle_{ABC} \text{ if}:
\\
\quad
\underset{i\in\langle1,3\rangle}{\large\forall}
\lambda_i \in \langle0,1\rangle
{\ }\cap{\ }
\lambda_1\lambda_2\lambda_3 \neq 0
\\
\\
P \text{ is {\color{blue} on edge} of } \triangle_{ABC} \text{ if}:
\\
\quad
\underset{i\in\langle1,3\rangle}{\large\forall}
\lambda_i \in \langle0,1\rangle
{\ }\cap{\ } 
\lambda_1\lambda_2\lambda_3 = 0
\\
\\
P \text{ is {\color{red} beyond} } \triangle_{ABC} \text{ if}:
\\
\quad
\underset{i\in\langle1,3\rangle}{\large\exists}
\lambda_i \notin \langle0,1\rangle
\end{array}
$$

## Expansion

$$
\begin{array}{l}
\lambda_1 = \frac{1}{\Delta} [(y_B-y_C)(x_P-x_C)+(x_C-x_B)(y_P-y_C)]
\\
\lambda_2 = \frac{1}{\Delta} [(y_C-y_A)(x_P-x_C)+(x_A-x_C)(y_P-y_C)]
\\
\lambda_3 = 1-\lambda_1-\lambda_2
\end{array}
$$

## Implementation

```
function checkTriangle([A,B,C], [xp,yp]) {
  const [[xa,ya],[xb,yb],[xc,yc]] = [A,B,C];
  const D = (yb-yc)*(xa-xc)+(xc-xb)*(ya-yc);
  const f = (a,b) => a*(xp-xc)+b*(yp-yc);
	
  const L1 = f(yb-yc,xc-xb)/D;
  const L2 = f(yc-ya,xa-xc)/D;
  const L3 = 1-L1-L2;
	
  const L = [L1,L2,L3];
  const vl = L.filter(x => x >= 0 && x <= 1);
	
  if (vl.length === 3) {
    const m = L.reduce((acc,curr) => acc*curr,1);
    if (m !== 0) return 'within';
    else return 'on';
  } else {
    return 'beyond';
  }
}
```

use:

```
const A = [2,3];
const B = [6,7];
const C = [4,10];

const points = [
  [5,7], [5,8], [4,5], [5,6], [6,8]
];
const res = points.map(p => {
  return `(${p}): ${
    checkTriangle([A,B,C],p)
  }`;
});

console.log(res);
/*
[
  "(5,7): within",
  "(5,8): within",
  "(4,5): on",
  "(5,6): on",
  "(6,8): beyond"
]
*/
```

![Checking points](https://github.com/damianc/math-notes/blob/master/_images/coords/barycentric-coords.png)


