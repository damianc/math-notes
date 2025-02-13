# Curl

The curl measures the tendency to rotate about a point in a _vector field_ in $\Bbb{R}^3$.

For a vector field $\vec{F}$:

$$
\vec{F} = P\hat{i} + Q\hat{j} + R\hat{k} = (P,Q,R)
$$

The curl is:

$$
\text{curl} \ \vec{F} = \nabla \times \vec{F} = \begin{vmatrix}
  \hat{i} & \hat{j} & \hat{k}
  \\
  \ 
  \\
  \frac{\partial}{\partial x} & \frac{\partial}{\partial y} & \frac{\partial}{\partial z}
  \\
  \ 
  \\
  P & Q & R
\end{vmatrix} = \begin{bmatrix}
  \frac{\partial R}{\partial y} - \frac{\partial Q}{\partial z}
  \\
  \ 
  \\
  \frac{\partial R}{\partial x} - \frac{\partial P}{\partial z}
  \\
  \ 
  \\
  \frac{\partial Q}{\partial x} - \frac{\partial P}{\partial y}
\end{bmatrix}^{\intercal}
$$

## Examples

### Example 1

The vector field:

$$
\vec{F}(x,y,z) = x\hat{j} - y \hat{i} = -y \hat{i} + x \hat{j} = (-y,x,0)
$$

The curl:

$$
\text{curl} \ \vec{F} = \nabla \times \vec{F} = \begin{vmatrix}
  \hat{i} & \hat{j} & \hat{k}
  \\
  \ 
  \\
  \frac{\partial}{\partial x} & \frac{\partial}{\partial y} & \frac{\partial}{\partial z}
  \\
  \ 
  \\
  -y & x & 0
\end{vmatrix} = M_{11}\hat{i} - M_{12}\hat{j} + M_{13}\hat{k}
$$

$$
\because \left[\begin{array}{l}
M_{11} = \frac{\partial}{\partial y}(0) - \frac{\partial}{\partial z}(x) = 0 - x \frac{\partial}{\partial z}(1) = 0-0 = 0
\\
\ 
\\
M_{12} = \frac{\partial}{\partial x}(0) - \frac{\partial}{\partial z}(-y) = 0 - (-y \frac{\partial}{\partial z}(1)) = 0-0 = 0
\\
\ 
\\
M_{13} = \frac{\partial}{\partial x}(x) - \frac{\partial}{\partial y}(-y) = 1 + \frac{\partial}{\partial y}(y) = 1+1 = 2
\end{array}\right.
$$

$$
\begin{array}{rl}
\text{curl} \ \vec{F} = \nabla \times \vec{F} & = M_{11}\hat{i} - M_{12}\hat{j} + M_{13}\hat{k}
\\
& = 0 \hat{i} - 0 \hat{j} + 2 \hat{k}
\\
& = (0,0,2)
\end{array}
$$

### Example 2

The vector field:

$$
\vec{F}(x,y,z) = xz \hat{i} + xyz \hat{j} - y^2 \hat{k} = (xz,xyz,-y^2)
$$

The curl:

$$
\text{curl} \ \vec{F} = \nabla \times \vec{F} = \begin{vmatrix}
  \hat{i} & \hat{j} & \hat{k}
  \\
  \ 
  \\
  \frac{\partial}{\partial x} & \frac{\partial}{\partial y} & \frac{\partial}{\partial z}
  \\
  \ 
  \\
  xz & xyz & -y^2
\end{vmatrix} = M_{11}\hat{i} - M_{12}\hat{j} + M_{13}\hat{k}
$$

$$
\because \left[\begin{array}{l}
M_{11} = \frac{\partial}{\partial y}(-y^2) - \frac{\partial}{\partial z}(xyz) = -\frac{\partial}{\partial y}(y^2) - xy \frac{\partial}{\partial z}(z) = -2y - xy = -y(2+x)
\\
\ 
\\
M_{12} = \frac{\partial}{\partial x}(-y^2) - \frac{\partial}{\partial z}(xz) = -y^2 \frac{\partial}{\partial x}(1) - x \frac{\partial}{\partial z}(z) = 0-x = -x
\\
\ 
\\
M_{13} = \frac{\partial}{\partial x}(xyz) - \frac{\partial}{\partial y}(xz) = yz \frac{\partial}{\partial x}(x) - xz \frac{\partial}{\partial y}(1) = yz-0 = yz
\end{array}\right.
$$

$$
\begin{array}{rl}
\text{curl} \ \vec{F} = \nabla \times \vec{F} & = M_{11}\hat{i} - M_{12}\hat{j} + M_{13}\hat{k}
\\
& = -y(2+x) \hat{i} + x \hat{j} + yz \hat{k}
\\
& = (-y(2+x),x,yz)
\end{array}
$$
