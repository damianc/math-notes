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

## Location of Special Points of Rotated Ellipse

| Points | Location |
|--|--|
| foci | $$F_{1,2} = (h \pm c \cos(\phi), k \pm c \sin(\phi))$$ |
| vertices | $$V_{1,2} = (h \pm a \cos(\phi), k \pm a \sin(\phi))$$ |
| co-vertices | $$W_{1,2} = (h \mp b \sin(\phi), k \pm b \cos(\phi))$$ |

> $c = \sqrt{a^2-b^2}$

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

Rotated ellipse lines are described as follows:

- latus rectum: $LR_{1,2} = \Gamma(x,\pm c)$ for $c=\sqrt{a^2-b^2}$
- directrix: $D_{1,2} = \Gamma(x,\pm d)$ for $d=\frac{a^2}{c}$
- minor axis: $\Gamma(x,0)$
