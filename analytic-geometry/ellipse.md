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

## Formulas

### Surface Area

$$
S = \pi ab
$$

### Circumference

A circumference of an ellipse can be obtained with use of [the complete elliptic integral of the second kind](https://en.m.wikipedia.org/wiki/Elliptic_integral#Complete_elliptic_integral_of_the_second_kind):

$$
\begin{array}{rl}
\ell & = 4a\ E(e)
\\
\ 
\\
& = 4a \displaystyle\int_0^{\frac{\pi}{2}}
\sqrt{1-e^2\sin^2\theta}\ d\theta
\end{array}
$$

$$
\text{where } e = \sqrt{1-\left(\frac{b}{a}\right)^2}
$$

#### Circumference Approximation

- approximation:

$$
\ell \approx \pi\left(
 \frac{3}{2} (a+b) - \sqrt{ab}
\right)
$$

- more accurate approximation:

$$
\begin{array}{rl}
\ell & \approx \pi[
 3(a+b)-\sqrt{(3a+b)(a+3b)}
\Bigr]
\\
\ 
\\
& = \pi \Bigl[
3(a+b)-\sqrt{3(a+b)^2+4ab}
\Bigr]
\end{array}
$$

- even more accurate approximation:

$$
\begin{array}{c}
\ell \approx \pi\Bigl(a+b\Bigr)\left(
1+\frac{3h}{10+\sqrt{4-3h}}
\right)
\\
\ 
\\
\text{where } h = \frac{(a-b)^2}{(a+b)^2}
\end{array}
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

> given $d_1(P) = |PF_1|$ and $d_2(P) = |PF_2|$:
>   
> $\underset{P \in E}{\forall} d_1(P) + d_2(P) = 2a$

![Sum of Distances from Foci](https://raw.githubusercontent.com/damianc/math-notes/refs/heads/master/_images/anal-geom/ellipse/ellipse-dists-sum.png)

$$
{\color{#2ae} d_1} + {\color{#2ae} d_2} = {\color{purple} 2a}
$$

### Special Case

when $P=(h,k \pm b)$, then $d_1 = d_2 = a$

![Sum of Equal Distances from Foci](https://raw.githubusercontent.com/damianc/math-notes/refs/heads/master/_images/anal-geom/ellipse/ellipse-dists-sum-special.png)

## Ellipse Components

![Ellipse Components](https://raw.githubusercontent.com/damianc/math-notes/refs/heads/master/_images/anal-geom/ellipse/ellipse-components.jpg)

**major axis** ($2a$)  
- the longest diameter of the ellipse
- passing through both foci ($F_1$ and $F_2$)
- vertices ($V_1$ and $V_2$) are its endpoints
- the longer axis of symmetry of the ellipse

**minor axis** ($2b$)  
- the shortest diameter of the ellipse
- perpendicular to the _major axis_ at its center
- co-vertices ($W_1$ and $W_2$) are its endpoints
- the shorter axis of symmetry of the ellipse

**semi-major axis** (denoted as $a$)  
half of the _major axis_, extending from the center to either vertex

**semi-minor axis** (denoted as $b$)  
half of the _minor axis_, extending from the center to either co-vertex

**foci**  
two fixed points on the _major axis_ whose distance from the center of the ellipse is $c$ (_linear eccentricity_ below)

$$
F_{1,2} = (h \pm c, k)
$$

**linear eccentricity** (denoted as $c$)  
the distance from the center of the ellipse to either focus ($F_1$ or $F_2$)

$$
c = \sqrt{a^2 - b^2} = ae
$$

**eccentricity** (denoted as $e$)  
a number between $0$ and $1$ that describes the shape of the ellipse (with $0$ being a circle); the ratio of the focal distance ($c$) to the _semi-major axis_ ($a$)

$$
e = \frac{c}{a} = \sqrt{1-\left(\frac{b}{a}\right)^2}, {\text{for }} a \gt b
$$

**vertex**  
one of two points where the _major axis_ intersects the ellipse, i.e., one of endpoints of the _major axis_

$$
V_{1,2} = (h \pm a, k)
$$

**co-vertex**  
one of two points where the _minor axis_ intersects the ellipse, i.e., one of endpoints of the _minor axis_

$$
W_{1,2} = (h, k \pm b)
$$

**latus rectum** (denoted as $l$)  
a line segment ($l$ in length) perpendicular to the _major axis_ and passing through a focus, with both endpoints on the ellipse

$$
l = \frac{2b^2}{a}
$$

**semi-latus rectum** (denoted as $\ell$)  
half the length of the _latus rectum_

$$
\ell = \frac{b^2}{a} = a(1-e^2)
$$

### Directrices

**directrix**  
a line outside the ellipse perpendicular to the _major axis_ whose distance from the center of the ellipse is $d$

$$
d = \frac{a^2}{c}
$$

![Ellipse Directrices](https://raw.githubusercontent.com/damianc/math-notes/refs/heads/master/_images/anal-geom/ellipse/ellipse-directrix.png)

#### Properties of Directrices

For every point $P$ there are two points related to it:

$$
\begin{array}{l}
D_1 = (h+d, P_y)
\\
D_2 = (h-d, P_y)
\\
\text{where } d = \frac{a^2}{c}
\end{array}
$$

For which the following properties hold:

$$
\begin{array}{rl}
\because & d_1 = e \cdot |PD_1|
\\
& d_2 = e \cdot |PD_2|
\\
\ 
\\
\therefore & d_1+d_2 = e(|PD_1|+|PD_2|) = 2a
\\
\ 
\\
\therefore & |PD_1| = \frac{d_1}{e}
\\
& |PD_2| = \frac{d_2}{e}
\\
\ 
\\
& e = \frac{d_1}{|PD_1|} = \frac{d_2}{|PD_2|}
\end{array}
$$
