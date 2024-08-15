# Generalized Union and Intersection of Sets

- generalized union:

$$
\bigcup_{n=1}^k A_n = A_1 \cup A_2 \cup \cdots \cup A_k
$$

- generalized intersection:

$$
\bigcap_{n=1}^k A_n = A_1 \cap A_2 \cap \cdots \cap A_k
$$

## Other Forms

| Union | Intersection |
|--|--|
| $$\bigcup_{n \in \Bbb N} A_n = \bigcup_{n=1}^{\infty} A_n$$ | $$\bigcap_{n \in \Bbb N} A_n = \bigcap_{n=1}^{\infty} A_n$$ |
| $$\bigcup_{n \in T} A_n = \bigcup_{n=1}^{\vert T \vert} A_n$$ | $$\bigcap_{n \in T} A_n = \bigcap_{n=1}^{\vert T \vert} A_n$$ |
| $$\bigcup_{1 \le n \le k} A_n = \bigcup_{n=1}^k A_n$$ | $$\bigcap_{1 \le n \le k} A_n = \bigcap_{n=1}^k A_n$$ |

## Membership Properties

- generalized union:

$$
\left( x \in \bigcup_{t \in T} A_t \right)
\iff
\underset{t \in T}{\large\exists}
\left( x \in A_t \right)
$$

$$
\left( x \notin \bigcup_{t \in T} A_t \right)\iff\underset{t \in T}{\large\forall}\left( x \notin A_t \right)
$$

- generalized intersection:

$$
\left( x \in \bigcap_{t \in T} A_t \right)
\iff
\underset{t \in T}{\large\forall}
\left( x \in A_t \right)
$$

$$
\left( x \notin \bigcap_{t \in T} A_t \right)
\iff
\underset{t \in T}{\large\exists}
\left( x \notin A_t \right)$$

## Example

indexing set:  
$I = \\{ 1,2 \\}$

indexed family:  
${\cal F} = \\{ A_i \\}_{i \in I} = \\{ A_1,A_2 \\}$

_i-th_ term of ${\cal F}$:  
$A_i = \\{ i,2i \\}$

terms of ${\cal F}$:

$$
\begin{array}{rcl}
A_1 & = & \\{ 1,2 \\}
\\
A_2 & = & \\{ 2,4 \\}
\end{array}
$$

generalized union and intersection:

$$
\begin{array}{rcl}
\displaystyle\bigcup_{i \in I} A_i & = & A_1 \cup A_2
\\
& = & \\{ 1,2,4 \\}
\\
\\
\displaystyle\bigcap_{i \in I} A_i & = & A_1 \cap A_2
\\
& = & \\{ 2 \\}
\end{array}
$$

## Analogy to Sigma/Pi Notation

$\displaystyle\bigcup_{i \in I}$ is similar to $\displaystyle\sum_{i \in I}$, but with terms being sets rather than numbers, and hence with operation $A \cup B$ instead of $A+B$:

$$
\begin{array}{lcl}
\displaystyle\sum_{n \in \Bbb N} n & = &
1+2+3+4+\cdots
\\
\\
\displaystyle\bigcup_{n \in \Bbb N} A_n & = &
A_1 \cup A_2 \cup A_3 \cup A_4 \cup \cdots
\end{array}
$$

the same holds for $\displaystyle\bigcap_{i \in I}$ and $\displaystyle\prod_{i \in I}$ with operation $A \cap B$ instead of $A \cdot B$:

$$
\begin{array}{lcl}
\displaystyle\prod_{n \in \Bbb N} n & = &
1 \cdot 2 \cdot 3 \cdot 4 \cdot \cdots
\\
\\
\displaystyle\bigcap_{n \in \Bbb N} A_n & = &
A_1 \cap A_2 \cap A_3 \cap A_4 \cap \cdots
\end{array}
$$
