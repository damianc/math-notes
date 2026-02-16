# Spherical Cap/Dome, Sector and Segment

## Spherical Cap/Dome

![Spherical Cap](https://raw.githubusercontent.com/damianc/math-notes/refs/heads/master/_images/figures/sphere/sphere-spherical-cap.jpg)


### Volume and Surface Area

| | using $r$ and $h$ | using $a$ and $h$ | using $r$ and $\theta$ |
|--|--|--|--|
| volume | $$\frac{1}{3} \pi h^2(3r-h)$$ | $$\frac{1}{6} \pi h(3a^2+h^2)$$ | $$\frac{1}{3} \pi r^3 (2+\cos(\theta))(1-\cos(\theta))^2$$ |
| surface area (lateral) | $$2\pi rh$$ | $$\pi (a^2+h^2)$$ | $$2\pi r^2(1-\cos(\theta))$$ |
| constraints | $0 \leq h \leq 2r$ | $a \geq 0, \ h \geq 0$ | $r \geq 0, \ \theta \in [0,\pi]$ |

### Other Properties

$$
\begin{array}{l}
\sin(\theta) = \frac{a}{r}
\\
\cos(\theta) = 1-\frac{h}{r}
\\
\tan(\theta) = \frac{a}{r-h}
\\
\ 
\\
a = \sqrt{r^2-(r-h)^2} = \sqrt{h(2r-h)} = r \sin(\theta) = (r-h) \tan(\theta)
\\
h = r(1-\cos(\theta)) = r-\frac{a}{\tan(\theta)}
\\
r = \frac{h}{1-\cos(\theta)} = \frac{a}{\sin(\theta)} = \frac{a}{\tan(\theta)} + h
\\
\ 
\\
2hr = a^2+h^2
\\
2ha = (a^2+h^2) \sin(\theta)
\end{array}
$$

## Spherical Sector

![Spherical Cap](https://raw.githubusercontent.com/damianc/math-notes/refs/heads/master/_images/figures/sphere/sphere-spherical-sector.jpg)

> Simply put, **a spherical sector** can be thought of as **a spherical cap/dome together with a cone**.

### Volume

$$
V = \frac{2}{3} \pi r^2h = \frac{2}{3} \pi r^3 (1-\cos(\theta))
$$

Using **the lateral surface area of the spherical cap** $S$:

$$
V = \frac{1}{3} r \cdot S
$$

### Surface Area

$$
S = 2\pi rh + \pi ra = \pi r(2h+a)
$$

## Spherical Segment/Zone

![Spherical Cap](https://raw.githubusercontent.com/damianc/math-notes/refs/heads/master/_images/figures/sphere/sphere-spherical-segment.jpg)

### Volume of a Spherical Segment

$$
V = \frac{1}{6} \pi h(3a^2 + 3b^2 + h^2)
$$

### Surface Area of a Spherical Zone

$$
S = 2 \pi rh
$$

> The radius can be obtained from the following equation:
> 
> $r^2 = a^2 + \left(
\frac{a^2-b^2-h^2}{2h}
\right)^2$

- formulas hold even if _a_/_b_ are swapped
- planes don't have to lay on the same hemisphere

## Integrals in Spherical Coordinates

![Sphere Sector](https://raw.githubusercontent.com/damianc/math-notes/refs/heads/master/_images/figures/sphere/sphere-simple-sector.jpg)

### Double Integral

The double integral gives **the lateral surface area of the spherical cap/dome**:

$$
\begin{array}{ll}
S_{\text{cap}} & = \rho^2 \displaystyle \int_0^{2\pi} \int_0^{\alpha} \sin(\varphi) \ d\varphi \ d\theta
\\
\ 
\\
& = 2\pi\rho^2 (1-\cos(\alpha))
\end{array}
$$

### Triple Integral

The triple integral gives **the volume of the spherical sector**:

$$
\begin{array}{ll}
V_{\text{sector}} & = \displaystyle \int_0^{2\pi} \int_0^{\alpha} \int_0^{\rho} r^2 \sin(\varphi) \ dr \ d\varphi \ d\theta
\\
\ 
\\
& = \frac{2}{3}\pi\rho^3 (1-\cos(\alpha))
\end{array}
$$
