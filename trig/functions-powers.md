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

| $n$ | Formula |
|--|--|
| odd | $\displaystyle\sin^n(\theta) = \frac{2}{2^n}\sum_{k=0}^{\frac{n-1}{2}}(-1)^{\frac{n-1}{2}-k}\binom{n}{k}\sin((n-2k)\theta)$ |
| even | $\displaystyle\sin^n(\theta) = \frac{1}{2^n}\binom{n}{n/2} + \frac{2}{2^n}\sum_{k=0}^{\frac{n}{2}-1}(-1)^{\frac{n}{2}-k}\binom{n}{k}\cos((n-2k)\theta)$ |

or:

| $\sin$ | Formula |
|--|--|
| $\sin^{2n}(x)$ | $\displaystyle \frac{1}{2^{2n}} \binom{2n}{n} + \frac{(-1)^n}{2^{2n-1}} \sum_{k=0}^{n-1} (-1)^k \binom{2n}{k} \cos(2(n-k)x)$ |
| $\sin^{2n+1}(x)$ | $\displaystyle \frac{(-1)^n}{4^n} \sum_{k=0}^{n} (-1)^k \binom{2n+1}{k} \sin((2n+1-2k)x)$ |

### Cosine

| $n$ | Formula |
|--|--|
| odd | $\displaystyle\cos^n(\theta) = \frac{2}{2^n}\sum_{k=0}^{\frac{n-1}{2}}\binom{n}{k}\cos((n-2k)\theta)$ |
| even | $\displaystyle\cos^n(\theta) = \frac{1}{2^n}\binom{n}{n/2} + \frac{2}{2^n}\sum_{k=0}^{\frac{n}{2}-1}\binom{n}{k}\cos((n-2k)\theta)$ |

or:

| $sin$ | Formula |
|--|--|
| $\cos^{2n}(x)$ | $\displaystyle\frac{1}{2^{2n}} \binom{2n}{n} + \frac{1}{2^{2n-1}} \sum_{k=0}^{n-1} \binom{2n}{k} \cos(2(n-k)x)$ |
| $\cos^{2n+1}(x)$ | $\displaystyle\frac{1}{4^n} \sum_{k=0}^{n} \binom{2n+1}{k} \cos((2n+1-2k)x)$ |

> $\binom{n}{k} = \frac{n!}{k!\ \cdot\ (n-k)!}$
