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

## Equations of Lines of Rotated Ellipse

### Major Axis Line

$$
y = (x-h)\tan(\phi)+k
$$

or with explicit terms:

$$
\left|\begin{array}{l}
y = mx + i
\\
\ 
\\
m = \tan(\phi)
\\
i = k-mh
\end{array}\right.
$$

### Minor Axis Line

$$
y = \frac{h-x}{\tan(\phi)} + k = (h-x)\cot(\phi)+k
$$

or with explicit terms:

$$
\left|\begin{array}{l}
y = mx + i
\\
\ 
\\
m = -\cot(\phi)
\\
i = k-mh
\end{array}\right.
$$

### Latus Rectum and Directrix

Having function $\Gamma(x,\Delta)$:

$$
\Gamma(x,\Delta) = \left(h+\frac{
 \Delta(1+\tan^2(\phi))
}{
 \sqrt{1+\tan^2(\phi)}
}-x\right)\cot(\phi)+k
$$
