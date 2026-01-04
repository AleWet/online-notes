---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/analisi-1/funzioni/definizioni/def-darboux/","tags":["math","uni"]}
---

una funzione $f:I \to \mathbb{R}$ ,dove $I$ è un [[01-uni/primo anno/analisi 1/basi funzioni/definizioni/def-intervallo\|intervallo]], è di Darboux se presi $x,y \in I : x<y$, la funzione $f$ assume tutti i valori compresi tra $f(x)$ e $f(y)$ nell'intervallo $[x,y]$ : 
$$\forall x,y \in I, \forall w  \in [f(x),f(y)], \exists c \in [x,y] : f(c) = w$$
(nota : può anche essere $[f(y),f(x)]$ dipende da chi è maggiore o minore).
### osservazione 1
$f:I\to \mathbb{R}$ è di Darboux $\implies$ preso un qualsiasi i intervallo $J \subseteq I$ si ha che $f(J)$ è un intervallo.
### osservazione 2
se $f$ ha la proprietà di Darboux $\not\Rightarrow$ $f$ è [[01-uni/primo-anno/analisi-1/funzioni/definizioni/def-continuità\|continua]], un esempio è :
$$f(x) = \cases{sin\left( \frac{1}{x} \right)\ \ \ x \ne 0  \\ \\ 0 \ \ \ \ \ \ \ \ \ \ \ \ \ \ x = 0}$$
che ha una [[01-uni/primo-anno/analisi-1/funzioni/definizioni/def-punti-discontinuità#discontinuità di II specie\|discontinuità di seconda specie]] in $x = 0$.
### osservazione 3
se $f  :I \to \mathbb{R}$ è di Darboux **non può avere**
- [[01-uni/primo-anno/analisi-1/funzioni/definizioni/def-punti-discontinuità#discontinuità eliminabile (III specie)\|discontinuità eliminabili]]
- [[01-uni/primo-anno/analisi-1/funzioni/definizioni/def-punti-discontinuità#discontinuità di tipo salto (I specie)\|discontinuità di tipo salto]]
