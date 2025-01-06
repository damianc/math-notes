# Integration by Parts: Exercise 2

$$
\large
\int x^2 \ e^x \ dx
$$

## Parts

$$
\int u \ dv = uv - \int v \ du
$$

$$
\begin{array}{lcl}
u=x^2 && du=2x
\\
dv=e^x && v=e^x
\end{array}
$$

## Solution

$$
\begin{array}{rl}
x^2 \ e^x - \displaystyle\int 2x \ e^x \ dx & = x^2 \ e^x - 2e^x(x-1)
\\
& = e^x(x^2-2(x-1))
\\
& = e^x(x^2-2x+2)
\end{array}
$$

> Solution for $\int 2x \ e^x \ dx$ is [here](https://github.com/damianc/math-notes/blob/master/_excercises/integrals/int-by-parts/ex-1.md)

## Result

$$
\int x^2 \ e^x \ dx = e^x(x^2-2x+2)
$$


