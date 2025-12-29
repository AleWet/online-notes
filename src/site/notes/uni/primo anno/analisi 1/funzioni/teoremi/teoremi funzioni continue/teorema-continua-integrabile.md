---
{"dg-publish":true,"permalink":"/uni/primo-anno/analisi-1/funzioni/teoremi/teoremi-funzioni-continue/teorema-continua-integrabile/","tags":["math","uni"]}
---

sia $f$ [[uni/primo anno/analisi 1/funzioni/definizioni/def-continuità\|continua]] in un intervallo $[a,b]$ allora $f \in R(a,b)$ (dove con $R(a,b)$ si intende [[uni/primo anno/analisi 1/funzioni/definizioni/def-integrale-Riemann-TBF\|questo]]).
### dim
grazie al [[uni/primo anno/analisi 1/funzioni/teoremi/teoremi funzioni continue/teorema-Heine-Cantor\|teorema-Heine-Cantor]] sappiamo che $f$ è [[uni/primo anno/analisi 1/funzioni/definizioni/def-uniformemente-continua\|uniformemente continua]] :
$$\implies \forall \varepsilon > 0 \exists  \ \delta >0 : \text{ se } |x-y| < \delta \implies |f(x)-f(y)| < \varepsilon$$
voglio mostrare che fissato $\varepsilon>0 \ \exists n_{0} : \text{ se } n \geq n_{0} \implies \omega(f) < \varepsilon$ (guarda [[uni/primo anno/analisi 1/funzioni/definizioni/def-integrale-Riemann-TBF#def $ Delta$ somme sup e inf\|qui]] per def. di $\omega(f)$).
sia $\varepsilon >0$ fissato e sia $n_0$ tale che 
$$\frac{b-a}{n} < \delta \ \forall n \geq n_{0}$$
se suddivido $[a,b]$ in $n$ intervalli (che chiamo $I_{k}$) avrò che:
$$l(I_{k}) = \frac{b-a}{n} < \delta$$
dove con $l(I)$ intendo la [[uni/primo anno/analisi 1/basi funzioni/definizioni/def-intervallo#lunghezza dell'intervallo\|lunghezza dell'intervallo]] e adesso uso il fatto che $f$ è uniformemente continua:
$$\forall x,y \in I_{k}, |f(x)-f(y)| < \varepsilon$$
$$\implies \sup_{I_{k}}f - \inf_{I_{k}}f < \varepsilon$$
$$\implies \omega(f) = \frac{b-a}{n}\sum_{k=1}^n \sup_{I_{k}}f - \inf_{I_{k}}f \leq \frac{b-a}{n} \sum_{k=1}^n\varepsilon = \varepsilon \frac{n(b-a)}{n} = \varepsilon(b-a)$$
$$\implies \omega(f) \to 0 \text{ poiché } (b-a)\varepsilon \to 0 \text{ if } \varepsilon \to 0$$