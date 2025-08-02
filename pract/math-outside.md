# Math Outside

## Approachable Objects

### with angle

![Distance to an approachable object with angle](https://github.com/damianc/math-notes/blob/master/_images/pract/env/env-01.png)

$$
\begin{array}{l}
h = d \cdot \tan(\alpha)
\\
d = \frac{h}{\tan(\alpha)}
\end{array}
$$

### without angle

![Distance to an approachable object without angle](https://github.com/damianc/math-notes/blob/master/_images/pract/env/env-02.png)

$$
\begin{array}{l}
h = \frac{d\mu}{t}
\\
d = \frac{ht}{\mu}
\end{array}
$$

## Distant Objects

### with tangent

![Distance to a distant object with tangent](https://github.com/damianc/math-notes/blob/master/_images/pract/env/env-03.png)

$$
d = s \cdot \tan(\alpha)
$$

### with Thales' theorem

![Distance to a distant object with Thales' theorem](https://github.com/damianc/math-notes/blob/master/_images/pract/env/env-04.png)

$$
d = \frac{ts_2}{s_1-s_2}
$$

### with 2 points

#### with angles

![Distance to a distant object with two angles](https://github.com/damianc/math-notes/blob/master/_images/pract/env/env-05.png)

$$
h = \frac{
 t \cdot \sin(\alpha) \cdot \sin(\beta)
}{
 \sin(\beta-\alpha)
}
$$

$$
\cup
$$

$$
h = \frac{
 t \cdot \tan(\alpha) \cdot \tan(\beta)
}{
 \tan(\beta) - \tan(\alpha)
}
$$

#### without angles

![Distance to a distant object with two points](https://github.com/damianc/math-notes/blob/master/_images/pract/env/env-06.png)

$$
h = \frac{\gamma ab}{b-a}
$$

$$
\iff
$$

$$
a = \frac{\mu_1}{t_1},
b = \frac{\mu_2}{t_2}
$$

or just:

$$
h = \frac{
 \gamma \mu_1 \mu_2
}{
 \mu_2 t_1 - \mu_1 t_2
}
$$

### with 4 angles

![Trapezoid with measured angles](https://github.com/damianc/math-notes/blob/master/_images/pract/env/env-07.png)

$$
X = \sqrt{
P^2 + Q^2 + 2PQ \cos(\theta_1 + \theta_2)
}
$$

$$
\iff
$$

$$
\begin{array}{l}
P = \frac{D \sin(\theta_2) \sin(\alpha-\theta_1)}{\sin(\theta_1+\theta_2) \sin(\alpha+\theta_2)}
\\
\ 
\\
Q = \frac{D \sin(\theta_1) \sin(\beta-\theta_2)}{\sin(\theta_1+\theta_2) \sin(\beta+\theta_1)}
\end{array}
$$

#### or with functions:

$$
\begin{array}{l}
P = k \ \lambda_{2,1}(\alpha)
\\
Q = k \ \lambda_{1,2}(\beta)
\end{array}
$$

$$
\iff
$$

$$
\begin{array}{l}
k = \frac{D}{\sin(\theta_1+\theta_2)}
\\
\ 
\\
\lambda_{i,j}(\varphi) = \sin(\theta_i) \cdot \frac{\sin(\varphi-\theta_j)}{\sin(\varphi+\theta_i)}
\\
{\color{gray} \tiny i,j \in \{{ 1,2 \}}, \ i \neq j}
\end{array}
$$

#### alternatively (with the same $k$):

$$
\begin{array}{l}
P = k \ \lambda(\alpha; \theta_2, \theta_1)
\\
Q = k \ \lambda(\beta; \theta_1, \theta_2)
\end{array}
$$

$$
\iff
$$

$$
\begin{array}{l}
\lambda(m; \varphi_1, \varphi_2) = \sin(\varphi_1) \cdot \frac{\sin(m-\varphi_2)}{\sin(m+\varphi_2)}
\\
{\color{gray} \tiny m,\varphi_1,\varphi_2 \in \left(0,\frac{1}{2}\pi\right), \min(m,\varphi_1,\varphi_2) \neq m}
\end{array}
$$
