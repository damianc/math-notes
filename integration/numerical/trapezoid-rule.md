# Trapezoid Rule

The **trapezoid(al) rule** is a technique for numerical integration, i.e. approximating the definite integral; area of the region under the graph is approximated by area of trapezoids under it.

![Trapezoid rule](https://raw.githubusercontent.com/damianc/math-notes/refs/heads/master/_images/integration/num-int-trapezoids.jpg)

$$
\int_a^b f(x) \ dx \approx
\frac{1}{2} \Delta
\sum_{i=1}^n (y_{i-1} + y_i)
$$

or just:

$$
\int_a^b f(x) \ dx \approx
\Delta\left(
\frac{y_0 + y_n}{2} +
\sum_{i=1}^{n-1} y_i
\right)
$$

> $y_i = f(a+i\Delta)$  
> $\Delta = \frac{b-a}{n}, \quad n \in \Bbb{N}$
