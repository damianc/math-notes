# Vector/Matrix Functions Derivative

## Function Scalar-to-Vector

For a _parametric curve_/vector-valued function of one variable ${\boldsymbol{f}}: \Bbb{R} \rightarrow \Bbb{R}^m$:

$$
{\boldsymbol{f}}(x) = \begin{bmatrix}
f_1(x)
\\
\vdots
\\
f_m(x)
\end{bmatrix}
$$

Its derivative is a vector derivative as follows:

$$
\frac{\partial {\boldsymbol{f}}}{\partial x} = \begin{bmatrix}
\frac{\partial f_1}{\partial x}
\\
\vdots
\\
\frac{\partial f_m}{\partial x}
\end{bmatrix}
$$

## Function Scalar-to-Matrix

For a matrix-valued function of one variable ${\boldsymbol{F}}: \Bbb{R} \rightarrow \Bbb{R}^{m \times n}$:

$$
{\boldsymbol{F}}(x) = \begin{bmatrix}
f_{11}(x) & \cdots & f_{1n}(x)
\\
\vdots & \ddots & \vdots
\\
f_{m1}(x) & \cdots & f_{mn}(x)
\end{bmatrix}
$$

Its derivative is a matrix derivative as follows:

$$
\frac{\partial {\boldsymbol{F}}}{\partial x} = \begin{bmatrix}
\frac{\partial f_{11}}{\partial x} & \cdots & \frac{\partial f_{1n}}{\partial x}
\\
\vdots & \ddots & \vdots
\\
\frac{\partial f_{m1}}{\partial x} & \cdots & \frac{\partial f_{mn}}{\partial x}
\end{bmatrix}
$$

## Function Vector-to-Scalar

For a **scalar field**/scalar function of several variables $f: \Bbb{R}^m \rightarrow \Bbb{R}$:

$$
f({\boldsymbol{x}}),
\quad {\boldsymbol{x}} = \begin{bmatrix}
x_1
\\
\vdots
\\
x_m
\end{bmatrix}
$$

Its derivative is the **gradient** as follows:

$$
\frac{\partial f}{\partial {\boldsymbol{x}}} = \nabla f = \begin{bmatrix}
\frac{\partial f}{\partial x_1}
\\
\vdots
\\
\frac{\partial f}{\partial x_m}
\end{bmatrix}
$$

## Function Vector-to-Vector

For a **vector field**/vector function of several variables ${\boldsymbol{f}}: \Bbb{R}^m \rightarrow \Bbb{R}^n$:

$$
{\boldsymbol{f}}({\boldsymbol{x}}) = \begin{bmatrix}
f_1({\boldsymbol{x}})
\\
\vdots
\\
f_n({\boldsymbol{x}})
\end{bmatrix}, \quad {\boldsymbol{x}} = \begin{bmatrix}
x_1
\\
\vdots
\\
x_m
\end{bmatrix}
$$

Its derivative is the **Jacobian** as follows:

$$
\frac{\partial{\boldsymbol{f}}}{\partial{\boldsymbol{x}}} = {\boldsymbol{J}}_f = \begin{bmatrix}
\frac{\partial f_1}{\partial x_1} & \cdots & \frac{\partial f_1}{\partial x_m}
\\
\vdots & \ddots & \vdots
\\
\frac{\partial f_n}{\partial x_1} & \cdots & \frac{\partial f_n}{\partial x_m}
\end{bmatrix}
$$

or with **gradients**:

$$
\frac{\partial{\boldsymbol{f}}}{\partial{\boldsymbol{x}}} = \begin{bmatrix}
(\nabla f_1)^T
\\
\vdots
\\
(\nabla f_n)^T
\end{bmatrix}
$$

## Function Matrix-to-Scalar

For a _matrix functional_/matrix-to-scalar function $f: \Bbb{R}^{m \times n} \rightarrow \Bbb{R}$:

$$
f({\boldsymbol{X}}), \quad {\boldsymbol{X}} = \begin{bmatrix}
x_{11} & \cdots & x_{1n}
\\
\vdots & \ddots & \vdots
\\
x_{m1} & \cdots & x_{mn}
\end{bmatrix}
$$

Its derivative is a matrix gradient/derivative as follows:

$$
\frac{\partial f}{\partial {\boldsymbol{X}}} = \begin{bmatrix}
\frac{\partial f}{\partial x_{11}} & \cdots & \frac{\partial f}{\partial x_{1n}}
\\
\vdots & \ddots & \vdots
\\
\frac{\partial f}{\partial x_{m1}} & \cdots & \frac{\partial f}{\partial x_{mn}}
\end{bmatrix}
$$
