# Getting Function from Gradient

A vector-field poses the [gradient](https://github.com/damianc/math-notes/blob/master/vectors/vc/function-gradient.md) of some function if the [Jacobian matrix](https://github.com/damianc/math-notes/blob/master/differentiation/partial/jacobian-matrix.md) is a symmetric matrix.

## Function of Two Variables

For the vector-field $\vec{F}(x,y) = (P,Q)$ we can obtain the function $f(x,y)$ whose gradient is $\vec{F}(x,y)$ if:

$$
\frac{\partial P}{\partial y} = \frac{\partial Q}{\partial x}
$$

If the condition above is fulfilled, then the vector-field:

$$
\vec{F}(x,y) = (P,Q)
$$

is the gradient of the function:

$$
f(x,y) = p(x,y) + q(y) + C
$$

where:

$$
\begin{array}{l}
p(x,y) = \int P \ dx
\\
\ 
\\
q(y) = \int \lambda_q(y) \ dy
\\
\quad \lambda_q(y) = Q - \frac{\partial p}{\partial y}
\end{array}
$$

### Examples

#### Example 1

If the vector-field $\vec{F}$ is defined as follows:

$$
\vec{F}(x,y) = (P,Q) = (2x,2y)
$$

Then:

$$
\begin{array}{l}
\boldsymbol{p(x,y)} = \int P \ dx = \int 2x \ dx = \boldsymbol{x^2}
\\
\ 
\\
\lambda_q(y) = Q - \frac{\partial p}{\partial y} = 2y - \frac{\partial}{\partial y} x^2 = 2y-0 = 2y
\\
\boldsymbol{q(y)} = \int \lambda_q(y) \ dy = \int 2y \ dy = \boldsymbol{y^2}
\end{array}
$$

Finally:

$$
\begin{array}{ll}
f(x,y) & = p(x,y)+q(y)
\\
& = x^2 + y^2
\end{array}
$$

#### Example 2

If the vector-field $\vec{F}$ is defined as follows:

$$
\vec{F}(x,y) = (P,Q) = (y^2,2xy)
$$

Then:

$$
\begin{array}{l}
\boldsymbol{p(x,y)} = \int P \ dx = \int y^2 \ dx = \boldsymbol{xy^2}
\\
\ 
\\
\lambda_q(y) = Q - \frac{\partial p}{\partial y} = 2xy - \frac{\partial}{\partial y} xy^2 = 2xy - 2xy = 0
\\
\boldsymbol{q(y)} = \int \lambda_q(y) \ dy = \int 0 \ dy = \boldsymbol{0}
\end{array}
$$

Finally:

$$
\begin{array}{ll}
f(x,y) & = p(x,y)+q(y)
\\
& = xy^2 + 0 = xy^2
\end{array}
$$

## Function of Three Variables

For the vector-field $\vec{F}(v_1,v_2,v_3) = (F_1,F_2,F_3)$ we can obtain the function $f(v_1,v_2,v_3)$ whose gradient is $\vec{F}$ if the **Jacobian matrix** of $\vec{F}$ is a symmetric matrix, i.e.:

$$
\underset{\substack{
1 \leqslant i \lt 3
\\
i \lt j \leqslant 3
}}{\Large\forall}
\quad \frac{\partial F_i}{\partial v_j} = \frac{\partial F_j}{\partial v_i}
$$

> alternatively, we can check if the vector-field does not have the [rotation](https://github.com/damianc/math-notes/blob/master/vectors/vc/curl.md), i.e., if $\nabla \times \vec{F} = \vec{0}$

with the condition fulfilled, the vector-field:

$$
\vec{F}(x,y,z) = (P,Q,R)
$$

is the gradient of the function:

$$
f(x,y,z) = p(x,y,z) + q(y,z) + r(z) + C
$$

where:

$$
\begin{array}{l}
p(x,y,z) = \int P \ dx
\\
\ 
\\
q(y,z) = \int \lambda_q(y,z) \ dy
\\
\quad \lambda_q(y,z) = Q - \frac{\partial p}{\partial y}
\\
\ 
\\
r(z) = \int \lambda_r(z) \ dz
\\
\quad \lambda_r(z) = R - \frac{\partial}{\partial z} (p+q)
\end{array}
$$

### Example

If the vector-field $\vec{F}$ is defined as follows:

$$
\begin{array}{rl}
\vec{F}(x,y,z) & = (P,Q,R)
\\
& = (\sin(y),z^2-x \cos(y),2yz+1)
\end{array}
$$

Then:

$$
\begin{array}{rl}
\boldsymbol{p(x,y,z)} & = \int P \ dx
\\
& = \int \sin(y) \ dx
\\
& = \boldsymbol{x \sin(y)}
\\
\ 
\\
\lambda_q(y,z) & = Q - \frac{\partial p}{\partial y}
\\
& = (z^2-x \cos(y)) - \frac{\partial}{\partial y} x \sin(y)
\\
& = (z^2-x \cos(y))-(-x \cos(y))
\\
& = z^2
\\
\boldsymbol{q(y,z)} & = \int \lambda_q(y,z) \ dy
\\
& = \int z^2 \ dy
\\
& = \boldsymbol{yz^2}
\\
\ 
\\
\lambda_r(z) & = R - \frac{\partial}{\partial z} (p+q)
\\
& = (2yz+1) - \frac{\partial}{\partial z} (x \sin(y)+yz^2)
\\
& = (2yz+1) - (0+2yz)
\\
& = 1
\\
\boldsymbol{r(z)} & = \int \lambda_r(z) \ dz
\\
& = \int 1 \ dz
\\
& = \boldsymbol{z}
\end{array}
$$

Finally:

$$
\begin{array}{rl}
f(x,y,z) & = p(x,y,z) + q(y,z) + r(z)
\\
& = x \sin(y) + yz^2 + z
\\
& = x \sin(y) + z(yz+1)
\end{array}
$$

## Generalization

If a vector-field has the symmetric Jacobian (or  has no rotation, i.e., $\text{curl } \vec{F} = \vec{0}$), there is the function $f$ whose gradient is the given vector-field $\vec{F}$.

If the condition above is fulfilled, then the vector-field:

$$
\vec{F}(V_n) = (F_1,F_2,\dots,F_n)
$$

is the gradient of the function:

$$
f(V_n) = \left[ \sum_{i=1}^n f_i(V_i) \right] + C
$$

where:

$$
\begin{array}{l}
V_i = [v_i, v_{i+1}, \dots, v_n]
\\
\ 
\\
f_1(V_1) = \int F_1(V_1) \ dv_1
\\
\ 
\\
f_i(V_i) = \int \lambda_{f_i}(V_i) \ dv_i
\\
\lambda_{f_i}(V_i) = F_i - \frac{\partial}{\partial v_i} \left[
\sum_{j=1}^{i-1} f_j(V_j)
\right]
\end{array}
$$

### Example

If the vector-field $\vec{F}$ is defined as follows:

$$
\begin{array}{rl}
\vec{F}(x,y,z,w) & = (P,Q,R,S)
\\
& = (2x+w,z,y,x+2)
\end{array}
$$

Then:

$$
\begin{array}{rl}
\boldsymbol{p(x,y,z,w)} & = \int P \ dx
\\
& = \int (2x+w) \ dx
\\
& = \boldsymbol{x^2+xw}
\\
\ 
\\
\lambda_q(y,z,w) & = Q-\frac{\partial p}{\partial y}
\\
& = z-\frac{\partial}{\partial y} (x^2+xw)
\\
& = z-0
\\
& = z
\\
\boldsymbol{q(y,z,w)} & = \int \lambda_q(y,z,w) \ dy
\\
& = \int z \ dy
\\
& = \boldsymbol{yz}
\\
\ 
\\
\lambda_r(z,w) & = R-\frac{\partial}{\partial z} (p+q)
\\
& = y - \frac{\partial}{\partial z} (x^2+xw+yz)
\\
& = y-y
\\
& = 0
\\
\boldsymbol{r(z,w)} & = \int \lambda_r(z,w) \ dz
\\
& = \int 0 \ dz
\\
& = \boldsymbol{0}
\\
\ 
\\
\lambda_s(w) & = S-\frac{\partial}{\partial w} (p+q+r)
\\
& = x+2 - \frac{\partial}{\partial w} (x^2+xw+yz+0)
\\
& = x+2-x
\\
& = 2
\\
\boldsymbol{s(w)} & = \int \lambda_s(w) \ dw
\\
& = \int 2 \ dw
\\
& = \boldsymbol{2w}
\end{array}
$$

Finally:

$$
\begin{array}{rl}
f(x,y,z,w) & = p(x,y,z,w) + q(y,z,w) + r(z,w) + s(w)
\\
& = (x^2+xw)+(yz)+(0)+(2w)
\\
& = x^2+xw+yz+2w
\\
& = x^2+yz+w(x+2)
\end{array}
$$

### Academic Example

> In this example, let $[x,y,z,t,w,p] \equiv [v_1,v_2,v_3,v_4,v_5,v_6]$ and $V_n = [v_n, v_{n+1}, \dots, v_6]$.

If the vector-field $\vec{F}$ is defined as follows:

$$
\begin{array}{rl}
\vec{F}(V_1) & = (F_1,F_2,F_3,F_4,F_5,F_6)
\\
& = \left(x(2+3px),z,y,4t,-\frac{1}{2}, x^3\right)
\end{array}
$$

Then:

$$
\begin{array}{rl}
\boldsymbol{f_1(V_1)} & = \int F_1(V_1) \ dx
\\
& = \int x(2+3px) \ dx
\\
& = \int (2x+3px^2) \ dx
\\
& = \boldsymbol{x^2+px^3}
\\
\ 
\\
\lambda_{f_2}(V_2) & = F_2-\frac{\partial f_1}{\partial y}
\\
& = z-\frac{\partial}{\partial y} (x^2+px^3)
\\
& = z - 0
\\
& = z
\\
\boldsymbol{f_2(V_2)} & = \int \lambda_{f_2}(V_2) \ dy
\\
& = \int z \ dy
\\
& = \boldsymbol{yz}
\\
\ 
\\
\lambda_{f_3}(V_3) & = F_3-\frac{\partial}{\partial z} (f_1+f_2)
\\
& = y-\frac{\partial}{\partial z} (x^2+px^3+yz)
\\
& = y-y
\\
& = 0
\\
\boldsymbol{f_3(V_3)} & = \int \lambda_{f_3}(V_3) \ dz
\\
& = \int 0 \ dz
\\
& = \boldsymbol{0}
\\
\ 
\\
\lambda_{f_4}(V_4) & = F_4-\frac{\partial}{\partial t} \left( \displaystyle\sum_{1 \leqslant i \le 4} f_i \right)
\\
& = 4t-\frac{\partial}{\partial t} (x^2+px^3+yz+0)
\\
& = 4t-0
\\
& = 4t
\\
\boldsymbol{f_4(V_4)} & = \int \lambda_{f_4}(V_4) \ dt
\\
& = \int 4t \ dt
\\
& = \boldsymbol{2t^2}
\\
\ 
\\
\lambda_{f_5}(V_5) & = F_5-\frac{\partial}{\partial w} \left( \displaystyle\sum_{1 \leqslant i \le 5} f_i \right)
\\
& = -\frac{1}{2}-\frac{\partial}{\partial w} (x^2+px^3+yz+0+2t^2)
\\
& = -\frac{1}{2}-0
\\
& = -\frac{1}{2}
\\
\boldsymbol{f_5(V_5)} & = \int \lambda_{f_5}(V_5) \ dw
\\
& = \int -\frac{1}{2} \ dw
\\
& = \boldsymbol{-\frac{1}{2} w}
\\
\ 
\\
\lambda_{f_6}(V_6) & = F_6-\frac{\partial}{\partial p} \left( \displaystyle\sum_{1 \leqslant i \le 6} f_i \right)
\\
& = x^3-\frac{\partial}{\partial p} \left(x^2+px^3+yz+0+2t^2-\frac{1}{2} w\right)
\\
& = x^3-x^3
\\
& = 0
\\
\boldsymbol{f_6(V_6)} & = \int \lambda_{f_6}(V_6) \ dp
\\
& = \int 0 \ dp
\\
& = \boldsymbol{0}
\end{array}
$$

Finally:

$$
\begin{array}{rl}
f(x,y,z,t,w,p) & = \displaystyle\sum_{1 \leqslant i \leqslant 6} f_i(V_i)
\\
& = x^2+px^3+yz+0+2t^2-\frac{1}{2} w+0
\\
& = x^2+px^3+yz+2t^2-\frac{1}{2} w
\\
& = x^2(1+px)+yz+2t^2-\frac{1}{2} w
\end{array}
$$
