---
{"dg-publish":true,"permalink":"/uni/primo-anno/analisi-1/successioni/teoremi/teorema-cuoricino/","tags":["uni","math"]}
---

siano $a_n$ e $b_n$ tali che:
- $a_n \downarrow \land \ b_n\uparrow$
- $a_n \ge b_n \forall n$
- $a_n - b_n \rightarrow0$
allora $\lim a_n = \lim b_n = l \in \mathbb{R}$
### ==dim==
$a_n , b_n$ sono successioni monotone limitate : $b_0\le b_n \le a_n \le a_0 \forall n \implies$ convergono in $\mathbb{R}$
([[uni/primo anno/analisi 1/successioni/teoremi/teorema-monotona-allora-regolare\|monotona e limitata allora converge]]) : $a_n \rightarrow \gamma, b_n \rightarrow l$.
prendo in considerazione :
$$|l-\gamma|$$
$$|l-\epsilon| = |l-b_n+b_n-a_n+a_n-\gamma| \le|a_n-b_n|+|b_n-l|+|a_n-\gamma|$$
$$\forall\epsilon>0 \ \exists n_0 :\forall n\ge n_0 \ \ \ \ |a_n-\gamma|<\epsilon$$
$$...$$

$$\forall \epsilon >0 \ \forall n\ge \max{(n_0, n_1, n_2)} \ \ |a_n-\gamma| + |b_n+l|+|a_n-b_n| < 3\epsilon$$
$$\implies|l-\gamma|\le3\epsilon\implies l = \gamma \ \ \ \ \ \ \ \ \square $$
