# Jacobian Matrix

The **Jacobian matrix** is a matrix of first-order partial derivatives of _the vector field_ (a vector-valued function), i.e., $f: \Bbb{R}^m \to \Bbb{R}^n$.

> Both the Jacobian matrix and its determinant are referred to as "the Jacobian".

For _the vector field_ $f(x)$:

$$
f(x) = \begin{bmatrix}
f_1(x)
\\
f_2(x)
\\
\vdots
\\
f_n(x)
\end{bmatrix}, x = [x_1, x_2, \dots, x_m]
$$

The **Jacobian matrix** is as follows:

$$
{\boldsymbol J}_f = \begin{bmatrix}
\frac{\partial f_1}{\partial x_1} & \frac{\partial f_1}{\partial x_2} & \cdots & \frac{\partial f_1}{\partial x_m}
\\
\ 
\\
\frac{\partial f_2}{\partial x_1} & \frac{\partial f_2}{\partial x_2} & \cdots & \frac{\partial f_2}{\partial x_m}
\\
\vdots & \vdots & \ddots & \vdots
\\
\frac{\partial f_n}{\partial x_1} & \frac{\partial f_n}{\partial x_2} & \cdots & \frac{\partial f_n}{\partial x_m}
\end{bmatrix}
$$

Thereby the $(\boldsymbol{J}\_f)_{ij}$ element is as follows:

$$
(\boldsymbol{J}\_f)_{ij} = \frac{\partial f_i}{\partial x_j}
$$

## In Terms of the Gradient

The **Jacobian matrix** can be defined in terms of the [gradient](https://github.com/damianc/math-notes/blob/master/vectors/vc/function-gradient.md) as:

$$
{\boldsymbol J}_f = \begin{bmatrix}
\nabla f_1(x)^{\intercal}
\\
\nabla f_2(x)^{\intercal}
\\
\vdots
\\
\nabla f_n(x)^{\intercal}
\end{bmatrix}
$$

## Example

As an example, let's consider the transformation from _polar coordinates_ to _Cartesian coordinates_: $(r,\theta) \mapsto (x,y)$, which is given by the following function $f: \cal{P} \to \Bbb{R}^2$ ( where $\cal{P} := \Bbb{R}^{+} \times [0,2\pi)$ ):

$$
f\left(\begin{bmatrix}
r
\\
\theta
\end{bmatrix}\right) = \begin{bmatrix}
r \cos(\theta)
\\
r \sin(\theta)
\end{bmatrix}
$$

The **Jacobian matrix** is as follows:

$$
{\boldsymbol J}_f = \begin{bmatrix}
\frac{\partial}{\partial r}(r \cos \theta) & \frac{\partial}{\partial \theta}(r \cos \theta)
\\
\ 
\\
\frac{\partial}{\partial r}(r \sin \theta) & \frac{\partial}{\partial \theta}(r \sin \theta)
\end{bmatrix} = \begin{bmatrix}
\cos(\theta) & -r \sin(\theta)
\\
\ 
\\
\sin(\theta) & r \cos(\theta)
\end{bmatrix}
$$

Thus its determinant is:

$$
\begin{array}{rl}
| {\boldsymbol J}_f | & = \begin{vmatrix}
\cos(\theta) & -r \sin(\theta)
\\
\sin(\theta) & r \cos(\theta)
\end{vmatrix}
\\
\ 
\\
& = r \cos^2(\theta) + r \sin^2(\theta)
\\
& = r(\cos^2(\theta) + \sin^2(\theta))
\\
& \quad\quad {\small\color{gray} \because \sin^2(x) + \cos^2(x) = 1}
\\
& = r
\end{array}
$$
