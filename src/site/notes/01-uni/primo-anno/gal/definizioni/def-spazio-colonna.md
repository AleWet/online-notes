---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/gal/definizioni/def-spazio-colonna/","tags":["math","uni"],"updated":"2026-03-25T20:19:10.110+01:00"}
---

sia $A$ una [[01-uni/primo-anno/gal/definizioni/def-matrice-(tbf)\|matrice]] $\in Mat_{m \times n}$ del tipo : 
$$\begin{bmatrix}  
\underline{c}_{1} | \underline{c}_{2} | \dots | \underline{c}_{n}
\end{bmatrix}$$
dove con la riga $c_i$  intendo un vettore colonna di dimensione $m$, definisco $Col(A)$ lo $spazio \ colonna$ come l'insieme di tutte le [[01-uni/primo-anno/gal/definizioni/def-combinazione-lineare\|combinazioni lineari]] delle colonne della matrice $A$, quindi lo [[01-uni/primo-anno/gal/definizioni/def-span\|span]] dei vettori colonna di $A$ :
$$Col(A) = span(\underline{c_{1}},\underline{c_{2}},\dots,\underline{c_{n}})$$
esso è un [[01-uni/primo-anno/gal/definizioni/def-sotto-spazio-vettoriale-(tbf)\|s.s.v.]] di $\mathbb{R}^m$  
### intuizione
Se vedi la matrice come una [[01-uni/primo-anno/gal/definizioni/def-funzione-lineare\|funzione lineare]], lo $span$ dei vettori colonna di una matrice può essere visto come tutte le combinazioni lineari dei vettori colonna della matrice poiché effettivamente è quello che la matrice "fa" come operazione : 
$$A \underline{x} = c_{1}x_{1}+c_{2}x_{2}+c_{3}x_{3}+\dots+c_{n}x_{n}$$
sono tutte le possibili combinazioni lineari con pesi $x$ delle colonne di $A$ e difatti si ha che:
$$Col(A) = \mathrm{Im}(L_{A})$$
dove con $L_{A}$ si intende la funzione lineare associata a una matrice.


