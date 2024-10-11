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
