# Riemann Sum

A **Riemann sum** is a kind of approximation of an integral by a finite sum.

## Left Rule

**Left (hand) rule** (_LHR_) gets a **left Riemann sum**:

$$
\int_a^b f(x) \ dx \approx
\Delta \sum_{i=1}^n f(x_{i-1})
$$

> $x_i = a+\Delta i, \quad i \geq 0$,
> $\Delta = \frac{b-a}{n}, \quad n \in \Bbb{N}$

## Right Rule

**Right (hand) rule** (_RHR_) gets a **right Riemann sum**:

$$
\int_a^b f(x) \ dx \approx
\Delta \sum_{i=1}^n f(x_i)
$$

## Midpoint Rule

**Midpoint rule** (_MPR_) gets a **middle Riemann sum**:

$$
\int_a^b f(x) \ dx \approx
\Delta \sum_{i=1}^n f\left(
\frac{x_{i-1} + x_i}{2}
\right)
$$


