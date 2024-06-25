# Fresnel Integrals

$$
\begin{array}{rcl}
S(u) & = &
\displaystyle
\int_0^u \sin(x^2)\ dx
\\
\\
C(u) & = &
\displaystyle
\int_0^u \cos(x^2)\ dx
\end{array}
$$

## Normalized Fresnel Integrals

$$
\begin{array}{rcl}
S(u) & = &
\displaystyle
\int_0^u \sin\left(\frac{\pi}{2} x^2\right)\ dx
\\
\\
C(u) & = &
\displaystyle
\int_0^u \cos\left(\frac{\pi}{2} x^2\right)\ dx
\end{array}
$$

## Use Examples

$$
\begin{array}{rcl}
\int \sin(ax^2)\ dx & = &
\frac{1}{\sqrt{a}} \left[
\sqrt{\frac{\pi}{2}}\ S(\nabla x)
\right]
\\
\\
\int \cos(ax^2)\ dx & = &
\frac{1}{\sqrt{a}} \left[
\sqrt{\frac{\pi}{2}}\ C(\nabla x)
\right]
\\
\\
\int \sin(ax^2+b)\ dx & = &
\frac{1}{\sqrt{a}} \left[
\sqrt{\frac{\pi}{2}}\
(\sin(b)\ C(\nabla x) +
\\
\cos(b)\ S(\nabla x))
\right]
\\
\\
\int \cos(ax^2+b)\ dx & = &
\frac{1}{\sqrt{a}} \left[
\sqrt{\frac{\pi}{2}}\
(\cos(b)\ C(\nabla x) -
\\
\sin(b)\ S(\nabla x))
\right]
\end{array}
$$
