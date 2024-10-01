# Arithmetic Sequence

Arithemic sequence is a sequence in which _n-th_ term is defined as:

$$
a_n = a_{n-1}+\Delta
$$

For example, for a difference factor $\Delta = 2$ and the very first term $a_1=0$, the sequence starts as follows:

$$
0,2,4,6,8,10,12,14,...
$$

> the difference factor $\Delta$ can be negative and form a descending sequence like $4,2,0,-2,-4,-6,...$

> every term is arithmetic mean of its siblings: $a_{n+1} = \frac{a_n+a_{n+2}}{2}$

Arithmetic sequence may be defined in set-builder notation as:

$$
\\{ a_1 + (n-1)\Delta \vert n \geqslant 1 \\}
$$

## Getting _n-th_ Term

$$
a_n = a_1 + (n-1)\Delta
$$

- by _k-th_ term:

$$
a_n = a_k + (n-k)\Delta
$$

## Sum of $n$ First Terms

$$
S_n = \left[ a_1+ \frac{(n-1)\Delta}{2} \right] \cdot n
$$

or as repeated $n$ times arithmetic mean of first and last terms:

$$
S_n = \frac{a_1+a_n}{2} \cdot n
$$

## Other Formulas

- position of term $x$:

$$
n = 1+\frac{x-a_1}{\Delta}
$$

- size of a finite sequence (with $z$ being the last term):

$$
L = 1+\frac{z-a_1}{\Delta}
$$

- _m-th_ term by _k-th_ and _n-th_ terms ($k \lt m \lt n$):

$$
a_m = a_k + \frac{(n-2k+1)(a_n-a_k)}{n-k}
$$

## Constructing a Sequence

$$
\Delta = \frac{a_n-a_1}{n-1}
$$

Where:
- $a_1$ - first term
- $a_n$ - last term
- $n$ - desired length of the sequence

For example, if $a_1=4$, $a_n=24$ and $n=6$:

$$
\Delta = \frac{24-4}{6-1} = 4
$$

| $a_1$ | $a_2$ | $a_3$ | $a_4$ | $a_5$ | $a_6$ |
|--|--|--|--|--|--|
| 4 | 8 | 12 | 16 | 20 | 24 |
