---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/analisi-1/funzioni/teoremi/teoremi-integrali-riemann/teorema-funzione-integrale-continua/","tags":["math","uni"],"updated":"2026-02-24T15:52:00.484+01:00"}
---

sia $f:[a,b] \to \mathbb{R}$ t.c. $f \in R(a,b)$ (guarda [[01-uni/primo-anno/analisi-1/funzioni/definizioni/def-integrale-Riemann#Riemann integrabile\|qui]]) e sia $I(x)$ la [[01-uni/primo-anno/analisi-1/funzioni/definizioni/def-funzione-integrale\|funzione integrale]] di $f$, allora $I(x)$ è [[01-uni/primo-anno/analisi-1/funzioni/definizioni/def-continuità\|continua]]. 
### osservazione
$F$ non è solo continua ma **Lipschitz** continua, questo è un concetto che il Pata ha citato e non è necessario ma una funzione Lipschitz continua non solo è continua ma si ha che:
$$\forall x,y \in [a,b] \ \  \ \exists L \ge 0 \ , \ L \in \mathbb{R}\ \   :\ \  |f(x)-f(y)| \le L|x-y|$$
che equivale a dire che in ogni punto la tua funzione se è derivabile la sua derivata è finita. Questa è una condizione ancora più forte della [[01-uni/primo-anno/analisi-1/funzioni/definizioni/def-uniformemente-continua\|continuità uniforme]].
### dim
analizzo la seguente quantità con $x,y \in [a,b]$ :
$$|I(x)-I(y)| = \left| \int_{x}^y f(t)dt\right|$$
qui uso [[01-uni/primo-anno/analisi-1/funzioni/teoremi/teoremi-integrali-Riemann/teorema-disuguaglianza-modulo\|teorema-disuguaglianza-modulo]] :
$$\leq \int_{x}^y |f(t)|dt \leq |x-y|\sup_{[x,y]}|f| $$
naturalmente l'area sotto la funzione è $\leq$ del rettangolo formato dal suo $\sup$ con la stessa base. Allora ottengo che $\forall x,y \in [a,b]$ :
$$|I(x)-I(y)| \leq |x-y| \sup_{[x,y]}|f|$$
poiché $f \in R(a,b)$ so che $f$ è limitata, allora se $|x-y|$ è arbitrario se lo moltiplico per il $\sup$ è ancora arbitrario (poiché quest'ultimo è finito), di conseguenza la distanza tra le immagini è arbitraria:
$$|I(x)-I(y)| \leq L|x-y|, \ \ \ L \in \mathbb{R} \ \ \  \square $$



