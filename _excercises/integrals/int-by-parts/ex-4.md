# Integration by Parts: Exercise 4

$$
\large
\int 4x^2 \ \ln(x) \ dx
$$

## Parts

$$
\int u \ dv = uv - \int v \ du
$$

$$
\begin{array}{lcl}
u=\ln(x) && du=\frac{1}{x}
\\
dv=4x^2 && v=\frac{4}{3} x^3
\end{array}
$$

## Solution

$$
\begin{array}{rl}
\frac{4}{3} x^3 \ln(x) - \displaystyle\int \frac{1}{x} \cdot \frac{4}{3}x^3 \ dx & = \frac{4}{3}x^3 \ln(x) - \displaystyle\int \frac{4x^3}{3x} \ dx
\\
& = \frac{4}{3}x^3 \ln(x) - \frac{4}{3} \displaystyle\int x^2 \ dx
\\
& = \frac{4}{3}x^3 \ln(x) - \frac{4}{3} \cdot \frac{x^3}{3}
\\
& = \frac{4}{3}x^3 \ln(x) - \frac{4}{9}x^3
\\
& = 4x^3\left( \frac{1}{3}\ln(x) - \frac{1}{9} \right)
\\
& \equiv \frac{4}{9}x^3(3 \ln(x)-1)
\end{array}
$$

## Result

$$
\int 4x^2 \ \ln(x) \ dx =  \frac{4}{9}x^3(3 \ln(x)-1)
$$
