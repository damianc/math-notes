# Matrix of Transformation 2D

Matrix of transformation has the following pattern:

$$
T = \begin{bmatrix}
sx & rx & tx
\\
ry & sy & ty
\\
0 & 0 & 1
\end{bmatrix}
$$

> _s_ - scale  
> _r_ - rotate  
> _t_ - translate

Coordinates of a point $P'$ being the point $P$ after applying the transformation $T$ is obtained by matrices multiplication:

$$
T \times \begin{bmatrix}
P_x
\\
P_y
\\ 1
\end{bmatrix} = \begin{bmatrix}
P'_x
\\
P'_y
\\
1
\end{bmatrix}
$$

It is:

$$
\begin{array}{l}
P'_x = (P_x \cdot sx) + (P_y \cdot rx) + tx
\\
P'_y = (P_x \cdot ry) + (P_y \cdot sy) + ty
\end{array}
$$

## Transformation Matrices

### Rotation by $\theta$ at $(0,0)$

$$
\begin{bmatrix}
\cos(\theta) & -\sin(\theta) & 0
\\
\sin(\theta) & \cos(\theta) & 0
\\
0 & 0 & 1
\end{bmatrix}
$$

### Rotation by $\theta$ at $(R_x,R_y)$

$$
\begin{bmatrix}
\cos(\theta) & -\sin(\theta) & R_x(1-\cos(\theta))+R_y \sin(\theta)
\\
\sin(\theta) & \cos(\theta) & R_y(1-\cos(\theta))-R_x \sin(\theta)
\\
0 & 0 & 1
\end{bmatrix}
$$

### Homothety with scale $s$ at $(R_x,R_y)$

$$
\begin{bmatrix}
s & 0 & R_x(1-s)
\\
0 & s & R_y(1-s)
\\
0 & 0 & 1
\end{bmatrix}
$$

### Skew-X by $\alpha$

$$
\begin{bmatrix}
1 & \tan(\alpha) & 0
\\
0 & 1 & 0
\\
0 & 0 & 1
\end{bmatrix}
$$

### Skew-Y by $\beta$

$$
\begin{bmatrix}
1 & 0 & 0
\\
\tan(\beta) & 1 & 0
\\
0 & 0 & 1
\end{bmatrix}
$$

### Skew-XY by $\alpha$ and $\beta$ (respectively)

$$
\begin{bmatrix}
1 & \tan(\alpha) & 0
\\
\tan(\beta) & 1 & 0
\\
0 & 0 & 1
\end{bmatrix}
$$

### Reflection by point $(R_x,R_y)$

$$
\begin{bmatrix}
-1 & 0 & 2R_x
\\
0 & -1 & 2R_y
\\
0 & 0 & 1
\end{bmatrix}
$$

### Reflection by horizontal line $y=n$

$$
\begin{bmatrix}
1 & 0 & 0
\\
0 & -1 & 2n
\\
0 & 0 & 1
\end{bmatrix}
$$

### Reflection by vertical line $x=m$

$$
\begin{bmatrix}
-1 & 0 & 2m
\\
0 & 1 & 0
\\
0 & 0 & 1
\end{bmatrix}
$$

### Reflection by line $y=mx+i$

$$
\frac{1}{1+m^2} \times \begin{bmatrix}
1-m^2 & 2m & -2mi
\\
2m & m^2-1 & 2i
\\
0 & 0 & 1
\end{bmatrix}
$$
