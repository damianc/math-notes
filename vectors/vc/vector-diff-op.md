# Vector Differential Operator ($\nabla$)

$$
\begin{array}{l|l}
\Bbb{R}^n & \nabla = \displaystyle\sum_{i=1}^n \hat{n}_i \frac{\partial}{\partial x_i} = \left(
\frac{\partial}{\partial x_1}, \cdots,
\frac{\partial}{\partial x_n}
\right)
\\
\ 
\\
\hline
\ 
\\
\Bbb{R}^3 & \nabla =
\hat{i} \frac{\partial}{\partial x} +
\hat{j} \frac{\partial}{\partial y} +
\hat{k} \frac{\partial}{\partial z} = \left(
\frac{\partial}{\partial x},
\frac{\partial}{\partial y},
\frac{\partial}{\partial z}
\right)
\end{array}
$$

## Use

| Operation | Notation | Description | Domain/Range |
|--|--|--|--|
| gradient | $\text{grad}(f) = \nabla f$ | Measures the rate and direction of change in _a scalar field_. | maps _scalar fields_ to _vector fields_ |
| divergence | $\text{div}(F) = \nabla \cdot F$ | Measures the scalar of a _source_ or _sink_ at a given point in _a vector field_. | maps _vector fields_ to _scalar fields_ |
| curl | $\text{curl}(F) = \nabla \times F$ | Measures the tendency to rotate about a point in _a vector field_ in $\Bbb{R}^3$. | maps _vector fields_ to _(pseudo)vector fields_ |
| Laplacian | $\Delta f = \nabla^2 = \nabla \cdot \nabla f$ | Measures the difference between the value of the scalar field with its average on infinitesimal balls. | maps between _scalar fields_ |
| vector Laplacian | $\nabla^2 F = \nabla(\nabla \cdot F) - \nabla \times (\nabla \times F)$ | Measures the difference between the value of the vector field with its average on infinitesimal balls. | maps between _vector fields_ |

### Gradient

For a function $f(x,y,z)$, the gradient is:

$$
\begin{array}{ll}
\text{grad} \ f = \nabla f{\color{#aaa} (x,y,z)} & = \frac{\partial}{\partial x} \hat{i} + \frac{\partial}{\partial y} \hat{j} + \frac{\partial}{\partial z} \hat{k}
\\
\ 
\\
& = \left[
\frac{\partial}{\partial x}, \frac{\partial}{\partial y}, \frac{\partial}{\partial z}
\right]^{\intercal}
\end{array}
$$

### Divergence

For a function $\vec{F} = P\hat{i} + Q\hat{j} + R\hat{k}$, the divergence is:

$$
\text{div} \ \vec{F} = \nabla \cdot \vec{F} = \frac{\partial P}{\partial x} + \frac{\partial Q}{\partial y} + \frac{\partial R}{\partial z}
$$

### Curl

For a function $\vec{F} = P\hat{i} + Q\hat{j} + R\hat{k}$, the curl is:

$$
\begin{array}{lcl}
\text{curl} \ \vec{F} = \nabla \times \vec{F} & = & \begin{vmatrix}
\hat{i} & \hat{j} & \hat{k}
\\
\ 
\\
\frac{\partial}{\partial x} & \frac{\partial}{\partial y} & \frac{\partial}{\partial z}
\\
\ 
\\
P & Q & R
\end{vmatrix}
\\
\ 
\\
& = & \left(
\frac{\partial R}{\partial y} - \frac{\partial Q}{\partial z}
\right) \hat{i} \ -
\\
\ 
\\
& & \left(
\frac{\partial P}{\partial z} - \frac{\partial R}{\partial x}
\right) \hat{j} \ +
\\
\ 
\\
& & \left(
\frac{\partial Q}{\partial x} - \frac{\partial P}{\partial y}
\right) \hat{k}
\\
\ 
\\
& = & \begin{bmatrix}
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
\end{array}
$$
