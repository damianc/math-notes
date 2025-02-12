# Covariance

Covariance is a measure that shows the linear relationship between two random variables:

- $\text{cov} \gt 0$: as one variable increases, other variable also increases
- $\text{cov} \lt 0$: as one variable increases, other variable decreases
- $\text{cov} \approx 0$: there's not the linear relationship between variables (still, there can occur other type of relationship)

## Formula

$$
\begin{array}{rl}
\text{cov}(x,y) & = \frac{1}{N} \sum (x-\overline{x})(y-\overline{y})
\\
\ 
\\
& = \frac{1}{N} \left[
 \sum xy
\right] \overline{x} \overline{y}
\end{array}
$$

or in terms of the **expected value**:

$$
\begin{array}{rl}
\text{cov}(X,Y) & = E\bigl[
 (X-E[X])(Y-E[Y])
 \bigr]
 \\
 \ 
 \\
 & = E[XY]-E[X]E[Y]
\end{array}
$$
