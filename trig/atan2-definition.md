# Definition of _atan2_

$$
\text{atan2}(y,x) = \begin{cases}
\arctan\left(\frac{y}{x}\right) & \text{if } x \gt 0
\\
\arctan\left(\frac{y}{x}\right) + \pi & \text{if } x \lt 0 \text{ and } y \geq 0
\\
\arctan\left(\frac{y}{x}\right) - \pi & \text{if } x \lt 0 \text{ and } y \lt 0
\\
+\frac{\pi}{2} & \text{if } x=0 \text{ and } y \gt 0
\\
-\frac{\pi}{2} & \text{if } x=0 \text{ and } y \lt 0
\\
\text{undefined} & \text{if } x=0 \text{ and } y=0
\end{cases}
$$
