# Hessian Matrix

> _Hessian matrix_ is also known as _Hessian_, or - less commonly - _Hesse matrix_

The Hessian matrix is a square matrix of second-order partial derivatives of the scalar field (a scalar-valued function), i.e., $f: \Bbb{R}^n \to \Bbb{R}$.

$$
H_f = \begin{bmatrix}
\frac{\partial^2f}{\partial x_1^2} & \frac{\partial^2f}{\partial x_1\partial x_2} & \cdots & \frac{\partial^2f}{\partial x_1 \partial x_n}
\\
\ 
\\
\frac{\partial^2f}{\partial x_2 \partial x_1} & \frac{\partial^2f}{\partial x_2^2} & \cdots & \frac{\partial^2f}{\partial x_2 \partial x_n}
\\
\ 
\\
\vdots & \vdots & \ddots & \vdots
\\
\ 
\\
\frac{\partial^2f}{\partial x_n \partial x_1} & \frac{\partial^2f}{\partial x_n \partial  x_2} & \cdots & \frac{\partial^2f}{\partial x_n^2}
\end{bmatrix}
$$

Thereby the $(H_f)_{ij}$ element is as follows:

$$
(H_f)_{ij} = \frac{\partial^2 f}{\partial x_i \partial x_j}
$$

> Second-order partial derivatives are evaluated in the following manner:
> 
> $\frac{\partial^2 f}{\partial x_1 \partial x_2} = \frac{\partial}{\partial x_2}\left( \frac{\partial f}{\partial x_1} \right)$
>
> If differentation takes place in respect to one variable:
> 
> $\frac{\partial^2 f}{\partial x_1^2} = \frac{\partial}{\partial x_1}\left( \frac{\partial f}{\partial x_1} \right)$

## Example

For the following function $f: \Bbb{R}^3 \to \Bbb{R}$:

$$
f(\begin{bmatrix}
t & u & v
\end{bmatrix}) = 2t^2 + tv + 3uv - u^2
$$

The Hessian matrix is as follows:

$$
H_f = \begin{bmatrix}
\frac{\partial^2f}{\partial t^2} & \frac{\partial^2f}{\partial t \partial u} & \frac{\partial^2f}{\partial t \partial v}
\\
\ 
\\
\frac{\partial^2f}{\partial u \partial t} & \frac{\partial^2f}{\partial u^2} & \frac{\partial^2f}{\partial u \partial v}
\\
\ 
\\
\frac{\partial^2f}{\partial v \partial t} & \frac{\partial^2f}{\partial v \partial u} & \frac{\partial^2f}{\partial v^2}
\end{bmatrix} = \begin{bmatrix}
4 & 0 & 1
\\
0 & -2 & 3
\\
1 & 3 & 0
\end{bmatrix}
$$
