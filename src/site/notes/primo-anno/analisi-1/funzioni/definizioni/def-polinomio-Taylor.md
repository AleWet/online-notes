---
{"dg-publish":true,"permalink":"/primo-anno/analisi-1/funzioni/definizioni/def-polinomio-taylor/","tags":["math","uni"],"updated":"2026-02-24T15:52:00.481+01:00"}
---

sia $f$ [[primo-anno/analisi-1/funzioni/definizioni/def-derivata#derivabilità\|derivabile]] $n$ volte in $x_0$, definiamo **polinomio di Taylor** di ordine $n$ centrato in $x_0$ i polinomio di grado $\le n$ :
$$P(x) = \sum_{k=0}^n \frac{f^{(k)}(x_0)}{k!} (x-x_0)^k$$
dove :
- la derivata $0-esima$ è la funzione $f$ originale.
- prendiamo $(x-x_0)^0 =1$.
### lista polinomi di Taylor 
guarda [[PDF-Sviluppi-Taylor.pdf|qui]] per gli sviluppi di Taylor notevoli del Pata, il file originale lo trovi su Webeep.
### osservazione base
Questa formula deriva dal fatto che sto tentando creare un polinomio la cui derivata $n-esima$ è uguale alla derivata $n-esima$ della mia funzione. Avrò quindi un polinomio la cui $k-esima$ derivata è uguale alla $k-esima$ derivata della mia funzione originale.
### osservazione 1
Potrebbe anche essere un polinomio degenere e quindi non avere grado $n$.
### osservazione 2
Posso quindi dire che l'[[primo-anno/analisi-1/successioni/definizioni/def-asintotico\|asintotico]] è un polinomio di Taylor di grado 1, è la miglior "retta" approssimante della mia funzione originale in un certo punto.
### osservazione importante
A priori la costruzione di questo polinomio non mi dona nessuna informazione riguardo la funzione $f$ originale, senza il [[primo-anno/analisi-1/funzioni/teoremi/teoremi-Taylor/teorema-Taylor-Peano\|teorema-Taylor-Peano]]. Logicamente ha senso però dire che sto "imitando" più accuratamente la funzione in $x_0$ poiché non solo $f$ e $P$ hanno lo stesso valore in $x_0$ ma anche la stessa derivata $k-esima$.
### osservazione extra
Si dimostra che una funzione pari nel suo sviluppo di Taylor ha solo termini pari (per le funzioni dispari è analogo). Il ragionamento per dimostrare questo è notare che la derivata di una funzione pari è sempre dispari, se prendi $x_{0} = 0\ \  (*)$  avrai che le derivate $f^{(2n+1)}$ sono tutte dispari e una funzione dispari definita in $u(0)$ si annulla in 0 :
$$f^{(2n+1)}(0) = -f^{(2n+1)}(-0) = -f^{(2n+1)}(0) \implies f^{(2n+1)}(0) = 0$$
importante notare che questo vale anche per le funzioni definite solo in 0 quindi anche se $f^{(2n+1)}$ non è continua né definita in un $u(0)$.

$(*$ cosa che penso sia necessaria quando si parla di funzioni dispari / dispari perché se no non ha senso parlarne, se hai una funzione definita solo su $(0,+\infty)$ essa non può essere dispari né pari) 