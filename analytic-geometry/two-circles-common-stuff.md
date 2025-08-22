# Common Points and Area of Two Circles

> if $|r_1-r_2| \lt d \lt r_1+r_2$, circles have 2 common points
>
> if $d = |r_1 \pm r_2|$, circles have 1 common point

## Common Points

If two circles have common points, $P$ and $Q$, their coordinates are:

$$
\large
\left[\begin{array}{l}
x_{P,Q} = x_M \mp h \cdot \frac{y_B-y_A}{d}
\\
y_{P,Q} = y_M \pm h \cdot \frac{x_B-x_A}{d}
\end{array}\right.
$$

where:

- $d$ is distance between centers of the circles:

$$
d = \sqrt{
(x_A-x_B)^2 + (y_A-y_B)^2
}
$$

- $h$ is half the length of the $\overline{\text{PQ}}$ chord:

$$
h = \sqrt{r_1^2 - p^2}
$$

- $(x_M,y_M)$ is the center of the $\overline{\text{PQ}}$ chord :

$$
\left[\begin{array}{l}
x_M = x_A + p \cdot \frac{x_B-x_A}{d}
\\
y_M = y_A + p \cdot \frac{y_B-y_A}{d}
\end{array}\right.
$$

- $p$ is the length of the $\overline{\text{AM}}$ line segment:

$$
p = \frac{r_1^2-r_2^2+d^2}{2d}
$$

> In formulas above, we can refer to an angle:  
> $\frac{x_B-x_A}{d} = \cos(\alpha) = \sin(\beta)$  
> $\frac{y_B-y_A}{d} = \sin(\alpha) = \cos(\beta)$

### With Auxiliary Function

$$
\left[\begin{array}{l}
x_{P,Q} = C_{\beta}(C_{\alpha}(x_A,p), \mp h)
\\
y_{P,Q} = C_{\alpha}(C_{\beta}(y_A,p), \pm h)
\end{array}\right.
$$

$$
\iff
$$

$$
\begin{array}{rl}
C_{\theta}(\nu, \rho) & = \nu + \rho \cos(\theta)
\\
& = \nu + \rho \sin\left(
\frac{1}{2}\pi - \theta
\right)
\end{array}
$$

> $p$ and $h$ remain the same as above

## Length of the Chord

If $\ell$ is the length of the $\overline{\text{PQ}}$ chord, its value can be defined:

- with $h$:

$$
\ell = 2h
$$

- with $p$:

$$
\ell = 2r_1 \sqrt{
1-\left(
\frac{p}{r_1}
\right)^2
}
$$

- explicitly:

$$
\ell = 2r_1 \sqrt{1-\left(
\frac{r_1^2 - r_2^2 + d^2}{2dr_1}
\right)^2}
$$

- or:

$$
\ell = \frac{1}{d} \sqrt{
((r_1+r_2)^2 - d^2)(d^2 - (r_1-r_2)^2)
}
$$

## Area of the Common Region

If two circles partially overlap, area of the common region is:

$$
\large
A = a_1 + a_2 - k
$$

where:

- $a_1$ and $a_2$ are defined as follows:

$$
a_1 = r_1^2 \arccos\left(
\frac{d^2 + r_1^2 - r_2^2}{2dr_1}
\right)
$$

$$
a_2 = r_2^2 \arccos\left(
\frac{d^2 + r_2^2 - r_1^2}{2dr_2}
\right)
$$

- $k$ is defined as follows:

$$
\begin{array}{rl}
k & = \frac{d\ell}{2}
\\
\ 
\\
& = \frac{1}{2} \sqrt{
((r_1+r_2)^2 - d^2)(d^2 - (r_1-r_2)^2)
}
\end{array}
$$

### With Auxiliary Function

With the auxiliary function:

$$
\theta(\rho,\nu) = \rho^2 \arccos\left(
\frac{d^2 + \rho^2 - \nu^2}{2d\rho}
\right)
$$

$a_1$ and $a_2$ can be defined as follows:

$$
\begin{array}{l}
a_1 = \theta(r_1,r_2)
\\
a_2 = \theta(r_2,r_1)
\end{array}
$$
