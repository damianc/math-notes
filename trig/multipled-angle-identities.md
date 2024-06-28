# Multipled Angle Identities

## Double Angle Identities

### Sine

$$
\begin{array}{rl}
\sin(2\alpha) & = 2\sin(\alpha)\cos(\alpha)
\\
& = \frac{2 \tan\alpha}{1+\tan^2\alpha}
\\
& = 2\sqrt{1-\cos^2\alpha}\ \cos\alpha
\\
& = 2\sqrt{1-\sin^2\alpha}\ \sin\alpha
\\
& = (\sin(\alpha)+\cos(\alpha))^2-1
\end{array}
$$

### Cosine

$$
\begin{array}{rl}
\cos(2\alpha) & = \cos^2(\alpha)-\sin^2(\alpha)
\\
& = 2 \cos^2(\alpha)-1
\\
& = 1-2 \sin^2(\alpha)
\\
& = \frac{1-\tan^2\alpha}{1+\tan^2\alpha}
\end{array}
$$

### Tangent

$$
\begin{array}{rl}
\tan(2\alpha) & = \frac{2\tan\alpha}{1-\tan^2\alpha}
\\
& = \frac{2}{\cot(\alpha)-\tan(\alpha)}
\end{array}
$$

### Others

$$
\begin{array}{rl}
\csc(2\alpha) & = \frac{\sec(\alpha)\csc(\alpha)}{2}
\\
& = \color{blue}{\frac{1+\tan^2\alpha}{2\tan\alpha}}
\\
\\
\sec(2\alpha) & =
\frac{\sec^2\alpha}{2-\sec^2\alpha}
\\
& = \color{blue}{\frac{1+\tan^2\alpha}{1-\tan^2\alpha}}
\\
\\
\cot(2\alpha) & =
\frac{\cot(\alpha)-\tan(\alpha)}{2}
\\
& = \color{blue}{\frac{\cot^2(\alpha)-1}{2 \cot(\alpha)}}
\\
\\
& = \frac{1-\tan^2\alpha}{2\tan\alpha}
\end{array}
$$

## Triple Angle Identities

> $60\degree \mapsto \frac{\pi}{3}$

### Sine

$$
\begin{array}{rl}
\sin(3\alpha) & =
3\sin(\alpha)-4\sin^3(\alpha)
\\
& \equiv
(3-4\sin^2\alpha)\sin\alpha
\\
& = 4\sin(\alpha)\sin(60\degree-\alpha)\sin(60\degree+\alpha)
\\
& = 3\cos^2(\alpha)\sin(\alpha)-\sin^3(\alpha)
\\
& \equiv
(3\cos^2(\alpha)-\sin^2(\alpha))\sin(\alpha)
\end{array}
$$

### Cosine

$$
\begin{array}{rl}
\cos(3\alpha) & =
4\cos^3(\alpha)-3\cos(\alpha)
\\
& \equiv
(4\cos^2(\alpha)-3)\cos\alpha
\\
& = 4\cos(\alpha)\cos(60\degree-\alpha)\cos(60\degree+\alpha)
\\
& = \cos^3(\alpha)-3\sin^2(\alpha)\cos(\alpha)
\\
& \equiv
(\cos^2(\alpha)-3\sin^2(\alpha))\cos(\alpha)
\end{array}
$$

### Tangent

$$
\begin{array}{rl}
\tan(3\alpha) & =
\frac{3\tan(\alpha)-\tan^3(\alpha)}{1-3\tan^2(\alpha)}
\\
& =
\frac{1-3\cot^2(\alpha)}{3\cot(\alpha)-\cot^3(\alpha)}
\\
& =
\tan(\alpha)\tan(60\degree-\alpha)\tan(60\degree+\alpha)
\end{array}
$$

### Others

$$
\begin{array}{rl}
\csc(3\alpha) & =
\frac{\csc^3(\alpha)}{3\csc^2(\alpha)-4}
\\
\\
\sec(3\alpha) & =
\frac{\sec^3\alpha}{4-3\sec^2\alpha}
\\
\\
\cot(3\alpha) & =
\frac{3\cot(\alpha)-\cot^3(\alpha)}{1-3\cot^2(\alpha)}
\\
& =
\color{blue}{\frac{1-3\tan^2(\alpha)}{3\tan(\alpha)-\tan^3(\alpha)}}
\\
& =
\cot(\alpha) \cot(60\degree-\alpha) \cot(60\degree+\alpha)
\end{array}
$$

## Half Angle Identities

### Sine

$$
\begin{array}{rl}
\sin\left(\frac{1}{2}\alpha\right)
& =
\pm \sqrt{\frac{1-\cos\alpha}{2}}
\\
& =
2\sin\left(\frac{1}{4}\alpha\right)\cos\left(\frac{1}{4}\alpha\right)
\\
& =
\sin\left(\frac{1}{6}\alpha\right)\left[3\cos^2\left(\frac{1}{6}\alpha\right)-\sin^2\left(\frac{1}{6}\alpha\right)\right]
\end{array}
$$

### Cosine

$$
\begin{array}{rl}
\cos\left(\frac{1}{2}\alpha\right)
& =
\pm \sqrt{\frac{1+\cos\alpha}{2}}
\\
& =
\cos^2\left(\frac{1}{4}\alpha\right)-\sin^2\left(\frac{1}{4}\alpha\right)
\\
& =
\cos\left(\frac{1}{6}\alpha\right)\left[\cos^2\left(\frac{1}{6}\alpha\right)-3\sin^2\left(\frac{1}{6}\alpha\right)\right]
\end{array}
$$

### Tangent

$$
\begin{array}{rl}
\tan\left(\frac{1}{2}\alpha\right)
& =
\pm \sqrt{\frac{1-\cos\alpha}{1+\cos\alpha}}
\\
& =
\frac{\sin\alpha}{1+\cos\alpha}
\\
& =
\frac{1-\cos\alpha}{\sin\alpha}
\\
& =
\csc(\alpha)-\cot(\alpha)
\\
& =
\frac{\tan\alpha}{1+\sec\alpha}
\end{array}
$$

### Others

$$
\begin{array}{rl}
\csc\left(\frac{1}{2}\alpha\right)
& =
\pm \sqrt{\frac{2}{1-\cos\alpha}}
\\
\\
\sec\left(\frac{1}{2}\alpha\right)
& =
\pm \sqrt{\frac{2}{1+\cos\alpha}}
\\
\\
\cot\left(\frac{1}{2}\alpha\right)
& =
\pm \sqrt{\frac{1+\cos\alpha}{1-\cos\alpha}}
\\
& =
\color{blue}{\frac{1+\cos\alpha}{\sin\alpha}}
\\
& =
\frac{\sin\alpha}{1-\cos\alpha}
\\
& =
\color{blue}{\csc(\alpha)+\cot(\alpha)}
\end{array}
$$

### HAI Using DAI

- sine

$$
\sin\alpha = 2\sin\left(\frac{1}{2}\alpha\right)\cos\left(\frac{1}{2}\alpha\right)
$$

- cosine

$$
\begin{array}{rl}
\cos\alpha
& =
\cos^2\left(\frac{1}{2}\alpha\right)-\sin^2\left(\frac{1}{2}\alpha\right)
\\
& =
1-2\sin^2\left(\frac{1}{2}\alpha\right)
\\
& =
2\cos^2\left(\frac{1}{2}\alpha\right)-1
\end{array}
$$

- tangent

$$
\tan\alpha =
\frac{
2\tan\left(\frac{1}{2}\alpha\right)
}{
1-\tan^2\left(\frac{1}{2}\alpha\right)
}
$$



