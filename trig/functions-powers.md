# Trigonometric Functions Power

## Power of 2

$$
\begin{array}{ll}
\sin^2(\theta) & = 1-\cos^2(\theta)
\\
& = \frac{1}{2}[1-\cos(2\theta)]
\\
\\
\cos^2(\theta) & = 1-\sin^2(\theta)
\\
& = \frac{1}{2}[\cos(2\theta)+1]
\end{array}
$$

## Power of 3

$$
\begin{array}{ll}
\sin^3(\theta) & =
\frac{1}{4}[3 \sin(\theta) - \sin(3\theta)]
\\
\\
\cos^3(\theta) & =
\frac{1}{4}[3 \cos(\theta) + \cos(3\theta)]
\end{array}
$$

## Power of 4

$$
\begin{array}{ll}
\sin^4(\theta) & =
\frac{1}{8}[3 - 4\cos(2\theta) + \cos(4\theta)]
\\
\\
\cos^4(\theta) & =
\frac{1}{8}[3 + 4\cos(2\theta) + \cos(4\theta)]
\end{array}
$$

## Power of 5

$$
\begin{array}{ll}
\sin^5(\theta) & =
\frac{1}{16}[10 \sin(\theta) - 5\sin(3\theta) + \sin(5\theta)]
\\
\\
\cos^5(\theta) & =
\frac{1}{16}[10 \cos(\theta) + 5\cos(3\theta) + \cos(5\theta)]
\end{array}
$$

## Power of $n$

### Sine

- if $n$ is odd:

$$
\sin^n(\theta) = \frac{2}{2^n}
\sum_{k=0}^{\frac{n-1}{2}}
(-1)^{\frac{n-1}{2}-k}
\binom{n}{k}
\sin((n-2k)\theta)
$$

- if $n$ is even:

$$
\sin^n(\theta) = \frac{1}{2^n}
\binom{n}{n/2} +
\frac{2}{2^n}
\sum_{k=0}^{\frac{n}{2}-1}
(-1)^{\frac{n}{2}-k}
\binom{n}{k}
\cos((n-2k)\theta)
$$
