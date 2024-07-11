# Set-Builder Notation: Quantifiers

- $\forall n \in S$ - the universal quantifier that reads _"for all"_
- $\exists n \in S$ - the existential quantifier that reads _"exists such"_

## Overview

> In the expressions below the following hold:
> - ${\tt T}(x,k)$ is a predicate
> - ${\tt G}(x,k)$ is a generator of the value

- every term ${\color{blue}x}$ from ${\Bbb S}_1$ for which there is term ${\color{red}k}$ from ${\Bbb S}_2$ such that ${\tt T}({\color{blue}x},{\color{red}k})$ returns _true_

$$
\\{\ {\color{blue}x} \in {\Bbb S}_1: (\exists {\color{red}k} \in {\Bbb S}_2)({\tt T}({\color{blue}x},{\color{red}k})) \ \\}
$$

$$
\\{\ {\color{blue}x} \in {\Bbb S}_1: (\exists {\color{red}k} \in {\Bbb S}_2)({\tt T}({\color{blue}x},{\color{red}k}) \implies {\color{blue}x}={\tt G}({\color{blue}x},{\color{red}k})) \ \\}
$$

- every term ${\color{blue}x}$ from ${\Bbb S}_1$ for which all terms ${\color{red}k}$'s of ${\Bbb S}_2$ satisfy ${\tt T}({\color{blue}x},{\color{red}k})$

$$
\\{\ {\color{blue}x} \in {\Bbb S}_1: (\forall {\color{red}k} \in {\Bbb S}_2)({\tt T}({\color{blue}x},{\color{red}k})) \ \\}
$$

$$
\\{\ {\color{blue}x} \in {\Bbb S}_1: (\forall {\color{red}k} \in {\Bbb S}_2)({\tt T}({\color{blue}x},{\color{red}k}) \implies {\color{blue}x}={\tt G}({\color{blue}x},{\color{red}k})) \ \\}
$$

> membership must be specified for a term bound to a quantifier: e.g., $\exists n \in \mathbb{N}$ is proper, while $\exists n$ not

## Examples

- **prime numbers**: every natural number ${\color{blue}p}$ which can be divided by itself, 1 and nothing else

$$
\left\\{\ {\color{blue}p} \in \mathbb{N} \ \|\ \forall({\color{red}k} \in \mathbb{N} \setminus \\{1,{\color{blue}p}\\})\left(\frac{{\color{blue}p}}{{\color{red}k}} \notin \mathbb{Z}\right) \ \right\\}
$$

- **concentrated points**: every point ${\color{blue}p}$ from ${\Bbb M}$ that has a neighbor ${\color{red}q}$ at a distance $\Delta$ or less

$$
\\{\ 
{\color{blue}p} \in \Bbb{R}^2:
{\color{blue}p} \subset {\Bbb M} \land
(\exists {\color{red}q} \in \Bbb{R}^2)(
{\color{red}q} \subset {\Bbb M}\setminus\\{{\color{blue}p}\\} \land
{\tt D}({\color{blue}p},{\color{red}q})
)
\ \\}
$$

$$
{\tt D}(p,q) =
(p_1-q_1)^2+(p_2-q_2)^2 \leq \Delta^2
$$

### Complex Quantifier

- **permutations**: every permutation $\color{blue}p$ ($\Bbb{R}^n$) that consists of all necessary terms without repetition, i.e., terms of $\Bbb{T}$ in all possible arrangements

$$
\begin{array}{ll}
\\{\ {\color{blue}p} \in \Bbb{R}^n \ \|
\\
\quad (\forall {\color{red}i},{\color{orange}j} \in [1,n], {\color{red}i} \neq {\color{orange}j})
({\color{blue}p}\_{\color{red}i} \neq {\color{blue}p}\_{\color{orange}j})
\\
\quad\quad \land
\\
\quad (\forall {\color{red}i} \in [1,n])({\color{blue}p}_{\color{red}i} \in \Bbb{T})
\\
\ \\}
\end{array}
$$


