---
{"dg-publish":true,"permalink":"/uni/primo-anno/analisi-1/funzioni/definizioni/def-polinomio-taylor/","tags":["math","uni"]}
---

sia $f$ [[uni/primo anno/analisi 1/funzioni/definizioni/def-derivata#derivabilità\|derivabile]] $n$ volte in $x_0$, definiamo **polinomio di Taylor** di ordine $n$ centrato in $x_0$ i polinomio di grado $\le n$ :
$$P(x) = \sum_{k=0}^n \frac{f^{(k)}(x_0)}{k!} * (x-x_0)^k$$
dove :
- la derivata $0-esima$ è la funzione $f$ originale.
- prendiamo $(x-x_0)^0 =1$.
### osservazione base
Questa formula deriva dal fatto che sto tentando creare un polinomio la cui derivata $n-esima$ è uguale alla derivata $n-esima$ della mia funzione. Avrò quindi un polinomio la cui $k-esima$ derivata è uguale alla $k-esima$ derivata della mia funzione originale.
### osservazione 1
Potrebbe anche essere un polinomio degenere e quindi non avere grado $n$.
### osservazione 2
Posso quindi dire che l'[[uni/primo anno/analisi 1/successioni/definizioni/def-asintotico\|asintotico]] è un polinomio di Taylor di grado 1, è la miglior "retta" approssimante della mia funzione originale in un certo punto.
### osservazione importante
A priori la costruzione di questo polinomio non mi dona nessuna informazione riguardo la funzione $f$ originale, senza il [[uni/primo anno/analisi 1/funzioni/teoremi/teoremi Taylor/teorema-Taylor-Peano-TBF\|teorema-Taylor-Peano-TBF]] non so se sto migliorando la mia approssimazione rispetto a un [[uni/primo anno/analisi 1/successioni/definizioni/def-asintotico\|asintotico]]. Logicamente ha senso però dire che sto "imitando" più accuratamente la funzione in $x_0$ poiché non solo $f$ e $P$ hanno lo stesso valore in $x_0$ ma anche la stessa derivata $k-esima$.