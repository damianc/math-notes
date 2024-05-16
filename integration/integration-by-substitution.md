# Integration by Substitution

| Step | Example 1 | Example 2 |
|--|--|--|
| | $\int \sin(mx+p)\ dx$ | $\int f(3x+4)\ dx$ |
| | | with $f(x)=2x+1$ |
| __1__.Let $u$ be assigned an expression (inner function) | $u=mx+p$ | $u=3x+4$ |
| __2__.Differentiate $u$: $du=u'\ dx$ | $du=m\ dx$ | $du=3\ dx$ |
| __3__.Get $dx$ from $du$ | $dx=\frac{du}{m}$ | $dx=\frac{du}{3}$ |
| __4__.Rewrite the integral with changed expression and $dx$ | $\int \sin(u)\ \frac{du}{m}$ | $\int f(u)\ \frac{du}{3}$ |
| __4a__.Pull out $du$ | $\int \sin(u)\ \frac{1}{m}\ du$ | $\int f(u)\ \frac{1}{3}\ du$ |
| | $=\int \frac{1}{m}\sin(u)\ du$ | $=\int \frac{1}{3}f(u)\ du$ |
| __4b__.Move constant value before the integral | $\frac{1}{m}\int \sin(u)\ du$ | $\frac{1}{3}\int f(u)\ du$ |
| __5__.Compute the integral | $\frac{1}{m}[-\cos(u)]+C$ | $\frac{1}{3}[u^2+u]+C$ |
| __6__.Restore expression from $u$ | $\frac{1}{m}[-\cos(mx+p)]+C$ | $\frac{1}{3}[(3x+4)^2+(3x+4)]+C$ |
| | | $=\frac{1}{3}(9x^2+16+24x+3x+4)+C$ |
| __6a__.Reduce and/or rearrange the final expression | $-\frac{1}{m}\cos(mx+p)+C$ | $\frac{1}{3}(9x^2+27x+20)+C$ |
| __DONE__ | $\int \sin(mx+p)\ dx\ =$ | $\int 2(F:x \mapsto 3x+4)+1\ dx\ =$ |
| | $-\frac{1}{m}\cos(mx+p)+C$ | $\frac{1}{3}(9x^2+27x+20)+C$ |
