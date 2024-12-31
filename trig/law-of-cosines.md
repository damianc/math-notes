# Law of Cosines

![Triangle and Law of Cosines](https://raw.githubusercontent.com/damianc/math-notes/refs/heads/master/_images/trigonometry/law-of-cosines.png)

$$
\begin{array}{l}
a^2 = b^2 + c^2 - 2bc \cos(\alpha)
\\
b^2 = a^2 + c^2 - 2ac \cos(\beta)
\\
c^2 = a^2 + b^2 - 2ab \cos(\gamma)
\end{array}
$$

## Reading Angles

$$
\begin{array}{rcl}
\cos(\alpha) & = & \frac{b^2+c^2-a^2}{2bc}
\\
\alpha &=& \arccos\left( \frac{b^2+c^2-a^2}{2bc} \right)
\\
\ 
\\
\cos(\beta) & = & \frac{a^2+c^2-b^2}{2ac}
\\
\beta &=& \arccos\left( \frac{a^2+c^2-b^2}{2ac} \right)
\\
\ 
\\
\cos(\gamma) & = & \frac{a^2+b^2-c^2}{2ab}
\\
\gamma &=& \arccos\left( \frac{a^2+b^2-c^2}{2ab} \right)
\end{array}
$$

## Implications

- if:

$$
a^2 = b^2 + c^2 - 2bc \cos(\alpha)
$$

- then:

$$
\alpha = \arccos\left(
 \frac{c^2 + b^2 - a^2}{2bc}
\right)
$$

$$
b = \frac{a}{\sin(\alpha)} \sin\left(
 \pi - \left(
  \alpha + \arcsin\left(
   \frac{c}{a} \sin(\alpha)
  \right)
 \right)
\right)
$$

$$
c = \frac{a}{\sin(\alpha)} \sin\left(
 \pi - \left(
  \alpha + \arcsin\left(
   \frac{b}{a} \sin(\alpha)
  \right)
 \right)
\right)
$$
