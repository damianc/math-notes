# Law of Sines

![Triangle and Law of Sines](https://raw.githubusercontent.com/damianc/math-notes/refs/heads/master/_images/trigonometry/law-of-sines.png)

$$
\large
\frac{a}{\sin\alpha} = \frac{b}{\sin\beta} = \frac{c}{\sin\gamma} = 2R
$$

- with the above, sides of the triangle can be read:

$$
\begin{array}{l}
a = 2R \sin(\alpha)
\\
b = 2R \sin(\beta)
\\
c = 2R \sin(\gamma)
\end{array}
$$

- as well as sines of its angles:

$$
\begin{array}{l}
\sin(\alpha) = \frac{a}{2R}
\\
\sin(\beta) = \frac{b}{2R}
\\
\sin(\gamma) = \frac{c}{2R}
\end{array}
$$

## Extension to Incircle

![Triangle and Extended Law of Sines](https://raw.githubusercontent.com/damianc/math-notes/refs/heads/master/_images/trigonometry/law-of-sines-extended.png)

$$
\large
\frac{bc \sin\alpha}{a+b+c} = \frac{ac \sin\beta}{a+b+c} = \frac{ab \sin\gamma}{a+b+c} = r
$$

- with the above, sines of the angles of the triangle can be read:

$$
\begin{array}{l}
\sin(\alpha) = \frac{r(a+b+c)}{bc}
\\
\sin(\beta) = \frac{r(a+b+c)}{ac}
\\
\sin(\gamma) = \frac{r(a+b+c)}{ab}
\end{array}
$$

- as well as its sides:

| side | by $\sin(\alpha)$ | by $\sin(\beta)$ | by $\sin(\gamma)$ |
|--|--|--|--|
| $a$ | $$\frac{bc \sin(\alpha)}{r}-(b+c)$$ | $$\frac{r(b+c)}{c \sin(\beta)-r}$$ | $$\frac{r(b+c)}{b \sin(\gamma)-r}$$ |
| $b$ | $$\frac{r(a+c)}{c \sin(\alpha)-r}$$ | $$\frac{ac \sin(\beta)}{r}-(a+c)$$ | $$\frac{r(a+c)}{a \sin(\gamma)-r}$$ |
| $c$ | $$\frac{r(a+b)}{b \sin(\alpha)-r}$$ | $$\frac{r(a+b)}{a \sin(\beta)-r}$$ | $$\frac{ab \sin(\gamma)}{r}-(a+b)$$ |
