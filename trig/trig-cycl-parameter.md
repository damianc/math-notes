# Trigonometric(Cyclometric(x))

|  $\square$ | $\sin(\square)$ | $\cos(\square)$ | $\tan(\square)$ |
|--|--|--|--|
| $\arcsin(x)$ | $$x$$ | $$\sqrt{1-x^2}$$ | $$\frac{x}{\sqrt{1-x^2}}$$ |
| $\arccos(x)$ | $$\sqrt{1-x^2}$$ | $$x$$ | $$\frac{\sqrt{1-x^2}}{x}$$ |
| $\arctan(x)$ | $$\frac{x}{\sqrt{1+x^2}}$$ | $$\frac{1}{\sqrt{1+x^2}}$$ | $$x$$ |
| | | | |
| $2\ \arcsin(x)$ | $$2x\sqrt{1-x^2}$$ | $$1-2x^2$$ | $$\frac{2x\sqrt{1-x^2}}{1-2x^2}$$ |
| $2\ \arccos(x)$ | $$2x\sqrt{1-x^2}$$ | $$2x^2-1$$ | $$\frac{2x\sqrt{1-x^2}}{2x^2-1}$$ |
| $2\ \arctan(x)$ | $$\frac{2x}{1+x^2}$$ | $$\frac{2}{1+x^2}-1$$ | $$\frac{2x}{1-x^2}$$ |

> examples: $\cos(\arcsin(x)) = \sqrt{1-x^2}$, $\cos(2\ \arcsin(x)) = 1-2x^2$

## Addition/Subtraction of Angles

| $\square$ | $\sin(\square)$ | $\cos(\square)$ |
|--|--|--|
| $90°+\arcsin(x)$ | $\sqrt{1-x^2}$ | $-x$ |
| $90°-\arcsin(x)$ | $\sqrt{1-x^2}$ | $x$ |
| $\arcsin(x)-90°$ | $-\sqrt{1-x^2}$ | $x$ |
| $90°+\arccos(x)$ | $x$ | $-\sqrt{1-x^2}$ |
| $90°-\arccos(x)$ | $x$ | $\sqrt{1-x^2}$ |
| $\arccos(x)-90°$ | $-x$ | $\sqrt{1-x^2}$ |

Remaining values can be obtained with use of the following identities:

- $\sin(90°+\theta) = \cos(\theta)$
- $\sin(90°-\theta) = \cos(\theta)$
- $\cos(90°+\theta) = -\sin(\theta)$
- $\cos(90°-\theta) = \sin(\theta)$
- $\tan(90°+\theta) = -\cot(\theta)$
- $\tan(90°-\theta) = \cot(\theta)$
- $\cot(\theta) = \frac{1}{\tan(\theta)}$

and:

- $\sin(\alpha-\beta) = -\sin(\beta-\alpha)$
- $\cos(\alpha-\beta) = \cos(\beta-\alpha)$
- $\tan(\alpha-\beta) = -\tan(\beta-\alpha)$

For example:

$$
\begin{array}{rl}
\tan(90°-\arcsin(x)) & = \cot(\arcsin(x))
\\
& = [\ \tan(\arcsin(x))\ ]^{-1}
\\
& = \left[\ \frac{x}{\sqrt{1-x^2}}\ \right]^{-1}
\\
& = \frac{\sqrt{1-x^2}}{x}
\end{array}
$$

$$
\begin{array}{rl}
\sin(90°+2 \arccos(x)) & = \cos(2 \arccos(x))
\\
& = 2x^2-1
\end{array}
$$

For summand other than $90°$ [function of sum/difference identities](https://github.com/damianc/math-notes/blob/master/trig/functions-of-sum-diff.md) can be used, for example:

$$
\begin{array}{rl}
\tan(\theta-\arctan(x)) & = \frac{
\tan(\theta)-\tan(\arctan(x))
}{
1+\tan(\theta)\tan(\arctan(x))
}
\\
& = \frac{\tan(\theta)-x}{1+x \tan(\theta)}
\end{array}
$$
