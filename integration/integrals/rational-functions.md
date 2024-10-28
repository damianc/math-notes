# Integrals of Rational Functions

For function with a sum in the numerator, its integral can be split:

$$
\int \frac{ax^p+bx^q+\cdots}{P(x)}\ dx =
\int \frac{ax^p}{P(x)}\ dx + \int \frac{bx^q}{P(x})\ dx + \cdots
$$

## Denominator as a Linear Function

| $f(x)$ | $\int f(x)\ dx$ |
|--|--|
| $$\frac{kx}{ax+b}$$ | $$\frac{1}{a^2}\Bigl[k(ax-b \ln(ax+b))\Bigr]$$ |
| $$\frac{ax+b}{cx+d}$$ | $$\frac{1}{c^2}\Bigl[(bc-ad) \ln(cx+d)+acx\Bigr]$$ |

## Denominator as a Quadratic Function

| $f(x)$ | $\int f(x)\ dx$ |
|--|--|
| $$\frac{kx}{ax^2+bx}$$ | $$\frac{1}{a}\Bigl[k \ln(ax+b)\Bigr]$$ |
| $$\frac{ax+b}{cx^2+dx}$$ | $$\frac{1}{cd}\Bigl[(ad-bc)\ln(cx+d)+bc\ln(x)\Bigr]$$ |
| $$\frac{kx}{ax^2+b}$$ | $$\frac{1}{2a}\Bigl[k \ln(ax^2+b)\Bigr]$$ |
| $$\frac{ax+b}{cx^2+d}$$ | $$\frac{a \ln(cx^2+d)}{2c}+\frac{b \arctan\left(\frac{\sqrt{c}\ x}{\sqrt{d}}\right)}{\sqrt{c}\sqrt{d}}$$ |
| $$\frac{kx}{ax^2+bx+c}$$ | $$\frac{k}{2a}\Bigl[\ln(x(ax+b)+c)-\frac{2b\arctan\left(\large{\frac{2ax+b}{\nabla}}\right)}{\nabla}\Bigr]$$ |
| | $$\nabla = \sqrt{4ac-b^2}$$ |
| $$\frac{ax+b}{cx^2+tx+e}$$ | $$\frac{1}{2c}\Bigl[a\ln(x(cx+t)+e)-\frac{2(at-2bc)\arctan\left(\large{\frac{2cx+t}{\nabla}}\right)}{\nabla}\Bigr]$$ |
| | $$\nabla = \sqrt{ce-t^2}$$ |

