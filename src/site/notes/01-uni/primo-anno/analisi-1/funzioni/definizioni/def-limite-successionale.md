---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/analisi-1/funzioni/definizioni/def-limite-successionale/","tags":["math","uni"],"updated":"2026-02-24T15:52:00.481+01:00"}
---

diciamo che $f$ ammette limite successionale $=l \in \overline{\mathbb{R}}$ per $x \rightarrow x_0$ se vale la seguente cosa:  
$$\forall a_n \in D(f) :  a_n \ne x_0 \ \land a_n\rightarrow x_0 \implies f(a_n) \rightarrow l$$
$$s\lim_{x\rightarrow x_0} f(x)$$
Equivale a dire che per tutte le successioni appartenenti al dominio della funzione che convergono a $x_0$ si ha che $f(x_0) \rightarrow l$. Questa notazione diventa subito ridondante nel momento in cui dimostri che questa notazione e la notazione di [[01-uni/primo-anno/analisi-1/funzioni/definizioni/def-limite-funzione\|limite per funzioni]] è equivalente :
$$\lim_{x \to x_0} f(x) \iff \lim_{n \to \infty} f(a_n) \text{ dove } a_n \to x_0$$
Di conseguenza se sai fare i limiti con le successioni sai automaticamente fare i limiti di funzioni, poiché rimpiazzi la tua $x\rightarrow x_0$ con una $a_n \rightarrow x_0$ che quindi diventa un semplice limite di successione $f(a_n)$ ([[01-uni/primo-anno/analisi-1/basi-funzioni/teoremi/teorema-ponte\|teorema-ponte]]).
