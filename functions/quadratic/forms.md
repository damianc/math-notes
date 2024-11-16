# Forms of Quadratic Functions

#### standard/general form:

$$
y = ax^2+bx+c
$$

#### vertex form:

$$
y = a(x-p)^2+q
$$

#### intercept/factored form:

$$
y = a(x-x_1)(x-x_2)
$$

$$
\text{or}
$$

$$
y = a(x-x_0)^2
$$

## Conversion

### From Standard Form

#### To Vertex Form

$$
\begin{array}{l}
ax^2+bx+c \quad \mapsto \quad a(x-p)^2+q
\\
\ 
\\
p = \frac{-b}{2a}
\\
q = c-ap^2
\end{array}
$$

#### To Intercept Form

$$
\begin{array}{l}
ax^2+bx+c \quad \mapsto \quad
a(x-x_1)(x-x_2)
\\
\ 
\\
x_{1,2} = \frac{-b\pm\sqrt{\Delta}}{2a}
\quad \iff \Delta \ge 0
\\
\Delta = b^2-4ac
\end{array}
$$

### From Vertex Form

#### To Standard Form

$$
\begin{array}{l}
a(x-p)^2+q \quad \mapsto \quad ax^2+bx+c
\\
\ 
\\
b = -2ap
\\
c = ap^2+q
\end{array}
$$

#### To Intercept Form

$$
\begin{array}{l}
a(x-p)^2+q \quad \mapsto \quad a(x-x_1)(x-x_2)
\\
\ 
\\
b = -2ap
\\
c = ap^2+q
\\
x_{1,2} = \frac{-b\pm\sqrt{\Delta}}{2a}
\quad \iff \Delta \ge 0
\\
\Delta = b^2-4ac
\end{array}
$$

### From Intercept Form

#### To Standard Form

$$
\begin{array}{l}
a(x-x_1)(x-x_2) \quad \mapsto \quad ax^2+bx+c
\\
\ 
\\
b = -a(x_1 + x_2)
\\
c = ax_1x_2
\end{array}
$$

#### To Vertex Form

$$
\begin{array}{l}
a(x-x_1)(x-x_2) \quad \mapsto \quad a(x-p)^2+q
\\
\ 
\\
p = \frac{x_1 + x_2}{2}
\\
q = -a(p-x_1)^2
\end{array}
$$

## JavaScript Implementation

```
function standardToVertex(a, b, c) {
  const p = -b / (2*a);
  const q = c - a * (p**2);

  return { a, p, q };
}

function standardToIntercept(a, b, c) {
  const { sqrt } = Math;
  const delta = (b**2) - 4*a*c;

  if (delta < 0) {
    return null;
  } else if (delta === 0) {
    const x0 = -b/(2*a);
    return { a, x0 };
  } else {
    const x1 = (-b-sqrt(delta))/(2*a);
    const x2 = (-b+sqrt(delta))/(2*a);
    return { a, x1, x2 };
  }
}

function vertexToStandard(a, p, q) {
  const b = -2*a*p;
  const c = a * (p**2) + q;

  return { a, b, c };
}

function vertexToIntercept(a, p, q) {
  const {b,c} = vertexToStandard(a, p, q);
  return standardToIntercept(a, b, c);
}

function interceptToStandard(a, x1, x2) {
  const b = -a*(x1 + x2);
  const c = a*x1*x2;

  return { a, b, c };
}

function interceptToVertex(a, x1, x2) {
  const p = (x1+x2) / 2;
  const q = -a * ((p-x1)**2);

  return { a, p, q };

  // or
  // const {b,c} = interceptToStandard(a, x1, x2);
  // return standardToVertex(a, b, c);
}
```
