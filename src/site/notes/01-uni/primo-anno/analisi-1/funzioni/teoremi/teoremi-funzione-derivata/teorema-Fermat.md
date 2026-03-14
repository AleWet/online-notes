---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/analisi-1/funzioni/teoremi/teoremi-funzione-derivata/teorema-fermat/","tags":["math","uni"],"updated":"2026-02-24T15:52:00.482+01:00"}
---

sia $f:(a,b) \to \mathbb{R}$ e sia $x_0 \in (a,b)$ un estremante locale, se $f$ è [[01-uni/primo-anno/analisi-1/funzioni/definizioni/def-derivata#derivabilità\|derivabile]] in $x_0$
$$\implies f'(x_0) = 0$$
### osservazione
il teorema di *Fermat* ti dice dove cercare i punti di massimo e di minimo ma non è una condizione necessaria e sufficiente ma solo necessaria, di conseguenza devi controllare che i punti con $f'(x_0) = 0$ siano effettivamente degli estremanti.
### dim
se $f$ è un massimo locale si ha che 
1) $R(f,x_0,h) \le0 \text{ se } h>0$
2) $R(f,x_0,h) \ge0 \text{ se } h<0$
dove $R(f,x_0,h)$ è il [[01-uni/primo-anno/analisi-1/funzioni/definizioni/def-derivata#rapporto incrementale\|rapporto incrementale]] di $f$.
da questa relazione si ha che :
$$0 \le \lim_{h \to 0^-}R(f,x_0,h)$$
$$0 \ge \lim_{h \to 0^+}R(f,x_0,h)$$
per il [[01-uni/primo-anno/analisi-1/successioni/teoremi/teorema-della-permanenza-del-segno\|teorema-della-permanenza-del-segno]]
$$\implies \lim_{h\to 0}R(f,x_0,h) = 0$$
la dimostrazione per un minimo locale è del tutto analoga.
