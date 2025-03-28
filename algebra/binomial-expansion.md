# Binomial Expansion

$$
\begin{array}{rl}
\large{\boldsymbol{(a+b)^n}} &
\large{=} &
\large{\displaystyle
\sum_{k=0}^n \binom{n}{k}
a^{n-k} b^k
}
\\
\ 
\\
& &
\small{\color{#aaa}\text{where }}
\color{#888}
\binom{n}{k} = \frac{n!}{k!(n-k)!}
\end{array}
$$

$$
\begin{array}{rcl}
\boldsymbol{(a+b)^2} & = &
a^2+2ab+b^2
\\
\\
\boldsymbol{(a+b)^3} & = &
a^3+3a^2b\ +
\\
& & b^3 + 3ab^2
\\
\\
\boldsymbol{(a+b)^4} & = &
a^4+4a^3b\ +
\\
& & 6a^2b^2\ +
\\
& & b^4 + 4ab^3
\\
\\
\boldsymbol{(a+b)^5} & = &
a^5 + 5a^4b + 10a^3b^2\ +
\\
& & b^5 + 5ab^4 + 10a^2b^3
\\
\\
\boldsymbol{(a+b)^6} & = &
a^6+6a^5b+15a^4b^2\ +
\\
& & 20a^3b^3\ +
\\
& & b^6+6ab^5+15a^2b^4
\\
\\
\boldsymbol{(a+b)^7} & = &
a^7+7a^6b+21a^5b^2+35a^4b^3
\\
& & b^7+7ab^6+21a^2b^5+35a^3b^4
\\
\\
\boldsymbol{(a+b)^8} & = &
a^8+8a^7b+28a^6b^2+56a^5b^3\ +
\\
& & 70a^4b^4\ +
\\
& & b^8+8ab^7+28a^2b^6+56a^3b^5
\\
\\
\boldsymbol{(a+b)^9} & = &
a^9+9a^8b+36a^7b^2\ +
\\
& & 84a^6b^3\ + 126a^5b^4\ +
\\
& & b^9+9ab^8+36a^2b^7\ +
\\
& & 84a^3b^6\ + 126a^4b^5
\\
\\
\boldsymbol{(a+b)^{10}} & = &
a^{10}+10a^9b+45a^8b^2\ +
\\
& & 120a^7b^3+210a^6b^4\ +
\\
& & 252a^5b^5\ +
\\
& & b^{10}+10ab^9+45a^2b^8\ +
\\
& & 120a^3b^7+210a^4b^6
\end{array}
$$

## Alternative Representation

$$
\begin{array}{l}
\text{given:}
\\
{\large\lambda}^a_b(m,n) = a^m b^n + a^n b^m
\\
k = \left\lceil \frac{n+1}{2} \right\rceil
\\
\\
{\large (a+b)^n} = \displaystyle\sum_{i=0}^{k-1}
\binom{n}{i}
{\Large\lambda}^a_b(n-i,i)
\end{array}
$$
