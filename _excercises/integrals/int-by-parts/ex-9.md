# Integration by Parts: Exercise 9

$$
\large
\int x^2 \sin(x) \ dx
$$

## Parts

$$
\int u \ dv = uv - \int v \ du
$$

$$
\begin{array}{lcl}
u = x^2 && du = 2x
\\
dv = \sin(x) && v = -\cos(x)
\end{array}
$$

## Solution

$$
\begin{array}{rl}
& -x^2 \cos(x) - \displaystyle\int -2x \cos(x) \ dx
\\
= & -x^2 \cos(x) + 2 \displaystyle\int x \cos(x) \ dx
\\
= & 2\left[\displaystyle\int x \cos(x) \ dx \right] - x^2 \cos(x)
\\
\ 
\\
& \quad u'=x, \ du'=1
\\
& \quad dv' = \cos(x), \ v' = \sin(x)
\\
\ 
\\
& \quad x \sin(x) - \int \sin(x) \ dx
\\
& \quad \ = x \sin(x) + \cos(x)
\\
\ 
\\
= & 2(x \sin(x) + \cos(x)) - x^2 \cos(x)
\\
= & 2x \sin(x) + 2 \cos(x) - x^2 \cos(x)
\\
= & 2x \sin(x) + (2-x^2)\cos(x)
\\
\equiv & 2x \sin(x) - (x^2-2)\cos(x)
\end{array}
$$

## Result

$$
\int x^2 \sin(x) \ dx = 2x \sin(x) + (2-x^2)\cos(x)
$$
