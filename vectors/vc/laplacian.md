# Laplacian

Measures the difference between the value of _the scalar field_ with its average on infinitesimal balls.

For a function $f(x,y,z)$, the Laplacian is:

$$
\Delta f = \nabla^2 f = \frac{\partial^2 f}{\partial x^2} + \frac{\partial^2 f}{\partial y^2} + \frac{\partial^2 f}{\partial z^2}
$$

> in general, the Laplacian in $\Bbb{R}^n$ is:  
> $$\Delta f = \displaystyle\sum_{i=1}^n \frac{\partial^2 f}{\partial x_i^2}$$

## Examples

### Example 1

The function:

$$
f(x,y,z) = x^2 + y^2 + z^2
$$

The Laplacian:

$$
\Delta f = \frac{\partial^2 f}{\partial x^2} + \frac{\partial^2 f}{\partial y^2} + \frac{\partial^2 f}{\partial z^2}
$$

$$
\because \left[\begin{array}{rl}
\frac{\partial^2 f}{\partial x^2} = \frac{\partial^2}{\partial x^2} (x^2 + y^2 + z^2) & = \frac{\partial^2}{\partial x^2}(x^2) + \frac{\partial^2}{\partial x^2}(y^2) + \frac{\partial^2}{\partial x^2}(z^2)
\\
\ 
\\
& = \frac{\partial}{\partial x}(2x) + \frac{\partial}{\partial x}(0) + \frac{\partial}{\partial x}(0)
\\
\ 
\\
& = 2 + 0 + 0 = 2
\\
\ 
\\
\frac{\partial^2 f}{\partial y^2} = \frac{\partial^2}{\partial y^2} (x^2 + y^2 + z^2)  & = \cdots = \frac{\partial}{\partial y}(2y) = 2
\\
\ 
\\
\frac{\partial^2 f}{\partial z^2} = \frac{\partial^2}{\partial z^2} (x^2 + y^2 + z^2)  & = \cdots = \frac{\partial}{\partial z}(2z) = 2
\end{array}\right.
$$

$$
\Delta f = \frac{\partial^2 f}{\partial x^2} + \frac{\partial^2 f}{\partial y^2} + \frac{\partial^2 f}{\partial z^2} = 2+2+2 = 6
$$

### Example 2

The function:

$$
f(x,y) = \sin(x) \cos(y)
$$

The Laplacian:

$$
\Delta f = \frac{\partial^2 f}{\partial x^2} + \frac{\partial^2 f}{\partial y^2}
$$

$$
\because \left[\begin{array}{rl}
\frac{\partial^2 f}{\partial x^2} = \frac{\partial^2}{\partial x^2}(\sin(x) \cos(y)) & = \cos(y) \frac{\partial^2}{\partial x^2}(\sin(x))
\\
\ 
\\
& = \cos(y) \frac{\partial}{\partial x}(\cos(x))
\\
\ 
\\
& = \cos(y) \cdot (-\sin(x))
\\
\ 
\\
& = -\sin(x)\cos(y)
\\
\ 
\\
\frac{\partial^2 f}{\partial y^2} = \frac{\partial^2}{\partial y^2}(\sin(x) \cos(y)) & = \sin(x) \frac{\partial^2}{\partial y^2}(\cos(y))
\\
\ 
\\
& = \sin(x) \frac{\partial}{\partial y}(-\sin(y))
\\
\ 
\\
& = -\sin(x) \frac{\partial}{\partial y}(\sin(y))
\\
\ 
\\
& = -\sin(x) \cos(y)
\end{array}\right.
$$

$$
\begin{array}{rl}
\Delta f = \frac{\partial^2 f}{\partial x^2} + \frac{\partial^2 f}{\partial y^2} & = (-\sin(x) \cos(y))+(-\sin(x) \cos(y))
\\
& = -2 \sin(x) \cos(y)
\end{array}
$$
