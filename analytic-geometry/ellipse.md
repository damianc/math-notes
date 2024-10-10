# Ellipse

![Ellipse](https://raw.githubusercontent.com/damianc/math-notes/refs/heads/master/_images/anal-geom/ellipse/ellipse-basic-scheme.png)

## Equation

> Given:
> - $a$ - semi-major axis (or: the longest radius)
> - $b$ - semi-minor axis (or: the shortest radius)
> - $(h,k)$ - the center of the ellipse

$$
\frac{(x-h)^2}{a^2} + \frac{(y-k)^2}{b^2} = 1
$$

For an ellipse with center at $(0,0)$:

$$
\frac{x^2}{a^2} + \frac{y^2}{b^2} = 1
$$

## Point on Ellipse

![Point on Ellipse](https://raw.githubusercontent.com/damianc/math-notes/refs/heads/master/_images/anal-geom/ellipse/ellipse-point-location.png)

$$
\begin{cases}
P_x = a \cos(\theta) + h
\\
P_y = b \sin(\theta) + k
\end{cases}
$$

## Definition

An ellipse is a set of points where the sum of the distances to two fixed points (foci: $F_1$ and $F_2$) is constant and equal to $2a$ (length of the major axis).

$$
E = \left\\{
 P \in \mathbb{R}^2:
 |PF_1| + |PF_2| = 2a
\right\\}
$$

![Sum of Distances from Foci](https://raw.githubusercontent.com/damianc/math-notes/refs/heads/master/_images/anal-geom/ellipse/ellipse-dists-sum.png)

$$
{\color{#2ae} d_1} + {\color{#2ae} d_2} = {\color{purple} 2a}
$$
