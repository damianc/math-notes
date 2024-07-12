# Permutations and Combinations with Repetition

## Permutations with Repetition

Number of ways all terms can be arranged, given _i-th_ term $n_i$ occurs $i$ times.

$$
\large
\overline{P}_{n_1,...,n_k} = \cfrac
{\left[ \sum n_i \right]!}
{\prod [n_i !]}
$$

For example, having to arrange 2 letters $a$ and 2 letters $b$, i.e., $(a,a,b,b)$:

- $n_1 = 2$ ( $a,a$ )
- $n_2 = 2$ ( $b,b$ )

$$
\overline{P}_{2,2} =
\frac{(2+2)!}{2! \cdot 2!} =
\frac{24}{4} = 6
$$

> The possibilities are as follows: $(aabb,abab,abba,bbaa,baba,baab)$


## Combinations with Repetition

Number of ways $k$ terms can be chosen from among $n$ terms, given one term can be chosen multiple times.

$$
\large
\overline{C_n^k} =
C_{n+k-1}^k =
\frac{(n+k-1)!}{k!(n-1)!}
$$

For example, having to pick 2 letters from among 4 letters $(a,b,c,d)$, given one letter can be picked multiple times:

- $k = 2$
- $n = 4$

$$
\overline{C_4^2} = C_5^2 =
\frac{5!}{2! \cdot 3!} = 10
$$

> The possibilities are as follows:

$$
\begin{bmatrix}
aa & ba & ca & da
\\
{\color{#aaa}ab} & bb & cb & db
\\
{\color{#aaa}ac} & {\color{#aaa}bc} & cc & dc
\\
{\color{#aaa}ad} & {\color{#aaa}bd} & {\color{#aaa}cd} & dd
\end{bmatrix}
$$

> Gray terms are not counted as in combinations $(a,b) \equiv (b,a)$.
