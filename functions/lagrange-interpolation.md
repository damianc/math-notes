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
