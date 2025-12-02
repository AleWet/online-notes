---
{"dg-publish":true,"permalink":"/uni/primo-anno/analisi-1/funzioni/teoremi/teoremi-integrali-riemann/teorema-linearita-integrale-tbf/","tags":["math","uni"]}
---

siano $f,g \in R(a,b)$ (dove con $R(a,b)$ si intende [[uni/primo anno/analisi 1/funzioni/definizioni/def-integrale-Riemann-TBF\|questo]]) allora 
$$\tag{1}f+\lambda g \in R(a,b)$$
$$\tag{2}\int_{a}^b [f(x)+\lambda g(x)] )= \int_{a}^b f(x)dx+\lambda\int_{a}^b g(x)dx$$
### osservazione importante
prima di dimostrare questo teorema è necessaria la seguente osservazione :
siano $f,g:I \to \mathbb{R}$ allora:
$$\sup_{I}(f,g) \le \sup_{I}f+\sup_{I}g$$
$$\inf_{I}(f,g) \ge \inf_{I}f+\inf_{I}g$$
dimostro brevemente:
$$f(x)\le \sup_{I}f, \ \ g(x) \le \sup_{I}g$$
$$\forall x \in I , \ f(x)+g(x) \le \sup_{I}f+\sup_{I}g$$
$$\implies \sup_{I}(f,g) \le \sup_{I}f +\sup_{I}g \ \text{ per la permanenza del segno}$$
### dim TBD
prendo $\lambda = 1$ per comodità, la dimostrazione è analoga con $\lambda$ generico.
Fissato $I_{k}$ :