---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/analisi-1/funzioni/teoremi/teoremi-integrali-riemann/teorema-confronto-integrali-tbf/","tags":["math","uni"]}
---

siano $f,g \in R(a,b)$ (dove con $R(a,b)$ si intende [[01-uni/primo-anno/analisi-1/funzioni/definizioni/def-integrale-Riemann\|questo]]) allora:
$$\text{se } f(x) \ge g(x) \ \forall x \in [a,b]$$
$$\implies \int f(x)dx \ge \int g(x)dx$$
### corollario
se ho che $f(x) \ge 0 \ \forall x \in [a,b]$ allora 
$$ \int_{a}^b f(x)dx \ge 0$$
### osservazione importante
non è vero che 
$$\int_{a}^b f(x)dx = 0 \implies f(x) = 0  \forall x \in [a,b]$$
poiché posso cambiare un numero $finito$ di punti e l'integrale rimane [[01-uni/primo-anno/analisi-1/funzioni/teoremi/teoremi-integrali-Riemann/teorema-integrale-finiti-punti-diversi-(tbf)\|lo stesso integrale alla fine]].
se impongo però che $f$ sia [[01-uni/primo-anno/analisi-1/funzioni/definizioni/def-continuità\|continua]] allora effettivamente la funzione è nulla (non posso più avere punti di "salto" dove l'integrale ha valori diversi che hanno "misura $0$"), la dimostrazione l'ha data il Pata in classe e se ho voglia sarà riportata qui sotto.
### dim teorema
per dimostrare basta notare che :
$$s_{n}(f)\geq s_{n}(g) \ \forall x \in [a,b]$$
$$\text{ se } s_{n}(f) \to \int_{a}^b f(x)dx \ \ \text{e} \ \ s_{n}(g) \to \int_{a}^b g(x)fx$$
uso il [[01-uni/primo-anno/analisi-1/successioni/teoremi/teorema-della-permanenza-del-segno\|teorema-della-permanenza-del-segno]] e ho finito.
### dim corollario
basta che metti $g(x) = 0$ e trovi la tesi.
### dim corollario continua (tbd)

