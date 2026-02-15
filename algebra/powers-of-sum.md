# The Powers of a Sum

$$
\left(
\sum_{i=1}^n a_i
\right)^p =
\sum_{j_1=1}^n \sum_{j_2=1}^n
\cdots
\sum_{j_p=1}^n
\prod_{k=1}^p a_{j_k}
$$

For example:

$$
\begin{array}{ll}
(a+b)^2 & = \displaystyle \sum_{j_1=1}^2 \sum_{j_2=1}^2 j_1 j_2
\\
& = a \cdot a + a \cdot b + b \cdot a + b \cdot b
\\
& = a^2 + ab + ba + b^2
\\
& = a^2 + b^2 + 2ab
\end{array}
$$

$$
\begin{array}{ll}
(a+b+c)^2 & = \displaystyle \sum_{j_1=1}^3 \sum_{j_2=1}^3 j_1 j_2
\\
& = a \cdot a + a \cdot b + a \cdot c + b \cdot a + b \cdot b + b \cdot c + c \cdot a + c \cdot b + c \cdot c
\\
& = a^2 + ab + ac + ba + b^2 + bc + ca + cb + c^2
\\
& = a^2 + b^2 + c^2 + 2ab + 2ac + 2bc
\\
& = a^2 + b^2 + c^2 + 2(ab+ac+bc)
\end{array}
$$

## Power of 2

$$
\begin{array}{l}
(a+b)^2 = a^2 + b^2 + 2ab
\\
\ 
\\
(a+b+c)^2 = a^2 + b^2 + c^2 + 2(
\\
\quad ab+ac+bc
\\
)
\\
\ 
\\
(a+b+c+d)^2 = a^2 + b^2 + c^2 + d^2 + 2(
\\
\quad ab+ac+ad+bc+bd+cd
\\
)
\end{array}
$$

## Power of 3

$$
\begin{array}{l}
(a+b)^3 = a^3 + b^3 + 3(a^2b+ab^2)
\\
\ 
\\
(a+b+c)^3 = a^3 + b^3 + c^3 + 3(
\\
\quad (a+b)ab + (a+c)ac + (b+c)bc
\\
) + 6abc
\\
\ 
\\
(a+b+c+d)^3 = a^3 + b^3 + c^3 + d^3 + 3(
\\
\quad (a+b)ab + (a+c)ac + (a+d)ad \ +
\\
\quad (b+c)bc + (b+d)bd + (c+d)cd
\\
) + 6(abc + abd + acd + bcd)
\end{array}
$$

## Power of 4

$$
\begin{array}{l}
(a+b)^4 = a^4 + b^4 + 4(a^3b+ab^3) + 6(ab)^2
\\
\ 
\\
\ 
\\
(a+b+c)^4 = a^4 + b^4 + c^4 + 4(
\\
\quad ab(a^2+b^2) + ac(a^2+c^2) + bc(b^2+c^2)
\\
) + 6(
\\
\quad (ab)^2+(ac)^2+(bc)^2
\\
) + 12abc(a+b+c)
\\
\ 
\\
\ 
\\
(a+b+c+d)^4 = a^4 + b^4 + c^4 + d^4 + 4(
\\
\quad ab(a^2+b^2) + ac(a^2+c^2) + ad(a^2+d^2) \ +
\\
\quad bc(b^2+c^2) + bd(b^2+d^2) + cd(c^2+d^2)
\\
) + 6(
\\
\quad (ab)^2 + (ac)^2 + (ad)^2 \ +
\\
\quad (bc)^2 + (bd)^2 + (cd)^2
\\
) + 12(
\\
\quad abc(a+b+c) + abd(a+b+d) \ +
\\
\quad acd(a+c+d) + bcd(b+c+d)
\\
) + 24abcd
\end{array}
$$

## Power of 5

$$
\begin{array}{l}
(a+b)^5 = a^5 + b^5 + 5ab(a^3+b^3) + 10(a+b)(ab)^2
\\
\ 
\\
\ 
\\
(a+b+c)^5 = a^5 + b^5 + c^5 + 5(
\\
\quad ab(a^3+b^3) + ac(a^3+c^3) + bc(b^3+c^3)
\\
) + 10(
\\
\quad (a+b)(ab)^2 + (a+c)(ac)^2 + (b+c)(bc)^2
\\
) + 20abc(a^2 + b^2 + c^2) + 30abc(ab+ac+bc)
\\
\ 
\\
\ 
\\
(a+b+c+d)^5 = a^5 + b^5 + c^5 + d^5 + 5(
\\
\quad ab(a^3+b^3) + ac(a^3+b^3) + ad(a^3+b^3) \ +
\\
\quad bc(b^3+c^3) + bd(b^3+d^3) + cd(c^3+d^3)
\\
) + 10(
\\
\quad (a+b)(ab)^2 + (a+c)(ac)^2 + (a+d)(ad)^2 \ +
\\
\quad (b+c)(bc)^2 + (b+d)(bd)^2 + (c+d)(cd)^2
\\
) + 20(
\\
\quad abc(a^2+b^2+c^2) + abd(a^2+b^2+d^2) \ +
\\
\quad acd(a^2+c^2+d^2) + bcd(b^2+c^2+d^2)
\\
) + 30(
\\
\quad abc(ab+ac+bc) + abd(ab+ad+bd) \ +
\\
\quad acd(ac+ad+cd) + bcd(bc+bd+cd)
\\
) + 60abcd(a+b+c+d)
\end{array}
$$

## Power of 6

$$
\begin{array}{l}
(a+b)^6 = a^6 + b^6 + 6ab(a^4+b^4) + 15(a^2+b^2)(ab)^2 + 20(ab)^3
\\
\ 
\\
\ 
\\
(a+b+c)^6 = a^6 + b^6 + c^6 + 6(
\\
\quad ab(a^4+b^4) + ac(a^4+c^4) + bc(b^4+c^4)
\\
) + 15(
\\
\quad (a^2+b^2)(ab)^2 + (a^2+c^2)(ac)^2 + (b^2+c^2)(bc)^2
\\
) + 20(
\\
\quad (ab)^3 + (ac)^3 + (bc)^3
\\
) + 30abc(a^3+b^3+c^3) + 60abc(
\\
\quad (a+b)ab + (a+c)ac + (b+c)bc
\\
) + 90(abc)^2
\\
\ 
\\
\ 
\\
(a+b+c+d)^6 = a^6 + b^6 + c^6 + d^6 + 6(
\\
\quad ab(a^4+b^4) + ac(a^4+c^4) + ad(a^4+d^4) \ +
\\
\quad bc(b^4+c^4) + bd(b^4+d^4) + cd(c^4+d^4)
\\
) + 15(
\\
\quad (a^2+b^2)(ab)^2 + (a^2+c^2)(ac)^2 + (a^2+d^2)(ad)^2 \ +
\\
\quad (b^2+c^2)(bc)^2 + (b^2+d^2)(bd)^2 + (c^2+d^2)(cd)^2
\\
) + 20(
\\
\quad (ab)^3 + (ac)^3 + (ad)^3 + (bc)^3 + (bd)^3 + (cd)^3
\\
) +30(
\\
\quad abc(a^3+b^3+c^3) + abd(a^3+b^3+d^3) \ +
\\
\quad acd(a^3+c^3+d^3) + bcd(b^3+c^3+d^3)
\\
) + 60(
\\
\quad abc(ab(a+b) + ac(a+c) + bc(b+c)) \ +
\\
\quad abd(ab(a+b) + ad(a+d) + bd(b+d)) \ +
\\
\quad acd(ac(a+c) + ad(a+d) + cd(c+d)) \ +
\\
\quad bcd(bc(b+c) + bd(b+d) + cd(c+d))
\\
) + 90(
\\
\quad (abc)^2 + (abd)^2 + (acd)^2 + (bcd)^2
\\
) + 120abcd(a^2+b^2+c^2+d^2) + 180abcd(
\\
\quad ab+ac+ad+bc+bd+cd
\\
)
\end{array}
$$
