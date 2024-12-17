# Gradient of a Function

The gradient of a scalar-valued differentiable multivariate function $f$ is the _vector field_ (or _vector-valued function_) $\nabla f$ whose value at a point $p$ gives the direction and the rate of fastest increase.

$$
\begin{array}{rl}
\text{grad } f(x_1,x_2,\dots,x_n) & = \nabla f(x_1,x_2,\dots,x_n)
\\
& = \left(
\frac{\partial f}{\partial x_1},
\frac{\partial f}{\partial x_2},\dots,
\frac{\partial f}{\partial x_n}
\right)
\end{array}
$$

> _i-th_ term of a resultant vector is a derivative of $f$ with respect to _i-th_ variable

## Example

For an example function $f(x,y) = x^2 + y^2$, the gradient is:

$$
\nabla f(x,y) = \left(
\frac{\partial f}{\partial x},
\frac{\partial f}{\partial y}
\right) = (2x,2y)
$$

For example, at point $(1,1)$ the gradient is:

$$
\nabla f(1,1) = (2,2)
$$

what means that at point $(1,1)$ the function $f$ has fastest increase towards point $(2,2)$.
