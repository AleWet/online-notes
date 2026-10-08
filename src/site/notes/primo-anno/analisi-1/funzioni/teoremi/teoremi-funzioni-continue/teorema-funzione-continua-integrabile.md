---
{"dg-publish":true,"permalink":"/primo-anno/analisi-1/funzioni/teoremi/teoremi-funzioni-continue/teorema-funzione-continua-integrabile/","tags":["math","uni"],"updated":"2026-02-24T15:52:00.483+01:00"}
---

sia  $f : [a,b] \to \mathbb{R}$ con $f$ [[primo-anno/analisi-1/funzioni/definizioni/def-continuità\|continua]] allora $f \in R(a,b)$ (dove con $R(a,b)$ intendo [[primo-anno/analisi-1/funzioni/definizioni/def-integrale-Riemann\|questo]]).
### dim
grazie al [[primo-anno/analisi-1/funzioni/definizioni/def-uniformemente-continua\|teorema di Heine-Cantor]] :
$$\implies \forall \varepsilon > 0 \exists  \ \delta >0 : \text{ se } |x-y| < \delta \implies |f(x)-f(y)| < \varepsilon$$
voglio mostrare che fissato $\varepsilon>0 \ \exists n_{0} : \text{ se } n \geq n_{0} \implies \omega(f) < \varepsilon$ (guarda [[primo-anno/analisi-1/funzioni/definizioni/def-integrale-Riemann#def $ Delta$ somme sup e inf\|qui]] per def. di $\omega(f)$).
sia $\varepsilon >0$ fissato e sia $n_0$ tale che 
$$\frac{b-a}{n} < \delta \ \forall n \geq n_{0}$$
se suddivido $[a,b]$ in $n$ intervalli (che chiamo $I_{k}$) avrò che:
$$l(I_{k}) = \frac{b-a}{n} < \delta$$
dove con $l(I)$ intendo la [[primo-anno/analisi-1/basi-funzioni/definizioni/def-intervallo#lunghezza dell'intervallo\|lunghezza dell'intervallo]] e adesso uso il fatto che $f$ è uniformemente continua:
$$\forall x,y \in I_{k}, |f(x)-f(y)| < \varepsilon$$
$$\implies \sup_{I_{k}}f - \inf_{I_{k}}f < \varepsilon$$
$$\implies \omega(f) = \frac{b-a}{n}\sum_{k=1}^n \sup_{I_{k}}f - \inf_{I_{k}}f \leq \frac{b-a}{n} \sum_{k=1}^n\varepsilon = \varepsilon \frac{n(b-a)}{n} = \varepsilon(b-a)$$
$$\implies \omega(f) \to 0 \text{ poiché } (b-a)\varepsilon \to 0 \text{ if } \varepsilon \to 0$$