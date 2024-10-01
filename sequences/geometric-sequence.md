# Geometric Sequence

Geometric sequence is a sequence in which _n-th_ term is defined as:

$$
a_n = a_{n-1} \cdot \Delta
$$

For example, if the very first term $a_1=2$:

- for $\Delta=2$, the sequence is $2,4,8,16,32,64,...$
- for $\Delta=-2$, the sequence is $2,-4,8,-16,32,-64,...$
- for $\Delta=0.5$, the sequence is $2,1,\frac{1}{2},\frac{1}{4},\frac{1}{8},\frac{1}{16},...$

Geometric sequence may be defined in set-builder notation as:

$$
\\{ a_1 \cdot \Delta^{n-1} \vert n \geqslant 1 \\}
$$

## Getting _n-th_ Term

$$
a_n = a_1 \cdot \Delta^{n-1}
$$

- by _k-th_ term:

$$
a_n = a_k \cdot \Delta^{n-k}
$$

## Sum of $n$ First Terms

$$
S_n = \begin{cases}
a_1 \cdot \frac{1-\Delta^n}{1-\Delta} & \text{if } \Delta \neq 1
\\
a_1 \cdot n & \text{if } \Delta=1
\end{cases}
$$

## Constructing a Sequence

$$
\Delta = \sqrt[n-1]{\frac{a_n}{a_1}}
$$

Where:
- $a_1$ - first term
- $a_n$ - last term
- $n$ - desired length of the sequence

For example, if $a_1=2$, $a_n=16$ and $n=4$:

$$
\Delta = \sqrt[4-1]{\frac{16}{2}} = \sqrt[3]{8} = 2
$$

| $a_1$ | $a_2$ | $a_3$ | $a_4$ |
|--|--|--|--|
| 2 | 4 | 8 | 16 |
