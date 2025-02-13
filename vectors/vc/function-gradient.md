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

## Example of the Gradient

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

## Examples

### Example 1

The function:

$$
f(x,y) = x^2 + y^2
$$

The gradient:

$$
\because \left[\begin{array}{l}
\frac{\partial}{\partial x}(x^2+y^2) = \frac{\partial}{\partial x}(x^2) + \frac{\partial}{\partial x}(y^2) = 2x+0 = 2x
\\
\ 
\\
\frac{\partial}{\partial y}(x^2+y^2) = \frac{\partial}{\partial y}(x^2) + \frac{\partial}{\partial y}(y^2) = 0+2y = 2y
\end{array}\right.
$$

$$
\nabla f = \left(
  \frac{\partial f}{\partial x}, \frac{\partial f}{\partial y}
\right) = (2x, 2y)
$$

### Example 2

The function:

$$
f(x,y) = x^2
$$

The gradient:

$$
\because \left[\begin{array}{l}
\frac{\partial}{\partial x}(x^2) = 2x
\\
\ 
\\
\frac{\partial}{\partial y}(x^2) = 0
\end{array}\right.
$$

$$
\nabla f = \left(
  \frac{\partial f}{\partial x}, \frac{\partial f}{\partial y}
\right) = (2x, 0)
$$

### Example 3

The function:

$$
f(x,y) = y^2 \ \sin(x)
$$

The gradient:

$$
\because \left[\begin{array}{l}
\frac{\partial}{\partial x}(y^2 \ \sin(x)) = y^2 \frac{\partial}{\partial x}(\sin(x)) = y^2 \ \cos(x)
\\
\ 
\\
\frac{\partial}{\partial y}(y^2 \ \sin(x)) = \sin(x) \frac{\partial}{\partial y}(y^2) = 2y \ \sin(x)
\end{array}\right.
$$

$$
\nabla f = \left(
  \frac{\partial f}{\partial x}, \frac{\partial f}{\partial y}
\right) = (y^2 \ \cos(x), 2y \ \sin(x))
$$

### Example 4

The function:

$$
f(x,y) = \sin(x) + y^2
$$

The gradient:

$$
\because \left[\begin{array}{l}
\frac{\partial}{\partial x}(\sin(x) + y^2) = \frac{\partial}{\partial x}(\sin(x)) + \frac{\partial}{\partial x}(y^2) = \cos(x) + 0 = \cos(x)
\\
\ 
\\
\frac{\partial}{\partial y}(\sin(x) + y^2) = \frac{\partial}{\partial y}(\sin(x)) + \frac{\partial}{\partial y}(y^2) = 0 + 2y = 2y
\end{array}\right.
$$

$$
\nabla f = \left(
  \frac{\partial f}{\partial x}, \frac{\partial f}{\partial y}
\right) = (\cos(x), 2y)
$$

### Example 5

The function:

$$
f(x,y,z) = \frac{xy^2}{z}
$$

The gradient:

$$
\because \left[\begin{array}{l}
\frac{\partial}{\partial x}\left(\frac{xy^2}{z}\right) = \frac{y^2}{z} \frac{\partial}{\partial x}(x) = \frac{y^2}{z}
\\
\ 
\\
\frac{\partial}{\partial y}\left(\frac{xy^2}{z}\right) = \frac{x}{z} \frac{\partial}{\partial y}(y^2) = \frac{x}{z} \cdot 2y = \frac{2xy}{z}
\\
\ 
\\
\frac{\partial}{\partial z}\left(\frac{xy^2}{z}\right) = xy^2 \frac{\partial}{\partial z}\left(\frac{1}{z}\right) = xy^2 \cdot -\frac{1}{z^2} = -\frac{xy^2}{z^2}
\end{array}\right.
$$

$$
\nabla f = \left(
  \frac{\partial f}{\partial x}, \frac{\partial f}{\partial y}, \frac{\partial f}{\partial z}
\right) = \left(
  \frac{y^2}{z}, \frac{2xy}{z}, -\frac{xy^2}{z^2}
\right)
$$

### Example 6

The function:

$$
f(x,y,z,w,v) = xyz + w^2v
$$

The gradient:

$$
\because \left[\begin{array}{ll}
\frac{\partial}{\partial x}(xyz+w^2v) & = \frac{\partial}{\partial x}(xyz) + \frac{\partial}{\partial x}(w^2v)
\\
& = yz \frac{\partial}{\partial x}(x) + w^2v \frac{\partial}{\partial x}(1)
\\
& = yz+0 = yz
\\
\ 
\\
\frac{\partial}{\partial y}(xyz+w^2v) & = \frac{\partial}{\partial y}(xyz) + \frac{\partial}{\partial y}(w^2v)
\\
& = xz \frac{\partial}{\partial y}(y) + w^2v \frac{\partial}{\partial y}(1)
\\
& = xz+0 = xz
\\
\ 
\\
\frac{\partial}{\partial z}(xyz+w^2v) & = \frac{\partial}{\partial z}(xyz) + \frac{\partial}{\partial z}(w^2v)
\\
& = xy \frac{\partial}{\partial z}(z) + w^2v \frac{\partial}{\partial z}(1)
\\
& = xy+0 = xy
\\
\ 
\\
\frac{\partial}{\partial w}(xyz+w^2v) & = \frac{\partial}{\partial w}(xyz) + \frac{\partial}{\partial w}(w^2v)
\\
& = xyz \frac{\partial}{\partial w}(1) + v \frac{\partial}{\partial w}(w^2)
\\
& = 0+2wv = 2wv
\\
\ 
\\
\frac{\partial}{\partial v}(xyz+w^2v) & = \frac{\partial}{\partial v}(xyz) + \frac{\partial}{\partial v}(w^2v)
\\
& = xyz \frac{\partial}{\partial v}(1) + w^2 \frac{\partial}{\partial v}(v)
\\
& = 0+w^2 = w^2
\end{array}\right.
$$

$$
\nabla f = \left(
  \frac{\partial f}{\partial x}, \frac{\partial f}{\partial y}, \frac{\partial f}{\partial z}, \frac{\partial f}{\partial w}, \frac{\partial f}{\partial v}
\right) = \left(
  yz, xz, xy, 2wv, w^2
\right)
$$
