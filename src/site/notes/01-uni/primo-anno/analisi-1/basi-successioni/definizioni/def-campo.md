---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/analisi-1/basi-successioni/definizioni/def-campo/","tags":["math","uni"]}
---

un campo $F$ è definito come un insieme con 2 [[01-uni/primo-anno/analisi-1/basi-successioni/definizioni/def-operazione-binaria\|operazioni binarie]] tali che:
- $(F, +)$ è un [[01-uni/primo-anno/analisi-1/basi-successioni/definizioni/def-gruppo\|gruppo abeliano]] con identità $n_0 = 0$
- $(F \ \textbackslash\ \{0\}, *)$ è un [[01-uni/primo-anno/analisi-1/basi-successioni/definizioni/def-gruppo\|gruppo abeliano]] con identità $n_1 = 1 \ne n_0$
- e con la proprietà distributiva : $\forall a,b,c \in F \ a*(b+c) = a*b+a*c$

con questa definizione, $\mathbb{R}, \mathbb{C}, \mathbb{Q}$ sono campi
___
### campo ordinato
sia $(\mathbb{K},+,*)$ un campo, se esiste una [[01-uni/primo-anno/analisi-1/basi-successioni/definizioni/def-relazione-d'ordine\|relazione d'ordine totale]] su $\mathbb{K}$ tale che :
- $a\le b \implies a +c \le b +c$
- $a\le b \implies a*c\le b*c$
allora si dice che la relazione d'ordine è compatibile con il campo ed è quindi un campo ordinato.
$\mathbb{R}, \mathbb{Q}$ sono campi ordinati, $\mathbb{C}$ non è un campo : 
##### dimostrazione che C non è un campo ordinato:
si dimostra che $\forall x, 0 \le x*x \implies 0 \le i*i \implies 0 \le -1 \implies 1 \le 0$ ma sappiamo che $0\le1$ di conseguenza l'unica opzione è che $0=1$ ma questo è contro le ipotesi di campo (elementi neutri diversi).
