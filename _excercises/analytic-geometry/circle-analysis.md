# Exercise: Circle Analysis

The line described with the equation $\color{blue}{(1)}$ intersects the circle described with the equation $\color{blue}{(2)}$.

$$
\begin{array}{ll}
\color{blue}{(1)} & y = f(x) = x-2
\\
\color{blue}{(2)} & (x-4)^2 + y^2 = 4
\end{array}
$$

1. Find points $P$ and $Q$ at which the line intersects the circle
2. Determine length of the chord $|PQ|$
3. Determine length of the shorter arc $\overset{\frown}{PQ}$
4. Determine the measure of the inscribed angle subtended by:  
  4.1. the shorter arc $\overset{\frown}{PQ}$  
  4.2. the longer arc $\overset{\frown}{PQ}$
5. Calculate the area of:  
  5.1. the sector of the circle based on the shorter arc $\overset{\frown}{PQ}$  
  5.2. the segment of the circle based on the chord $|PQ|$

## Solution

### Exercise 1

In the circle equation replace $y$ with the function $f(x) = x-2$:

$$
\begin{array}{l}
(x-4)^2 + \boldsymbol{y}^2 = 4
\\
(x-4)^2 + (\boldsymbol{x-2})^2 = 4
\end{array}
$$

Obtain a square function:

$$
\begin{array}{l}
(x-4)^2 + (x-2)^2 = 4
\\
(x-4)^2 + (x-2)^2 - 4 = 0
\\
x^2 + 16 - 8x + x^2 + 4 - 4x - 4 = 0
\\
2x^2 - 12x + 16 = 0
\end{array}
$$

Determine the roots of this function:

$$
\begin{array}{l}
A = 2
\\
B = -12
\\
C = 16
\\
\ 
\\
\Delta = B^2-4AC = 144-128 = 16
\\
\ 
\\
x_1 = \frac{-B+\sqrt{\Delta}}{2A} = \frac{12+4}{4} = 4
\\
x_2 = \frac{-B-\sqrt{\Delta}}{2A} = \frac{12-4}{4} = 2
\end{array}
$$

Pass the roots $x_1$ and $x_2$ to the $f(x)$ function to get coordinates of the intersection points:

$$
\begin{array}{l}
x_1 = 4
\\
y_1 = f(x_1) = 4-2 = 2
\\
\boldsymbol{P} = (x_1,y_1) = \boldsymbol{(4,2)}
\\
\ 
\\
x_2 = 2
\\
y_2 = f(x_2) = 2-2 = 0
\\
\boldsymbol{Q} = (x_2,y_2) = \boldsymbol{(2,0)}
\end{array}
$$

### Exercise 2

$$
\begin{array}{ll}
\boldsymbol{|PQ|} & = \sqrt{(x_P-x_Q)^2 + (y_P-y_Q)^2}
\\
& = \sqrt{2^2 + 2^2}
\\
& = \boldsymbol{\sqrt{8}}
\end{array}
$$

### Exercise 3

To get the length of an arc we use formula:

$$
\overset{\frown}{a} = \alpha r
$$

Where $\alpha$ is the central angle, yet we don't know its measure. Fortunately, we can get it from the formula for the length of a chord:

$$
c = 2r \sin\left(\frac{\alpha}{2}\right)
$$

It can be transformed to obtain formula for $\alpha$:

$$
\alpha = 2 \arcsin\left(\frac{c}{2r}\right)
$$

As radius $r$ equals $2$ and the chord length $c$ equals $\sqrt{8}$:

$$
\begin{array}{ll}
\alpha & = 2 \arcsin\left(\frac{\sqrt{8}}{4}\right)
\\
& = 2 \arcsin\left(\frac{1}{\sqrt{2}}\right)
\\
& = 2 \cdot 45\degree
\\
& = 90\degree
\\
& = \frac{1}{2} \pi \quad \text{\tiny radians}
\end{array}
$$

Finally:

$$
\boldsymbol{\overset{\frown}{a}} = \alpha r = \frac{1}{2} \pi \cdot 2 = \boldsymbol{\pi}
$$

### Exercise 4

The inscribed angle is half the central angle subtended by the same arc.

- for the shorter arc:

$$
\begin{array}{l}
\alpha = 90\degree
\\
\boldsymbol{\theta_{\alpha}} = \frac{1}{2} \alpha = \boldsymbol{45\degree}
\end{array}
$$

- for the longer arc:

$$
\begin{array}{l}
\alpha' = 360\degree - \alpha = 360\degree - 90\degree = 270\degree
\\
\boldsymbol{\theta_{\alpha'}} = \frac{1}{2} \alpha' = \boldsymbol{135\degree}
\end{array}
$$

### Exercise 5

- area of a sector can be obtained from the formula $\frac{1}{2} \alpha r^2$:

$$
\boldsymbol{A_{\text{sector}}} = \frac{1}{2} \cdot \frac{1}{2} \pi \cdot 4 = \boldsymbol{\pi}
$$

- area of a segment can be obtained from the formula $\frac{1}{2} r^2 (\alpha - \sin \alpha)$:

$$
\boldsymbol{A_{\text{segment}}} = \frac{1}{2} \cdot 4 \left(\frac{1}{2} \pi - 1\right) = \boldsymbol{\pi-2} \approx 1.1416
$$

### Resume

1. $(4,2)$ and $(2,0)$
2. $\sqrt{8}$
3. $\pi$
4. $45\degree$ and $135\degree$
5. $\pi$ and $\pi-2$ ($\approx 1.1416$)
