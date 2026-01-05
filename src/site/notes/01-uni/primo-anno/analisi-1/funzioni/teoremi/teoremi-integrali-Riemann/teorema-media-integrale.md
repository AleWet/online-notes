---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/analisi-1/funzioni/teoremi/teoremi-integrali-riemann/teorema-media-integrale/","tags":["math","uni"]}
---

sia $f \in R_{P}(a,b)$ (guarda [[01-uni/primo-anno/analisi-1/funzioni/definizioni/def-primitiva#notazione interna al corso\|qui]]) allora 
$$\exists c \in (a,b) : \ \frac{1}{b-a} \int_{a}^b f(x)dx = f(c)$$
in pratica stai dicendo che $\exists$ un punto $c$ nell'intervallo $(a,b)$ dove se fai $f(c)(b-a)$ ottieni il tuo integrale $\int_{a}^b f(x)dx$, esiste sempre un punto da cui puoi costruire un rettangolo che ha la stessa area della funzione integranda.
### dim 
sia $F$ una primitiva di $f$, applico [[01-uni/primo-anno/analisi-1/funzioni/teoremi/teoremi-funzione-derivata/teorema-Lagrange\|Lagrange]] su $[a,b]$  su $F$ (so che $F$ [[01-uni/primo-anno/analisi-1/funzioni/teoremi/teoremi-integrali-Riemann/teorema-funzione-integrale-continua-TBF\|è continua]]) :
$$\exists c \in (a,b) : F'(c) (b-a)= F(b)-F(a)$$
$$\implies f(c)(b-a) = F(b)-F(a)$$
qui usi banalmente il [[01-uni/primo-anno/analisi-1/funzioni/teoremi/teoremi-integrali-Riemann/teorema-fondamentale-del-calcolo\|teorema-fondamentale-del-calcolo]] e trovi che
$$f(c)(b-a) = \int_{a}^b f(x)dx  $$

