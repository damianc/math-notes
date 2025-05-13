# Exercise: Equation of a Circle by Three Points On It

Points __A__, __B__ and __C__ lay on a circle. Find the equation of this circle.

$$
\begin{array}{l}
A = (6,0)
\\
B = (2.4,1.2)
\\
C = (4,-2)
\end{array}
$$

## Solution

The perpendicular bisectors of a triangle inscribed in a circle intersect at the center of the circle.

1. Find the center of this circle  
  1.1. Find equations of the lines $|AB|$ and $|AC|$  
  1.2. Find the midpoints $P$ and $Q$ of the segments $|AB|$ and $|AC|$, respectively  
  1.3. Find equations of the lines perpendicular to respective line ($|AB|$ and $|AC|$) and passing through respective midpoint ($P$ and $Q$)  
  1.4. Find the point of their intersection - that's the center $O$ of the circle
3. Determine the radius of this circle - the distance between the center and one of points ($A$, $B$ or $C$)
4. Put obtained values into the equation of the circle

### Step 1.1

$$
\begin{array}{ll}
f_{|AB|}(x) & = \begin{Bmatrix}
m = \frac{y_A-y_B}{x_A-x_B} = \frac{0-1.2}{6-2.4} = -\frac{1}{3}
\\
i = y_A-mx_A = \frac{6}{3} = 2
\end{Bmatrix}
\\
\ 
\\
& = mx+i = 2-\frac{1}{3}x
\end{array}
$$

$$
\begin{array}{ll}
f_{|AC|}(x) & = \begin{Bmatrix}
m = \frac{y_A-y_C}{x_A-x_C} = \frac{0+2}{6-4} = 1
\\
i = y_A-mx_A = -6
\end{Bmatrix}
\\
\ 
\\
& = mx+i = x-6
\end{array}
$$

### Step 1.2

$$
\begin{array}{ll}
P = \left(\frac{x_A+x_B}{2}, \frac{y_A+y_B}{2}\right) & = \left(\frac{6+2.4}{2}, \frac{0+1.2}{2}\right)
\\
\ 
\\
& = (4.2, 0.6)
\\
\ 
\\
Q = \left(\frac{x_A+x_C}{2}, \frac{y_A+y_C}{2}\right) & = \left(\frac{6+4}{2}, \frac{0-2}{2}\right)
\\
\ 
\\
& = (5, -1)
\end{array}
$$

### Step 1.3

$$
\begin{array}{ll}
f_{\perp |AB|}(x) & = \begin{Bmatrix}
m = \frac{-1}{m_{f_{|AB|}}} = \frac{-1}{-1:3} = 3
\\
i = y_P-mx_P = -12
\end{Bmatrix}
\\
\ 
\\
& = mx+i = 3x-12
\end{array}
$$

$$
\begin{array}{ll}
f_{\perp |AC|}(x) & = \begin{Bmatrix}
m = \frac{-1}{m_{f_{|AC|}}} = -\frac{1}{1} = -1
\\
i = y_Q-mx_Q = 4
\end{Bmatrix}
\\
\ 
\\
& = mx+i = 4-x
\end{array}
$$

### Step 1.4

$$
\begin{array}{l}
f_{\perp |AB|}(x) = f_{\perp |AC|}(x)
\\
3x-12 = 4-x
\\
3x+x = 4+12
\\
4x = 16
\\
x = 4
\\
\ 
\\
\boldsymbol{x_O} = \boldsymbol{4}
\\
\boldsymbol{y_O} = f_{\perp |AB|}(4) = 3 \cdot 4 - 12 = \boldsymbol{0}
\end{array}
$$

### Step 2

$$
\begin{array}{rl}
\boldsymbol{r} & = \sqrt{(x_O-x_A)^2 + (y_O-y_A)^2}
\\
\ 
\\
& = \sqrt{(4-6)^2 + (0-0)^2}
\\
\ 
\\
& = \sqrt{4} = \boldsymbol{2}
\end{array}
$$

### Step 3

$$
\begin{array}{l}
x_O = 4
\\
y_O = 0
\\
r = 2
\\
\ 
\\
(x-x_O)^2 + (y-y_O)^2 = r^2
\\
(x-4)^2 + (y-0)^2 = 2^2
\\
\ 
\\
\boldsymbol{(x-4)^2 + y^2 = 4}
\end{array}
$$
