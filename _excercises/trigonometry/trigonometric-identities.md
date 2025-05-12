# Exercise: Trigonometric Identities

Find the value of $\alpha$:

$$
\frac{\sin(90\degree-\alpha)}{\cos(\alpha)} \cdot \frac{(\sin(\alpha)+\cos(\alpha))^2-1}{\sin(2\alpha)} + 2 \sin(\alpha) \sin(-\alpha) = \frac{1}{2}
$$

## Solution

1. Let $A = \frac{\sin(90\degree-\alpha)}{\cos(\alpha)}$ and handle it
2. Let $B = \frac{(\sin(\alpha)+\cos(\alpha))^2-1}{\sin(2\alpha)}$ and handle it
3. Let $C = 2 \sin(\alpha) \sin(-\alpha)$ and handle it
4. Handle $AB+C = \frac{1}{2}$ to obtain $\alpha$

### Step 1

$$
\begin{array}{ll}
A = \frac{\sin(90\degree-\alpha)}{\cos(\alpha)}
\\
& \color{gray}{\small \because \ \sin(90\degree-\alpha) = \cos(\alpha)}
\\
\boldsymbol{A} = \frac{\cos(\alpha)}{\cos(\alpha)} = \boldsymbol{1}
\end{array}
$$

### Step 2

$$
\begin{array}{ll}
B = \frac{(\sin(\alpha)+\cos(\alpha))^2-1}{\sin(2\alpha)}
\\
& \color{gray}{\small \because \ (a+b)^2 = a^2 + b^2 + 2ab}
\\
B = \frac{\sin^2(\alpha)+\cos^2(\alpha)+2\sin(\alpha)\cos(\alpha)-1}{\sin(2\alpha)}
\\
& \color{gray}{\small \because \ \sin^2(\alpha)+\cos^2(\alpha) = 1}
\\
B = \frac{1+2\sin(\alpha)\cos(\alpha)-1}{\sin(2\alpha)}
\\
\ 
\\
B = \frac{2\sin(\alpha)\cos(\alpha)}{\sin(2\alpha)}
\\
& \color{gray}{\small \because \ 2 \sin(\alpha) \cos(\alpha) = \sin(2\alpha)}
\\
\boldsymbol{B} = \frac{\sin(2\alpha)}{\sin(2\alpha)} = \boldsymbol{1}
\end{array}
$$

### Step 3

$$
\begin{array}{ll}
C = 2 \sin(\alpha) \sin(-\alpha)
\\
& \color{gray}{\small \because \ \sin(-\alpha) = -\sin(\alpha)}
\\
C = -2 \sin(\alpha) \sin(\alpha)
\\
\boldsymbol{C} = \boldsymbol{-2 \sin^2(\alpha)}
\end{array}
$$

### Step 4

$$
\begin{array}{ll}
AB+C = \frac{1}{2}
\\
1 \cdot 1 + (-2 \sin^2(\alpha)) = \frac{1}{2}
\\
1 - 2 \sin^2(\alpha) = \frac{1}{2}
\\
& \color{gray}{\small \because \ a-b=c \implies a-c=b}
\\
1-\frac{1}{2} = 2 \sin^2(\alpha)
\\
\frac{1}{2} = 2 \sin^2(\alpha)
\\
& \color{gray}{\small | \ :2}
\\
\frac{1}{4} = \sin^2(\alpha)
\\
& \color{gray}{\small | \ \sqrt{\ \ }}
\\
\frac{1}{2} = \sin(\alpha)
\\
& \color{gray}{\small \because \ a=b \implies b=a}
\\
\sin(\alpha) = \frac{1}{2}
\\
& \color{gray}{\small | \ \arcsin()}
\\
\alpha = \arcsin\left(\frac{1}{2}\right)
\\
\boldsymbol{\alpha} = \boldsymbol{30\degree}
\end{array}
$$
