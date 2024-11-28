# Multiple Integral over a Circle

> Example function: $(xy)^2$  
> Example circle: center at $(0,0)$ and radius $4$


$$
\int \int_C (xy)^2 \ dx \ dy
$$

$$
C = \\{
(x,y) \in \Bbb{R}^2 \ |\  x^2 + y^2 \leq 4^2
\\}
$$

1. Convert Cartesian to polar coordinates:

$$
\begin{cases}
x = r \cos(\theta)
\\
y = r \sin(\theta)
\end{cases}
$$

2. Replace Cartesian coordinates with polar ones and $dx \ dy$ with $r \ dr \ d\theta$:

$$
\int \int_C = (r \cos(\theta) \times r \sin(\theta))^2 \ r \ dr \ d\theta
$$

3. Simplify expression:

$$
\begin{array}{rl}
& (r \cos(\theta) \times r \sin(\theta))^2 \ r \ dr \ d\theta
\\
= & (r^2 \cos(\theta) \sin(\theta))^2 \ r \ dr \ d\theta
\\
& \quad\quad \because \sin(\theta) \cos(\theta) = \frac{1}{2} \sin(2\theta)
\\
= & \Bigl( \frac{r^4}{4} \sin^2(2\theta) \Bigr) r \ dr \ d\theta
\\
= & \frac{r^5}{4} \sin^2(2\theta) \ dr \ d\theta
\end{array}
$$

4. Define limits of integration:
- $r \in \langle 0,r \rangle$, here: $r \in \langle 0,4 \rangle$
- $\theta \in \langle 0,2\pi \rangle$

thus integral becomes:

$$
\int_0^{2\pi} \int_0^4 \frac{r^5}{4} \sin^2(2\theta) \ dr \ d\theta
$$

5. Do remaining math:

- integration with respect to $r$

$$
\begin{array}{rl}
\displaystyle
\int_0^4 \frac{1}{4} r^5 \sin^2(2\theta) \ dr & = \frac{1}{4} \sin^2(2\theta) \displaystyle \int_0^4 r^5 \ dr
\\
& = \frac{1}{4} \sin^2(2\theta) \Bigl[
\frac{r^6}{6}
\Bigr]_0^4
\\
& = \left( 170 + \frac{2}{3} \right) \sin^2(2\theta)
\end{array}
$$

- integration with respect to $\theta$

$$
\begin{array}{rl}
\displaystyle \int_0^{2\pi}
 \left( 170 + \frac{2}{3} \right) \sin^2(2\theta) \ d\theta & =  \left( 170 + \frac{2}{3} \right) \displaystyle \int_0^{2\pi} \sin^2(2\theta)
 \\
 & =  \left( 170 + \frac{2}{3} \right) \Bigl[
 -\frac{1}{8} (\sin(4\theta)-4\theta)
 \Bigr]_0^{2\pi}
 \\
 & =  \left( 170 + \frac{2}{3} \right) \pi
 \\
 & = \frac{512\pi}{3}
 \end{array}
$$

the result is:

$$
\large
\int \int_C (xy)^2 \ dx \ dy = \frac{512\pi}{3}
$$

## Another Example

> Example function: $xy$  
> Example circle: center at $(1,1)$ and radius $4$

$$
\int \int_C xy \ dx \ dy
$$

$$
C = \\{
(x,y) \in \Bbb{R}^2 \ |\  (x-1)^2 + (y-1)^2 \leq 4^2
\\}
$$

1. Convert Cartesian to polar coordinates:

$$
\begin{cases}
x = r \cos(\theta) + 1
\\
y = r \sin(\theta) + 1
\end{cases}
$$

2. Replace Cartesian coordinates with polar ones and $dx \ dy$ with $r \ dr \ d\theta$:

$$
\int \int_C = (r \cos(\theta) + 1)(r \sin(\theta) + 1) \ r \ dr \ d\theta
$$

3. Simplify expression:

$$
\begin{array}{rl}
& (r \cos(\theta) + 1)(r \sin(\theta) + 1)
\\
= & r \cos(\theta)(r \sin(\theta)+1) + (r \sin(\theta) + 1)
\\
= & r^2\cos(\theta)\sin(\theta) + r\cos(\theta) + r \sin(\theta) + 1
\\
= & \frac{1}{2} r^2 \sin(2\theta) + r(\cos(\theta)+\sin(\theta)) + 1
\end{array}
$$

thus integral becomes:

$$
\begin{array}{rl}
& {\displaystyle \int \int_C} \Bigl( \frac{1}{2} r^2 \sin(2\theta) + r(\cos(\theta)+\sin(\theta)) + 1 \Bigr) \ r \ dr \ d\theta
\\
= & {\displaystyle \int \int_C} \Bigl( \frac{1}{2} r^3 \sin(2\theta) + r^2(\cos(\theta)+\sin(\theta)) + r \Bigr) \ dr \ d\theta
\end{array}
$$

4. Define limits of integration:

- $r \in \langle 0,r \rangle$, here: $r \in \langle 0,4 \rangle$
- $\theta \in \langle 0,2\pi \rangle$

thus integral becomes:

$$
\int_0^{2\pi} \int_0^4 \Bigl( \frac{1}{2} r^3 \sin(2\theta) + r^2(\cos(\theta)+\sin(\theta)) + r \Bigr) \ dr \ d\theta
$$

5. Do remaining math:

5.1. Extract summands:

$$
\begin{array}{lr}
I_1 = \frac{1}{2} r^3 \sin(2\theta)
\\
I_2 = r^2(\cos(\theta)+\sin(\theta))
\\
I_3 = r
\end{array}
$$

5.2. Handle $I_1$ / $I_2$:

$$
\begin{array}{rl}
\because & \sin(2\theta)-\sin(0) = 0
\\
& \cos(2\theta)-\cos(0) = 0
\\
\ 
\\
\therefore & I_1 = 0
\\
& I_2 = 0
\end{array}
$$

5.3. Handle $I_3$:

- integration with respect to $r$

$$
I_3 = \int_0^4 r \ dr = \Bigl[ \frac{r^2}{2} \Bigr]_0^4 = 8
$$

- integration with respect to $\theta$

$$
\begin{array}{rl}
I_3 = \displaystyle \int_0^{2\pi} 8 \ d\theta & =
8 \displaystyle \int_0^{2\pi} 1 \ d\theta
\\
& = 8 \times \Bigl[ \theta \Bigr]_0^{2\pi}
\\
& = 8 \times 2\pi = 16\pi
\end{array}
$$

5.4. Sum up results:

$$
I_1 + I_2 + I_3 = 0 + 0 + 16\pi = 16\pi
$$

the result is:

$$
\large
\int \int_C xy \ dx \ dy = 16\pi
$$
