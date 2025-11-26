# Line Intersection

> formulas for $A$, $B$ and $C$ are below this section

$$
\Delta = B^2-4AC
$$

- if $\Delta \lt 0$: there is not intersection
- if $\Delta = 0$: there is 1 intersection point $x_0=\frac{-B}{2A}$
- if $\Delta \gt 0$: there are 2 intersection points $x_{1,2} = \frac{-B\pm\sqrt{\Delta}}{2A}$

## Intersection with Parabola

![Intersection of line and parabola](https://raw.githubusercontent.com/damianc/math-notes/refs/heads/master/_images/anal-geom/intersection/line-intersection-with-parabola.png)

$$
\begin{array}{l}
A = a
\\
B = b-m
\\
C = c-i
\end{array}
$$

## Intersection with Hyperbola

![Intersection of line and hyperbola](https://raw.githubusercontent.com/damianc/math-notes/refs/heads/master/_images/anal-geom/intersection/line-intersection-with-hyperbola.png)

$$
\begin{array}{l}
A = mc
\\
B = ic+md-a
\\
C = id-b
\end{array}
$$

## Intersection with Circle

![Intersection of line and circle](https://raw.githubusercontent.com/damianc/math-notes/refs/heads/master/_images/anal-geom/intersection/line-intersection-with-circle.png)

$$
\begin{array}{l}
A = 1+m^2
\\
B = 2((i-b)m-a)
\\
C = a^2 + (b-i)^2 - r^2
\end{array}
$$

- for a circle with center at $(0,0)$:

$$
\begin{array}{l}
A = 1+m^2
\\
B = 2im
\\
C = i^2-r^2
\end{array}
$$

> Alternatively, with translation of the circle with center at $(a,b)$ to $(0,0)$:  
>  
> $t=i+ma-b$  
> $A=1+m^2$  
> $B=2mt$  
> $C=t^2-r^2$  
> $\Delta=B^2-4AC$  
> $x_{1,2}=\frac{-B \pm \sqrt{\Delta}}{2A} + a$

## Intersection with Ellipse

![Intersection of line and ellipse](https://raw.githubusercontent.com/damianc/math-notes/refs/heads/master/_images/anal-geom/intersection/line-intersection-with-ellipse.png)

$$
\begin{array}{l}
\varphi = \left(\frac{b}{a}\right)^2
\\
A = m^2 + \varphi
\\
B = 2((i-k)m-\varphi h)
\\
C = (i-k)^2-b^2+\varphi h^2
\end{array}
$$

- for an ellipse with center at $(0,0)$:

$$
\begin{array}{l}
A = m^2+\left(\frac{b}{a}\right)^2
\\
B = 2im
\\
C = i^2-b^2
\end{array}
$$

> Alternatively, with translation of the ellipse with center at $(h,k)$ to $(0,0)$:  
>  
> $t=i+mh-k$  
> $A=b^2+a^2m^2$  
> $B=2a^2mt$  
> $C=a^2(t^2-b^2)$  
> $\Delta=B^2-4AC$  
> $x_{1,2} = \frac{-B \pm \sqrt{\Delta}}{2A}+h$

## Intersection with Rotated Ellipse

![Intersection of line and rotated ellipse](https://raw.githubusercontent.com/damianc/math-notes/refs/heads/master/_images/anal-geom/intersection/line-intersection-with-rotated-ellipse.png)

In case of rotated ellipse a little bit more math must be done:
- let the ellipse and the intersecting line be a system $E$, then unrotate it and move to $(0,0)$
- get intersection points
- move to $(h,k)$ and rotate back given points with respect to the center of the ellipse $(h,k)$

To begin with, define functions that rotate a point relative to the center of the ellipse:

$$
\begin{array}{rl}
\lambda(\theta,f_c,f_s,f_1,f_2)  &= f_c \cos(\theta) + f_s \sin(\theta)
\\
& + \ f_1 (1-\cos(\theta))
\\
& + \ f_2 \sin(\theta)
\end{array}
$$

$$
\Gamma_x(x,y,\theta) = \lambda(\theta,x,-y,h,k)
$$

$$
\Gamma_y(x,y,\theta) = \lambda(\theta,y,x,k,-h)
$$

Reset rotation and translation of the ellipse and move the line along with it:

$$
\begin{array}{l}
g(x) = nx+j
\\
n = \tan(\arctan(m)-\phi)
\\
j = nh + (\partial_g - k)
\\
\partial_g = \Gamma_y(0,i,-\phi) - n \cdot \Gamma_x(0,i,-\phi)
\end{array}
$$

Get intersection points:

$$
\begin{array}{l}
A = n^2 + \left(\frac{b}{a}\right)^2
\\
B = 2nj
\\
C = j^2 - b^2
\\
\Delta = B^2 - 4AC
\\
\ 
\\
x'\_{1,2} = \frac{-B \pm \sqrt{\Delta}}{2A}
\\
y'\_{1,2} = g(x'_{1,2})
\end{array}
$$

Move and rotate these points back:

$$
\begin{cases}
x_1 = \Gamma_x(x'_1+h, y'_1+k, \phi)
\\
y_1 = \Gamma_y(x'_1+h, y'_1+k, \phi)
\end{cases}
$$

$$
\begin{cases}
x_2 = \Gamma_x(x'_2+h, y'_2+k, \phi)
\\
y_2 = \Gamma_y(x'_2+h, y'_2+k, \phi)
\end{cases}
$$


