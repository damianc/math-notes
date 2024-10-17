# Derivatives Rules

| Rule | Formula |
|--|--|
| power rule | $$\large [x^n]' = nx^{n-1}$$ |
| constant rule | $$\large C' = 0$$ |
| constant multiple rule | $$\large [C\ f(x)]' = C\ f'(x)$$ |
| sum/difference rule | $$\large [f(x) \pm g(x)]' = f'(x) \pm g'(x)$$ |
| chain rule | $$\large [f(g(x))]' = f'(g(x))g'(x)$$ |
| product rule | $$\large [f(x)g(x)]' = f(x)g'(x) + g(x)f'(x)$$ |
| quotient rule | $$\large \left[\frac{f(x)}{g(x)}\right]' = \frac{g(x)f'(x)-f(x)g'(x)}{[g(x)]^2}$$ |

## Examples

### Power Rule

$$
\large
[x^n]' = nx^{n-1}
$$

for example:

$$
[x^3]' = 3x^2
$$

### Constant Rule

$$
\large
C' = 0
$$

for example:

$$
[2]' = 0
$$

### Constant Multiple Rule

$$
\large
[C\ f(x)]' = C\ f'(x)
$$

for example:

$$
\begin{array}{rl}
[2x^2]' & = 2 \cdot [x^2]'
\\
& = 2 \cdot 2x
\\
& = 4x
\end{array}
$$

### Sum/Difference Rule

$$
\large
[f(x) \pm g(x)]' = f'(x) \pm g'(x)
$$

for example:

$$
\begin{array}{rl}
[\sin(x)+\cos(x)]' & = [\sin(x)]' + [\cos(x)]'
\\
& = \cos(x) - \sin(x)
\end{array}
$$

### Chain Rule

$$
\large
[f(g(x))]' = f'(g(x))g'(x)
$$

for example:

$$
\begin{array}{rl}
[\sin(x^2)]' & = \sin'(x^2) \cdot [x^2]'
\\
& = 2x \cos(x^2)
\end{array}
$$

### Product Rule

$$
\large
[f(x)g(x)]' = f(x)g'(x) + g(x)f'(x)
$$

for example:

$$
\begin{array}{rl}
[2x \cdot \sin(x)]' & = 2x \cdot [\sin(x)]' + \sin(x) \cdot [2x]'
\\
& = 2x \cdot \cos(x) + \sin(x) \cdot 2
\\
& = 2(x \cos(x) + \sin(x))
\end{array}
$$

### Quotient Rule

$$
\large
\left[\frac{f(x)}{g(x)}\right]' = \frac{g(x)f'(x) - f(x)g'(x)}{[g(x)]^2}
$$

for example:

$$
\begin{array}{rl}
\left[
\frac{\sin(x)}{2x}
\right]' & = \frac{
2x \cdot [\sin(x)]' - \sin(x) \cdot [2x]'
}{[2x]^2}
\\
& = \frac{
2x \cdot \cos(x) - \sin(x) \cdot 2
}{4x^2}
\\
& = \frac{
x \cos(x) - \sin(x)
}{2x^2}
\end{array}
$$


