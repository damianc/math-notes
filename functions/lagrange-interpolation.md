# Lagrange Interpolation

**Lagrange interpolation** finds a polynomial function whose graph passes through given points. That is, by a set of points $(x_1,y_1),(x_2,y_2),\dots,(x_n,y_n)$, we can find such a function $P(x)$ for which the following holds:

  $$
  \begin{cases}
  y_1 = P(x_1)
  \\
  y_2 = P(x_2)
  \\
  \dots
  \\
  y_n = P(x_n)
  \end{cases}
  $$
  
  ## Formula

$$
\large
P(x) = \sum_{i=1}^n y_i \ell_i(x), \quad 
\ell_i(x) = \prod_{j \neq i}  \frac{x-x_j}{x_i-x_j}  $$

### Related Articles

- [Finding a Line by Two Points](https://github.com/damianc/math-notes/blob/master/analytic-geometry/finding-line.md#by-two-points)
- [Finding a Parabola by Roots and Vertex](https://github.com/damianc/math-notes/blob/master/functions/quadratic/constructing-parabola.md)

## Expansion

- For two points $(x_1,y_1), (x_2,y_2)$:

$$
\begin{array}{rl}
P(x) & = y_1\left(
\frac{x-x_2}{x_1-x_2}
\right) + y_2\left(
\frac{x-x_1}{x_2-x_1}
\right)
\\
\ 
\\
& = \frac{
y_1(x-x_2)(x_2-x_1)+y_2(x-x_1)(x_1-x_2)
}{
-(x_1-x_2)^2
}
\\
\ 
\\
& = \frac{
(x_1-x_2)(y_1(x-x_2)-y_2(x-x_1))
}{
-(x_1-x_2)^2
}
\\
\ 
\\
& = \frac{
y_2(x-x_1)-y_1(x-x_2)
}{
x_2-x_1
}
\end{array}
$$

- For three points $(x_1,y_1), (x_2,y_2), (x_3,y_3)$:

$$
\begin{array}{rl}
P(x) & = y_1\left(
\frac{x-x_2}{x_1-x_2} \frac{x-x_3}{x_1-x_3}
\right) + y_2\left(
\frac{x-x_1}{x_2-x_1} \frac{x-x_3}{x_2-x_3}\right) + y_3\left(
\frac{x-x_1}{x_3-x_1} \frac{x-x_2}{x_3-x_2}
\right)
\\
\ 
\\
& = \frac{y_1(x-x_2)(x-x_3)}{(x_1-x_2)(x_1-x_3)} +
\frac{y_2(x-x_1)(x-x_3)}{(x_2-x_1)(x_2-x_3)} +
\frac{y_3(x-x_1)(x-x_2)}{(x_3-x_1)(x_3-x_2)}
\end{array}
$$
