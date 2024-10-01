# Arithmetic Sequence: Special Sums

| | formula | formula only with $a_1$ |
|--|--|--|
| first $n$ terms | $$S_n = \frac{n}{2}(a_1+a_n)$$ | $$S_n = n\left(a_1 + \frac{1}{2}\Delta(n-1)\right)$$ |
| last $n$ terms * | $$S_{-n} = \frac{n}{2}\left(2a_L-\Delta(n-1)\right)$$ | $$S_{-n} = n\left(a_1 + \frac{1}{2}\Delta(2L-n-1)\right)$$ |
| $n$ terms starting from _k-th_ term | $$S_{n+k} = \frac{n}{2}(2a_k+\Delta(n-1))$$ | $$S_{n+k} = n\left( a_1+\frac{1}{2}\Delta(2k+n-3) \right)$$ |
| terms from _k-th_ to _t-th_ | $$S_{k → t} = \frac{1}{2}(t-k+1)(a_k+a_t)$$ | $$S_{k → t} = (t-k+1)\left( a_1+\frac{1}{2}\Delta(t+k-2) \right)$$ |

> \* - for a finite sequence $L$ in length

## Summing Every _s-th_ Term
| | formula | formula only with $a_1$ |
|--|--|--|
| first $n$ terms | $$S_n^{(s)} = \frac{n}{2}(a_1 + a_{(n-1)s+1})$$ | $$S_n^{(s)} = n\left( a_1 + \frac{1}{2}\Delta s(n-1) \right)$$ |
| last $n$ terms * | $$S_{-n}^{(s)} = \frac{n}{2} (2a_L - (n-1)\Delta s)$$ | $$S_{-n}^{(s)} = n\left( a_1 + \frac{1}{2}\Delta[ 2(L-1)-s(n-1) ] \right)$$ |
| $n$ terms starting from _k-th_ term | $$S_{n+k}^{(s)} = \frac{n}{2} (2a_k + (n-1)\Delta s)$$ | $$S_{n+k}^{(n)} = n\left(a_1 + \frac{1}{2}\Delta[2(k-1)+s(n-1)] \right)$$ |
| terms from _k-th_ to _t-th_ ** | $$S_{k → t}^{(s)} = \frac{1}{2}\left( \frac{t-k}{s} + 1 \right)(a_k + a_t)$$ | $$S_{k → t}^{(s)} = \left(\frac{t-k}{s}+1\right)\left( a_1 + \frac{1}{2}\Delta(k+t-2) \right)$$ |

> \* - for a finite sequence $L$ in length  
> \** - for $r(a,b) = a-b \cdot \lfloor \frac{a}{b} \rfloor$, if $\overline{r} = r(t-k,s) \neq 0$, then $t=t-\overline{r}, a_t=a_{t-\overline{r}}$
