# Integration by Parts: Exercise 6

$$
\large
\int xe^{-x} \ dx
$$

## Parts

$$
\int u \ dv = uv - \int v \ du
$$

$$
\begin{array}{lcl}
u = x && du = 1
\\
dv = e^{-x} && v = -e^{-x}
\end{array}
$$

## Solution

$$
\begin{array}{rl}
-xe^{-x} - \displaystyle\int -e^{-x} \ dx & = -xe^{-x} + \displaystyle\int e^{-x} \ dx
\\
& = -xe^{-x} + (-e^{-x})
\\
& = -xe^{-x} - e^{-x}
\\
& = -e^{-x} (x+1)
\\
& \equiv -\frac{x+1}{e^x}
\end{array}
$$

## Result

$$
\int xe^{-x} \ dx = -e^{-x} (x+1)
$$
