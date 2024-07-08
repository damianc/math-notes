# MathJax Text

## Font Style

```
\STYLE{text}
```

| Style | Preview | Style | Preview |
|--|--|--|--|
| `mathnormal` | $\mathnormal{ABC\ abc\ 123}$ | `textnormal` | $\textnormal{ABC\ abc\ 123}$ |
| `mathrm` | $\mathrm{ABC\ abc\ 123}$ | `textrm` | $\textrm{ABC\ abc\ 123}$ |
| `mathsf` | $\mathsf{ABC\ abc\ 123}$ | `textsf` | $\textsf{ABC\ abc\ 123}$ |
| `mathbf` | $\mathbf{ABC\ abc\ 123}$ | `textbf` | $\textbf{ABC\ abc\ 123}$ |
| `mathit` | $\mathit{ABC\ abc\ 123}$ | `textit` | $\textit{ABC\ abc\ 123}$ |
| `mathtt` | $\mathtt{ABC\ abc\ 123}$ | `texttt` | $\texttt{ABC\ abc\ 123}$ |
| `mathfrak` | $\mathfrak{ABC\ abc\ 123}$ | `frak` | $\frak{ABC\ abc\ 123}$ |
| `mathscr` | $\mathscr{ABC\ abc\ 123}$ | `scr` | $\scr{ABC\ abc\ 123}$ |
| `mathcal` | $\mathcal{ABC\ abc\ 123}$ | `cal` | $\cal{ABC\ abc\ 123}$ |
| `mathbb` | $\mathbb{ABC\ abc\ 123}$ | `Bbb` | $\Bbb{ABC\ abc\ 123}$ |

> __ADDITIONALLY__:  
> `text` may be used instead of `textnormal`

## Decoration

```
\DECORATION{text}
```

| Decoration | Preview |
|--|--|
| `boldsymbol` | $\boldsymbol{ABC\ abc}$ |
| `pmb` | $\pmb{ABC\ abc}$ |
| `underline` | $\underline{ABC\ abc}$ |
| `overline` | $\overline{ABC\ abc}$ |

> __ADDITIONALLY__:  
> `\textnormal` and `\mathnormal` can be used within some decorations (e.g., `boldsymbol`) to remove its effects

### Dashed Line

To get a dashed line a trick with matrix must be used:

```
\begin{matrix}
abc 
\\
\hdashline
\ 
\end{matrix}
```

$$
\begin{matrix}
abc
\\
\hdashline
\ 
\end{matrix}
$$

```
\begin{matrix}
\ 
\\
\hdashline
abc
\end{matrix}
```

$$
\begin{matrix}
\ 
\\
\hdashline
abc
\end{matrix}
$$

> There is a space after each standalone __\\__ (`\ `).

## Font Size

```
{\SIZE text}
```

| Size | Preview |
|--|--|
| `scriptsize` | ${\scriptsize ABC\ abc}$ |
| `tiny` | ${\tiny ABC\ abc}$ |
| `Tiny` | ${\Tiny ABC\ abc}$ |
| `small` | ${\small ABC\ abc}$ |
| `normalsize` | ${\normalsize ABC\ abc}$ |
| normal size | $ABC\ abc$ |
| `large` | ${\large ABC\ abc}$ |
| `Large` | ${\Large ABC\ abc}$ |
| `LARGE` | ${\LARGE ABC\ abc}$ |
| `huge` | ${\huge ABC\ abc}$ |
| `Huge` | ${\Huge ABC\ abc}$ |

## Crossing Out

```
\CROSSING{text}
```

| Crossing | Preview |
|--|--|
| `cancel` | $\cancel{abc}$ |
| `bcancel` | $\bcancel{abc}$ |
| `xcancel` | $\xcancel{abc}$ |

> __ADDITIONALLY__:  
> `\cancelto{abc}{def}` produces $\cancelto{abc}{def}$
