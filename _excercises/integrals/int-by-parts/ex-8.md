# Integration by Parts: Exercise 8

$$
\large
\int \frac{1+x^2}{x} \ dx
$$

> It can be easily split into $\int \frac{1}{x} + x \ dx$, nonetheless the below is to practise the integration by parts.

## Parts

$$
\int u \ dv = uv - \int v \ du
$$

$$
\begin{array}{lcl}
u = 1+x^2 && du = 2x
\\
dv = \frac{1}{x} && v = ln(x)
\end{array}
$$

## Solution

$$
\begin{array}{rl}
& (1+x^2)\ln(x) - \displaystyle\int 2x\ln(x) \ dx
\\
\ 
\\
& \quad u' = \ln(x), \ du' = \frac{1}{x}
\\
& \quad dv' = 2x, \ v' = x^2
\\
\ 
\\
& \quad x^2 \ln(x) - \int \frac{x^2}{x} \ dx
\\
& \quad \ = x^2 \ln(x) - \int x \ dx
\\
& \quad \ = x^2 \ln(x) - \frac{1}{2} x^2
\\
& \quad \ = x^2\left(\ln(x)-\frac{1}{2}\right)
\\
\ 
\\
= & (1+x^2) \ln(x) - x^2\left(\ln(x)-\frac{1}{2}\right)
\\
\ 
\\
= & \ln(x)+x^2 \ln(x)-x^2 \ln(x)+\frac{1}{2}x^2
\\
\ 
\\
= & \frac{1}{2}x^2+\ln(x)
\end{array}
$$

## Result

$$
\int \frac{1+x^2}{x} \ dx = \frac{1}{2} x^2 + \ln(x)
$$
