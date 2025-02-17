# Vector Laplacian

Measures the difference between the value of _the vector field_ with its average on infinitesimal balls.

For a vector field $\vec{F}$:

$$
\vec{F} = P\hat{i} + Q\hat{j} + R\hat{k}
$$

The vector Laplacian is:

$$
\Delta F = \nabla^2 F = (\Delta F_1, \Delta F_2, \Delta F_3)
$$

It can be defined in terms of the $\nabla$ operator as:

$$
\begin{array}{rl}
\Delta F = \nabla^2 F & = \nabla(\nabla \cdot F) - \nabla \times (\nabla \times F)
\\
& = \text{grad}(\text{div} \ F) - \text{curl}(\text{curl} \ F)
\end{array}
$$

## Examples

### Example 1

The vector field:

$$
\vec{F}(x,y,z) = x^2\hat{i} + y^2\hat{j} + z^2\hat{k} = (x^2,y^2,z^2)
$$

The vector Laplacian:

$$
\Delta \vec{F} = (\Delta \vec{F}_x, \Delta \vec{F}_y, \Delta \vec{F}_z)
$$

$$
\because \left[\begin{array}{rl}
\Delta \vec{F}_x & = \frac{\partial^2(x^2)}{\partial x^2} + \frac{\partial^2(x^2)}{\partial y^2} + \frac{\partial^2(x^2)}{\partial z^2}
\\
\ 
\\
& = \frac{\partial(2x)}{\partial x} + \frac{\partial(2x)}{\partial y} + \frac{\partial(2x)}{\partial z} = 2+0+0 = 2
\\
\ 
\\
\Delta \vec{F}_y & = \frac{\partial^2(y^2)}{\partial x^2} + \frac{\partial^2(y^2)}{\partial y^2} + \frac{\partial^2(y^2)}{\partial z^2}
\\
\ 
\\
& = \frac{\partial(2y)}{\partial x} + \frac{\partial(2y)}{\partial y} + \frac{\partial(2y)}{\partial z} = 0+2+0 = 2
\\
\ 
\\
\Delta \vec{F}_z & = \frac{\partial^2(z^2)}{\partial x^2} + \frac{\partial^2(z^2)}{\partial y^2} + \frac{\partial^2(z^2)}{\partial z^2}
\\
\ 
\\
& = \frac{\partial(2z)}{\partial x} + \frac{\partial(2z)}{\partial y} + \frac{\partial(2z)}{\partial z} = 0+0+2 = 2
\end{array}\right.
$$

$$
\Delta \vec{F} = (\Delta \vec{F}_x, \Delta \vec{F}_y, \Delta \vec{F}_z) = (2,2,2)
$$

### Example 2

The vector field:

$$
\vec{F}(x,y) = \hat{i}\sin(x) + \hat{j} \cos(y) = (\sin(x), \cos(y))
$$

The vector Laplacian:

$$
\Delta \vec{F} = (\Delta \vec{F}_x, \Delta \vec{F}_y)
$$

$$
\because \left[\begin{array}{rl}
\Delta \vec{F}_x & = \frac{\partial^2}{\partial x^2}(\sin x) + \frac{\partial^2}{\partial y^2}(\sin x)
\\
\ 
\\
& = \frac{\partial}{\partial x}(\cos x) + \frac{\partial}{\partial y}(0)
\\
\ 
\\
& = -\sin(x) + 0 = -\sin(x)
\\
\ 
\\
\Delta \vec{F}_y & = \frac{\partial^2}{\partial x^2}(\cos y) + \frac{\partial^2}{\partial y^2}(\cos y)
\\
\ 
\\
& = \frac{\partial}{\partial x}(0) + \frac{\partial}{\partial y}(-\sin y)
\\
\ 
\\
& = 0 - \frac{\partial}{\partial y}(\sin y)
\\
\ 
\\
& = 0 - \cos(y) = -\cos(y)
\end{array}\right.
$$

$$
\Delta \vec{F} = (\Delta \vec{F}_x, \Delta \vec{F}_y) = (-\sin(x), -\cos(y))
$$
