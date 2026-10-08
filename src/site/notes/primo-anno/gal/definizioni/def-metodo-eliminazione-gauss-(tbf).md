---
{"dg-publish":true,"permalink":"/primo-anno/gal/definizioni/def-metodo-eliminazione-gauss-tbf/","tags":["math","uni"],"updated":"2026-03-25T17:14:00.446+01:00"}
---

### matrice a scala
una [[primo-anno/gal/definizioni/def-matrice-(tbf)\|matrice]] si dice **a scala** quando ha la seguente forma:
$$\begin{bmatrix}
a & b & c & d  & \dots \\
0 & e & f & g & \dots \\
0 & 0 & 0 & h & \dots \\
\vdots & \vdots & \vdots & \vdots &  \ddots
\end{bmatrix}$$
ovvero quando il primo elemento non nullo trovato su una riga è l'ultimo elemento non nullo di quella colonna (partendo da top-left). La notazione che si usa è $U$ per le matrici a scala.
____
### eliminazione di Gauss
Presa una $A$ di grandezza $m \times n$, si usa il **metodo di eliminazione di gauss** per trovare la matrice a scala associata. L'algoritmo è il seguente:
1) fai in modo che la prima riga sia quella con più elementi non nulli partendo da sinistra
2) prendi la riga dopo e gli sottrai la prima riga in modo da rendere il termine più a sinistra nullo
3) repeat finché non arrivi in fondo
questo metodo garantisce che alla fine rimangano solo tutte le equazioni "indipendenti", ovvero stai togliendo le informazioni ridondanti contenute nelle altre equazioni della matrice. 
### insieme soluzione
Il motivo per cui questa serie di operazioni lasci intatto l'insieme delle soluzioni di una matrice non è banale, si può vedere però che le operazioni fondamentali di riga sono alla fine [[primo-anno/gal/definizioni/def-combinazione-lineare\|combinazioni lineari]] dei vettori riga della matrice di partenza che non intaccano le "informazioni espresse" dalle equazioni, ovvero non cambia lo [[primo-anno/gal/definizioni/def-spazio-riga\|spazio riga]] della matrice.
### spazio colonna
Al contrario dello spazio riga, lo [[primo-anno/gal/definizioni/def-spazio-colonna\|spazio colonna]] cambia quando fai operazioni sulle righe, questo si vede subito perché stai effettivamente cambiando l'ordine delle coordinate dei vettori colonna di $A$, i vettori che ci sono nella matrice a scala sono in qualche modo i vettori di $A$ ma trasformati.
### sostituzione all'indietro
Le matrici a scala sono particolarmente utili perché permettono di "risolvere" un sistema associato molto velocemente con delle sostituzioni all'indietro. Se partiamo con una matrice del genere :
$$ A =\begin{bmatrix}
a & b & c \\
d & e & f  \\
g  & h & i
\end{bmatrix}$$
e la si riduce a scala :
$$ U =\begin{bmatrix}
a & b & c \\
0 & j & k \\
0 & 0 & l
\end{bmatrix}$$
e si esamina un possibile sistema lineare associato a questa matrice : 
$$U \underline{x} = \underline{b} \iff \begin{cases}
ax_{1}+bx_{2}+cx_{3} = b_{1} \\
0x_{1}+jx_{2}+kx_{3} = b_{2} \\
0x_{1}+0x_{2}+lx_{3} = b_{3}
\end{cases}$$
si nota subito come avere una matrice a scala rende la risoluzione di questo sistema (ovvero trovare il vettore $\underline{x} : U \underline{x} = \underline{b}$) molto più facile poiché basta sostituire all'indietro partendo dall'ultima equazione :
$$lx_{3} = b_{3} \implies x_{3} =\frac{b_{3}}{l} \implies  jx_{2} = b_{2} -\frac{kb_{3}}{l} \implies \dots$$
