---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/analisi-1/funzioni/teoremi/teoremi-funzioni-continue/teorema-weierstrass-darboux/","tags":["math","uni"]}
---

### tesi
se $f:[a,b] \to \mathbb{R}$ è [[01-uni/primo anno/analisi 1/funzioni/definizioni/def-continuità\|continua]] $\implies f([a,b]) = [m, M]$ dove $m = \min, M = \max$.
### dim
banalmente se $f:[a,b] \to \mathbb{R}$ è continua $\implies f$ è di Darboux (guarda [[01-uni/primo-anno/analisi-1/funzioni/teoremi/teoremi-funzioni-continue/teorema-Darboux\|teorema-Darboux]]), con le stesse ipotesi puoi dire che $f$ ammette $\max$ e $\min$ in $[a,b]$ dal [[01-uni/primo-anno/analisi-1/funzioni/teoremi/teoremi-funzioni-continue/teorema-Weierstrass\|teorema-Weierstrass]]
$$\forall x \in [a,b], f(x) \in [m,M]$$
siano $x_m$ e $x_M$ tali che $f(x_m) = m$ e $f(x_M) = M$ con naturalmente $x_m,x_M \in [a,b]$ 
$$\implies \forall w \in [f(x_m),f(x_M)] \ \exists z \in [x_m, x_M] : f(z) = w$$
$$[x_m,x_M]\subseteq[a,b]$$
$$\implies \forall w \in[m,M] \ \exists z \in [a,b] : f(z) = w \ \ \square$$
