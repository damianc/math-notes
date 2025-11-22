# Section Formula

The **section formula** finds the ratio in which a line segment is divided by a point.

## Internal Section

If point $\color{#f44}P$ lying on the line segment $\overline{AB}$ divides it in the ratio ${\color{#fa0}m}:{\color{purple}n}$, its coordinates are:

$$
{\color{#f44}P} = \left(
\frac{{\color{#fa0}m}x_B+{\color{purple}n}x_A}{{\color{#fa0}m}+{\color{purple}n}},
\frac{{\color{#fa0}m}y_B+{\color{purple}n}y_A}{{\color{#fa0}m}+{\color{purple}n}}
\right)
$$

[]

> $A{\color{#f44}P} : {\color{#f44}P}B = {\color{#fa0}m} : {\color{purple}n}$

## External Section

If point $\color{#f44}P$ lying on the extension of the line segment $\overline{AB}$ divides it in the ratio ${\color{#fa0}m}:{\color{purple}n}$, its coordinates are:

$$
{\color{#f44}P} = \left(
\frac{{\color{#fa0}m}x_B-{\color{purple}n}x_A}{{\color{#fa0}m}-{\color{purple}n}},
\frac{{\color{#fa0}m}y_B-{\color{purple}n}y_A}{{\color{#fa0}m}-{\color{purple}n}}
\right)
$$

[]

> $A{\color{#f44}P} : B{\color{#f44}P} = {\color{#fa0}m} : {\color{purple}n}$

> **VECTORS**
> 
> If $\vec{a}$ and $\vec{b}$ are position vectors of points $A$ and $B$, respectively, the position vector of a point $P$ is as follows:
> 
> $$\frac{m\vec{b} \pm n\vec{a}}{m \pm n}$$
> 
> **+** is for **internal section**  
> **-** is for **external section**

## Midpoint

The midpoint $\color{#f44}P$ - lying in the middle of the line segment $\overline{AB}$ - divides it internally in the ratio $1:1$, hence its coordinates are:

$$
{\color{#f44}P} = \left(
\frac{x_A+x_B}{2},
\frac{y_A+y_B}{2}
\right)
$$

> **OVERVIEW**
>
> With auxiliary function:
> 
> $$\lambda(m, n) = \left(\frac{mx_B+nx_A}{m+n},\frac{my_B+ny_A}{m+n}\right)$$
>
> - **internal section** is given by $\lambda(m, n)$
> - **external section** is given by $\lambda(m, -n)$
> - **midpoint** is given by $\lambda(1, 1)$

## Section in 3D

Given point $A = (x_1,y_1,z_1)$ and point $B = (x_2,y_2,z_3)$, the section formula gives the coordinates of point $P$ as:

$$
P = \left(
\frac{mx_2+nx_1}{m+n},
\frac{my_2+ny_1}{m+n},
\frac{mz_2+nz_1}{m+n}
\right)
$$

## Centroid

The centroid of a triangle is a point in which the medians intersect. Each median is divided in the ratio $2:1$.

For triangle $\triangle_{ABC}$, coordinates of its centroid are:

$$
P = \left(
\frac{x_A+x_B+x_C}{3},
\frac{y_A+y_B+y_C}{3}
\right)
$$
