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

what means that at point $(1,1)$ the function $f$ has fastest increase towards point $(2,2)$; its rate is:

$$
\vert \vert \nabla f \vert \vert = \sqrt{2^2 + 2^2} = \sqrt{8} = 2\sqrt{2}
$$

### Other Examples

- $f(x,y) = x^2$:

$$
\begin{array}{rl}
\nabla f(x,y) & = \left(
\frac{\partial f}{\partial x},
\frac{\partial f}{\partial y}
\right)
\\
\ 
\\
& = (2x,0)
\end{array}
$$

- $f(x,y) = y^2$:

$$
\begin{array}{rl}
\nabla f(x,y) & = \left(
\frac{\partial f}{\partial x},
\frac{\partial f}{\partial y}
\right)
\\
\ 
\\
& = (0,2y)
\end{array}
$$



- $f(x,y,z) = \frac{xy^2}{z}$:

$$
\begin{array}{rl}
\nabla f(x,y,z) & = \left(
\frac{\partial f}{\partial x},
\frac{\partial f}{\partial y},
\frac{\partial f}{\partial z}
\right)
\\
\ 
\\
& = \left(
\frac{y^2}{z},
\frac{2xy}{z},
-\frac{xy^2}{z^2}
\right)
\end{array}
$$

- $f(x,y,z,w,v) = xyz+w^2 v$:

$$
\begin{array}{rl}
\nabla f(x,y,z,w,v) & = \left(
\frac{\partial f}{\partial x},
\frac{\partial f}{\partial y},
\frac{\partial f}{\partial z},
\frac{\partial f}{\partial w},
\frac{\partial f}{\partial v}
\right)
\\
\ 
\\
& = (yz,xz,xy,2wv,w^2)
\end{array}
$$
