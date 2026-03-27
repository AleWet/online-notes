---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/analisi-1/successioni/teoremi/teorema-del-confronto/","tags":["math","uni"],"updated":"2026-01-05T09:25:10.885+01:00"}
---

### primo teorema del confronto
siano $a_n \le c_n \le b_n : \lim a_n = \lim b_n = l \in \mathbb{R} \implies \lim c_n = l$.
Questa relazione è sufficiente che sia valida *definitivamente*
### secondo teorema del confronto
- $a_n \le b_n \ \land a_n \rightarrow +\infty \implies b_n \rightarrow +\infty$
- $a_n \le b_n \ \land b_n \rightarrow -\infty \implies b_n \rightarrow -\infty$
### corollario-infinitesima-per-limitata-è-infinitesima
se $a_n$ è una [[01-uni/primo-anno/analisi-1/successioni/definizioni/def-successione-infinitesima\|successione infinitesima]] allora :
$$b_n:=a_n * \mathcal{E}_n \text{ è infinitesima}$$
### ==dim 1 / 2==
sia $a_n\le c_n \le b_n$ definitivamente e dove $a_n,b_n\rightarrow l \in  \overline{\mathbb{R}}$
$$\forall \epsilon>0 \exists n_0:\forall n\ge n_0$$
$$l-\epsilon<a_n\le c_n \le b_n < l+\epsilon$$
$$\implies l-\epsilon<c_n<l+\epsilon$$
$$\implies c_n\rightarrow l \ \ \ \square$$
