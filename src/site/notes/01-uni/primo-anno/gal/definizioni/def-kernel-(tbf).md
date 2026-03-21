---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/gal/definizioni/def-kernel-tbf/","tags":["math","uni"],"updated":"2026-03-15T11:27:45.289+01:00"}
---

Sia $L:V \to W$ una [[01-uni/primo-anno/gal/definizioni/def-funzione-lineare\|funzione lineare]] chiamo $Kern(L)$ l'insieme dei vettori di $V$ che vengono mappati nell'origine di $W$ :
$$Kern(L) := \{  \underline{v} \in V : L( \underline{v}) = \underline{0} \}$$
Detto in altri termini è l'insieme delle soluzioni de sistema $omogeneo$ (metti $\underline{b} =  \underline{0}$) associato :
$$Kern(L)\iff Sol(L \underline{v} = \underline{0})$$
___
### sotto spazio vettoriale
Il nucleo di una funzione lineare è un [[01-uni/primo-anno/gal/definizioni/def-sotto-spazio-vettoriale-(tbf)\|sottospazio vettoriale]] dello [[01-uni/primo-anno/gal/definizioni/def-spazio-vettoriale\|spazio]] $V$ di partenza, per controllarlo basta usare il [[01-uni/primo-anno/gal/definizioni/def-sotto-spazio-vettoriale-(tbf)#teorema controllo s.s.v\|seguente teorema]] sul sottospazio :
1) $Lv = \underline{0}$ è sempre risolubile $\iff Ker(L) \ne \emptyset$
2) la somma di soluzioni del sistema omogeneo è soluzione
3) ogni multiplo di una soluzione è soluzione
### dims
1) $L \underline{0} = \underline{0} \implies Ker(L) \ne \emptyset$
2) $Lh_{1} =Lh_{2} = \underline{0}  \implies L(h_{1}+h_{2})=  Lh_{1}+Lh_{2} = \underline{0}+  \underline{0} = \underline{0}$ 
3) $c \in \mathbb{N}, \ Lh = \underline{0} \implies L(ch) = c(Lh) = c \underline{0} = \underline{0}$
usando solo le proprietà di funzione lineare
____
### todo
in pratica $Kern(L)$ o $Kern(A)$ ti dice come sono distribuite le soluzioni delle equazioni del tipo:
$$L( \underline{x}) = \underline{b}$$
