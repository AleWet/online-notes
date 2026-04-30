---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/gal/definizioni/def-spazio-riga/","tags":["math","uni"],"updated":"2026-03-25T17:06:06.506+01:00"}
---

sia $A$ una [[01-uni/primo-anno/gal/definizioni/def-matrice-(tbf)\|matrice]] $\in Mat_{m \times n}$ del tipo : 
$$\begin{bmatrix}
\underline{a_{1}} \\
\underline{a_{2}} \\
\underline{a_{3}} \\
\dots \\
\underline{a_{m}}
\end{bmatrix}$$
dove con la riga $a_i$  intendo un vettore riga di dimensione $n$, definisco $Row(A)$ lo $spazio \ riga$ come l'insieme di tutte le [[01-uni/primo-anno/gal/definizioni/def-combinazione-lineare\|combinazioni lineari]] delle righe della matrice $A$, quindi lo [[01-uni/primo-anno/gal/definizioni/def-span\|span]] dei vettori riga di $A$ :
$$Row(A) = span(\underline{a_{1}},\underline{a_{2}},\dots,\underline{a_{n}})$$
esso è un [[01-uni/primo-anno/gal/definizioni/def-sotto-spazio-vettoriale-(tbf)\|s.s.v.]] di $\mathbb{R}^n$  
### intuizione (tbf)
Lo $span$ delle righe di una matrice può essere visto come l'insieme di tutti i possibili "vincoli" che portano allo stesso risultato. Questo è più facile pensarlo nello spazio 3D : immagina una retta come intersezione di due piani, la matrice che descrive questa retta sta in realtà descrivendo due piani che si intersecano in una retta. Fare le combinazioni lineari di questi due piani (i vincoli, le equazioni della matrice) equivale a trovare tutti i possibili piani che intersecati trovano la retta di prima.
Questo è il motivo per cui il [[01-uni/primo-anno/gal/definizioni/def-metodo-eliminazione-gauss-(tbf)\|MEG]] funziona, perché lascia lo spazio riga invariato (cosa che non è vera per lo [[01-uni/primo-anno/gal/definizioni/def-spazio-colonna\|spazio colonna]]) quindi trova i piani (o altre cose in dimensioni superiori) più "semplici" da descrivere che però hanno le stesse soluzioni di quelli originali.