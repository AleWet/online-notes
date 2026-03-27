---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/gal/definizioni/def-kernel/","tags":["math","uni"],"updated":"2026-03-25T20:19:10.109+01:00"}
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
### intuizione 1
in pratica $Kern(L)$ o $Kern(A)$ ti dice come sono distribuiti i vettori del dominio che vengono mandati in un certo vettore del codominio, se  $dim(kern(L)) = 1$ vuol dire che la "dimensione" dell'insieme dei vettori mandati nell'origine è $1$ e quindi è una retta. Tutta una retta di vettori del dominio viene mandata nell'origine del codominio. 
Se adesso prendo un generico vettore $\underline{b}$ dell'immagine di $L$ ho la seguente proprietà  :
$$\underline{x} : L(\underline{x}) = \underline{b}$$
$$H:= kern(L) = \{ v \in V : L(v) = \underline{0} \}$$
$$v_{0} \in H\implies L( \underline{x} + v_{0}) = L(\underline{x})+L(v_{0}) = L(\underline{x})+\underline{0} = \underline{b}+\underline{0} = \underline{b}$$
in pratica se "mi sposto" da $\underline{x}$ con un vettore del nucleo vengo comunque mappato in $\underline{b}$ da $L$.
Questo è il motivo per cui solo le [[01-uni/primo-anno/gal/definizioni/def-funzione-lineare\|funzioni lineari]] il cui $kern$ è solo il vettore nullo sono iniettive, se no ci sarebbero infinite soluzioni trovate aggiungendo ad una soluzioni i vettori del $kern$.