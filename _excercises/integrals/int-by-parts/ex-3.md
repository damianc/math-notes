# Integration by Parts: Exercise 3

$$
\large
\int 2x \ \sin(x) \ dx
$$

## Parts

$$
\int u \ dv = uv - \int v \ du
$$

$$
\begin{array}{lcl}
u=2x && du=2
\\
dv=\sin(x) && v=-\cos(x)
\end{array}
$$

## Solution

$$
\begin{array}{rl}
-2x \cos(x) - \displaystyle\int -2 \cos(x) \ dx & = -2x \cos(x) + 2 \displaystyle\int \cos(x) \ dx
\\
& = -2x \cos(x) + 2 \sin(x)
\\
& = 2 \sin(x) - 2x \cos(x)
\\
& = 2(\sin(x) - x \cos(x))
\end{array}
$$

## Result

$$
\int 2x \ \sin(x) \ dx = 2(\sin(x) - x \cos(x))
$$
