# Rotated Ellipse

![Rotated Ellipse](https://raw.githubusercontent.com/damianc/math-notes/refs/heads/master/_images/anal-geom/ellipse/rotated-ellipse.png)

## Equation

$$
\frac{
 ((x-h)\cos(\phi)+(y-k)\sin(\phi))^2
}{a^2} + \frac{
 ((x-h)\sin(\phi)-(y-k)\cos(\phi))^2
}{b^2} = 1
$$

splitting up:

$$
\begin{array}{l}
{\large\frac{\partial_E^x}{a^2} +
\frac{\partial_E^y}{b^2} = 1}
\\
\\
\partial_E^x = ((x-h)\cos(\phi)+(y-k)\sin(\phi))^2
\\
\partial_E^y = ((x-h)\sin(\phi)-(y-k)\cos(\phi))^2
\end{array}
$$

## Point on Rotated Ellipse

![Point on Rotated Ellipse](https://raw.githubusercontent.com/damianc/math-notes/refs/heads/master/_images/anal-geom/ellipse/rotated-ellipse-point-location.png)

$$
\begin{cases}
P_x = a \cos(\phi) \cos(\theta) - b \sin(\phi) \sin(\theta) + h
\\
P_y = a \cos(\theta) \sin(\phi) + b \sin(\theta) \cos(\phi) + k
\end{cases}
$$
