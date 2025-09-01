# Factorial and Multifactorial

## Factorial

Product of $n$ consecutive numbers:


$$
\begin{array}{rl}
n! & = 1 \cdot 2 \cdot 3 \ \cdots \ (n-1) \cdot n
\\
& = \displaystyle\prod_{k=0}^{n-1} \ k
\end{array}
$$

For example:
- $2! = 1 \cdot 2 \tiny = 2$
- $4! = 1 \cdot 2 \cdot 3 \cdot 4 \tiny = 24$

## Double Factorial

> ${\color{red} n!! \neq (n!)!}$

**Multifactorial** described in the next chapter below for $k=2$:

$$
\begin{array}{rl}
n!! & = n(n-2)(n-4) \ \cdots
\\
& = \displaystyle\prod_{k=0}^t (n-2k), \text{ where } t = \left\lfloor\frac{n}{2}\right\rfloor-1
\end{array}
$$

For example:

- $8!! = 8 \cdot 6 \cdot 4 \cdot 2 \tiny = 384$
- $5!! = 5 \cdot 3 \cdot 1 \tiny = 15$

## Multifactorial

$$
\begin{array}{rl}
n\underbrace{! \cdots !}\_{\times k} = n!^{(k)} & = n(n-k)(n-2k) \ \cdots
\\
& = \displaystyle\prod_{p=0}^t (n-pk), \text{ where } t = \left\lfloor\frac{n-1}{k}\right\rfloor
\end{array}
$$

> $n!! = n!^{(2)}$

For example:

- $6!! = 6!^{(2)} = 6 \cdot 4 \cdot 2 \tiny = 48$
- $9!!! = 9!^{(3)} = 9 \cdot 6 \cdot 3 \tiny = 162$
- $15!^{(5)} = 15 \cdot 10 \cdot 5 \tiny = 750$
- $20!^{(8)} = 20 \cdot 12 \cdot 4 \tiny = 960$

Basic multifactorials include:

| | |
|--|--|
| double factorial | $n!! = n(n-2)(n-4) \cdots$ |
| triple factorial | $n!!! = n(n-3)(n-6) \cdots$ |
| quadruple factorial | $n!!!! = n(n-4)(n-8) \cdots$ |
| quintuple factorial | $n!!!!! = n(n-5)(n-10) \cdots$ |
