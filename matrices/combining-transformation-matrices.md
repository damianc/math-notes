# Combining Transformation Matrices

Transformation matrices $T_1$ and $T_2$:

$$
T_1 = \begin{bmatrix}
sx_1 & rx_1 & tx_1
\\
ry_1 & sy_1 & ty_1
\\
0 & 0 & 1
\end{bmatrix}
$$

$$
T_2 = \begin{bmatrix}
sx_2 & rx_2 & tx_2
\\
ry_2 & sy_2 & ty_2
\\
0 & 0 & 1\end{bmatrix}$$

can be combined by multiplication:

$$
T_1 \times T_2 = \begin{bmatrix}
sx_1sx_2+rx_1ry_2 & sx_1rx_2+rx_1sy_2 & sx_1tx_2+rx_1ty_2+tx_1
\\
ry_1sx_2+sy_1ry_2 & ry_1rx_2+sy_1sy_2 & ry_1tx_2+sy_1ty_2+ty_1
\\
0 & 0 & 1
\end{bmatrix}
$$

## Application to Point

$$
[T_1 \times T_2] \times P = \begin{bmatrix}
\lambda(P,sx_1,rx_1)+tx_1
\\
\lambda(P,ry_1,sy_1)+ty_1
\\
1
\end{bmatrix}
$$

where:

$$
\begin{array}{rl}
\lambda(P,a,b) = & a(P_xsx_2+P_yrx_2+tx_2)+
\\
& b(P_xry_2+P_ysy_2+ty_2)
\end{array}
$$

### Expansion

The above can be expanded:

$$
\begin{array}{rl}
P'_x & = sx_1(P_xsx_2+P_yrx_2+tx_2)
\\
& +rx_1(P_xry_2+P_ysy_2+ty_2)
\\
& +tx_1
\\
\ 
\\
P'_y & = ry_1(P_xsx_2+P_yrx_2+tx_2)
\\
& + sy_1(P_xry_2+P_ysy_2+ty_2)
\\
& +ty_1
\end{array}
$$
