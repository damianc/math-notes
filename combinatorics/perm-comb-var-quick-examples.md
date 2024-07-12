# Quick Examples of Permutations, Combinations and Variations

## Permutations

### Without Repetition

Number of ways to arrange $(a,b,c)$:

$$
P_3 = 3! = 6
$$

$$
\begin{bmatrix}
abc & acb
\\
bac & bca
\\
cab & cba
\end{bmatrix}
$$

### With Repetition

Number of ways to arrange $(a,a,b,c)$:

$$
P_{2,1,1} = \frac{(2+1+1)!}{2! \cdot 1! \cdot 1!} =
\frac{4!}{2!} = \frac{24}{2} = 12
$$

$$
\begin{bmatrix}
aabc & baac & bcaa
\\
aacb & caab & cbaa
\\
\\
abca & abac & baca
\\
acba & acab & caba
\end{bmatrix}
$$

## Combinations

### Without Repetition

Number of ways to pick 2 terms from $\\{a,b,c\\}$:

$$
C^2_3 = \frac{3!}{2! \cdot 1!} =
\frac{6}{2} = 3
$$

$$
\begin{bmatrix}
\- & ab & ac
\\
\cancel{ba} & \- & bc
\\
\cancel{ca} & \cancel{cb} & \-
\end{bmatrix}
$$

### With Repetition

Number of ways to pick 2 terms from $\\{a,b,c\\}$, having possibility to pick one term multiple times:

$$
\overline{C^2_3} = C^2_4 =
\frac{4!}{2! \cdot 2!} = \frac{24}{4} = 6
$$

$$
\begin{bmatrix}
aa & ab & ac
\\
\cancel{ba} & bb & bc
\\
\cancel{ca} & \cancel{cb} & cc
\end{bmatrix}
$$

## Variations

### Without Repetition

Number of ways to arrange 2 terms from $\\{a,b,c\\}$:

$$
V^2_{\ 3} = \frac{3!}{1!} = 3! = 6
$$

$$
\begin{bmatrix}
\- & ab & ac
\\
ba & \- & bc
\\
ca & cb & \-
\end{bmatrix}
$$

### With Repetition

Number of ways to arrange 2 terms from $\\{a,b,c\\}$, having possibility to pick one term multiple times:

$$
W^2_{\ 3} = 3^2 = 9
$$

$$
\begin{bmatrix}
aa & ab & ac
\\
ba & bb & bc
\\
ca & cb & cc
\end{bmatrix}
$$
