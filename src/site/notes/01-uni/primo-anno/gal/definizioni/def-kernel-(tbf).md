---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/gal/definizioni/def-kernel-tbf/","tags":["math","uni"]}
---

il $kernel$ o $nucleo$ di una [[01-uni/primo-anno/gal/definizioni/def-matrice-(tbf)\|matrice]] $A$ di forma $m \times n$ è definito come l'insieme delle soluzioni del sistema $omogeneo$ (metti  $\underline{b}=\underline{0}$) associato : 
$$Ker(A) = \{ v \in V \ |\ Av = \underline{0}  \} \iff Sol(A \underline{x} = \underline{0})$$
______
### sotto spazio vettoriale
Il nucleo di una matrice è un [[01-uni/primo-anno/gal/definizioni/def-sotto-spazio-vettoriale-(tbf)\|sottospazio vettoriale]] dello [[01-uni/primo-anno/gal/definizioni/def-spazio-vettoriale\|spazio]] $V$ di partenza, per controllarlo basta usare il [[01-uni/primo-anno/gal/definizioni/def-sotto-spazio-vettoriale-(tbf)#teorema controllo s.s.v\|seguente teorema]] sul sottospazio :
1) $Av = \underline{0}$ è sempre risolubile $\iff Ker(A) \ne \emptyset$
2) la somma di soluzioni del sistema omogeneo è soluzione
3) ogni multiplo di una soluzione è soluzione
### dims
1) $A \underline{0} = \underline{0} \implies Ker(A) \ne \emptyset$
2) $Ah_{1} =Ah_{2} = \underline{0}  \implies A(h_{1}+h_{2})=  Ah_{1}+Ah_{2} = \underline{0}+  \underline{0} = \underline{0}$ 
3) $c \in \mathbb{N}, \ Ah = \underline{0} \implies A(ch) = c(Ah) = c \underline{0} = \underline{0}$
 usando le proprietà delle [[01-uni/primo-anno/gal/definizioni/def-operazione-lineare-(tbd)\|operazioni lineari]] 
 