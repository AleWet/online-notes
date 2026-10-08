---
{"dg-publish":true,"permalink":"/primo-anno/analisi-1/funzioni/teoremi/teoremi-integrali-riemann/teorema-media-integrale/","tags":["math","uni"],"updated":"2026-02-24T15:52:00.484+01:00"}
---

sia $f \in R_{P}(a,b)$ (guarda [[primo-anno/analisi-1/funzioni/definizioni/def-primitiva#notazione interna al corso\|qui]]) allora 
$$\exists c \in (a,b) : \ \frac{1}{b-a} \int_{a}^b f(x)dx = f(c)$$
in pratica stai dicendo che $\exists$ un punto $c$ nell'intervallo $(a,b)$ dove se fai $f(c)(b-a)$ ottieni il tuo integrale $\int_{a}^b f(x)dx$, esiste sempre un punto da cui puoi costruire un rettangolo che ha la stessa area sotto la funzione integranda.
### dim 
sia $F$ una primitiva di $f$, applico [[primo-anno/analisi-1/funzioni/teoremi/teoremi-funzione-derivata/teorema-Lagrange-(tbf)\|Lagrange]] su $[a,b]$  su $F$ (so che $F$ è derivabile per definizione di primitiva) :
$$\exists c \in (a,b) : F'(c) (b-a)= F(b)-F(a)$$
$$\implies f(c)(b-a) = F(b)-F(a)$$
qui usi banalmente il [[primo-anno/analisi-1/funzioni/teoremi/teoremi-integrali-Riemann/teorema-fondamentale-del-calcolo\|teorema-fondamentale-del-calcolo]] e trovi che
$$f(c)(b-a) = \int_{a}^b f(x)dx  $$

