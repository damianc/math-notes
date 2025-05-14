# Integration by Parts: Exercise 7

$$
\large
\int x \ln(x) \ dx
$$

## Parts

$$
\int u \ dv = uv - \int v \ du
$$

$$
\begin{array}{lcl}
u = \ln(x) && du = \frac{1}{x}
\\
dv = x && v = \frac{1}{2} x^2
\end{array}
$$

## Solution

$$
\begin{array}{rl}
\frac{1}{2} x^2 \ln(x) - \displaystyle\int \frac{x^2}{2} \cdot \frac{1}{x} \ dx & = \frac{1}{2} x^2 \ln(x) - \displaystyle\int \frac{1}{2} x \ dx
\\
& = \frac{1}{2} x^2 \ln(x) - \frac{1}{2} \displaystyle\int x \ dx
\\
& = \frac{1}{2} x^2 \ln(x) - \frac{1}{2} \cdot \frac{1}{2} x^2
\\
\ 
\\
& = \frac{1}{2} x^2 \ln(x) - \frac{1}{4} x^2
\\
\ 
\\
& = \frac{1}{2} x^2 \left( \ln(x) - \frac{1}{2} \right)
\\
\ 
\\
& \equiv \frac{1}{4} x^2 (2 \ln(x) - 1)
\end{array}
$$

## Result

$$
\int x \ln(x) \ dx = \frac{1}{2} x^2 \left( \ln(x) - \frac{1}{2} \right)
$$
