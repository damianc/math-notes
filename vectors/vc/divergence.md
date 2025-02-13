# Divergence

For a vector field $\vec{F}$:

$$
\vec{F} = P\hat{i} + Q\hat{j} + R\hat{k}
$$

The divergence is:

$$
\text{div} \ \vec{F} = \nabla \cdot \vec{F} = \frac{\partial P}{\partial x} + \frac{\partial Q}{\partial y} + \frac{\partial R}{\partial z}
$$

## Examples

### Example 1

The vector field:

$$
\vec{F}(x,y,z) = x^2 \hat{i} + y^2 \hat{j} + z^2 \hat{k} = (x^2, y^2, z^2)
$$

The divergence:

$$
\text{div} \ \vec{F} = \nabla \cdot \vec{F} = \frac{\partial \vec{F}_x}{\partial x} + \frac{\partial \vec{F}_y}{\partial y} + \frac{\partial \vec{F}_z}{\partial z}
$$

$$
\because \left[\begin{array}{l}
\frac{\partial \vec{F}_x}{\partial x} = \frac{\partial}{\partial x} (x^2) = 2x
\\
\ 
\\
\frac{\partial \vec{F}_y}{\partial y} = \frac{\partial}{\partial y} (y^2) = 2y
\\
\ 
\\
\frac{\partial \vec{F}_z}{\partial z} = \frac{\partial}{\partial z} (z^2) = 2z
\end{array}\right.
$$

$$
\text{div} \ \vec{F} = \nabla \cdot \vec{F} = 2x + 2y + 2z = 2(x+y+z)
$$

### Example 2

The vector field:

$$
\vec{F}(x,y,z) = xz \hat{i} + xyz \hat{j} - y^2 \hat{k} = (xz, xyz, -y^2)
$$

The divergence:

$$
\text{div} \ \vec{F} = \nabla \cdot \vec{F} = \frac{\partial \vec{F}_x}{\partial x} + \frac{\partial \vec{F}_y}{\partial y} + \frac{\partial \vec{F}_z}{\partial z}
$$

$$
\because \left[\begin{array}{l}
\frac{\partial \vec{F}_x}{\partial x} = \frac{\partial}{\partial x} (xz) = z \frac{\partial}{\partial x} (x) = z \cdot 1 = z
\\
\ 
\\
\frac{\partial \vec{F}_y}{\partial y} = \frac{\partial}{\partial y} (xyz) = xz \frac{\partial}{\partial y} (y) = xz \cdot 1 = xz
\\
\ 
\\
\frac{\partial \vec{F}_z}{\partial z} = \frac{\partial}{\partial z} (-y^2) = -y^2 \frac{\partial}{\partial z} (1) = -y^2 \cdot 0 = 0
\end{array}\right.
$$

$$
\text{div} \ \vec{F} = \nabla \cdot \vec{F} = z + xz = (1+x)z
$$
