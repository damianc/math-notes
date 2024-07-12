# Combinatorial Analysis

| Number of ... | Formula |
|--|--|
| permutations | $$P_n = n!$$ |
| combinations | $$C_n^k = \binom{n}{k} = \frac{n!}{k!(n-k)!}$$ |
| variations without repetition | $$V_{\ n}^k = \frac{n!}{(n-k)!}$$ |
| variations with repetition | $$W_n^k = n^k$$ |

## Permutations

$$
\large
P_n = n!
$$

Number of ways all $n$ terms can be arranged.

## Combinations

$$
\large
C_n^k = \binom{n}{k} =
\frac{n!}{k!(n-k)!}
$$

Number of ways $k$ terms can be chosen from among $n$ terms.

## Variations

Number of sequences $k$ in length that can be constructed using terms of a set $n$ in size...

### Variations without Repetition

... given one term can be picked one time.

$$
\large
V_{\ n}^k = \frac{n!}{(n-k)!} =
\prod_{i=0}^{k-1} n-i
$$

### Variations with Repetition

... given one term can be picked multiple times.

$$
\large
W_n^k = n^k =
\prod_{i=1}^k n
$$

## Combinations vs Variations

- in terms of **combinations**: $(a,b) \equiv (b,a)$
- in terms of **variations**: $(a,b) \not\equiv (b,a)$
