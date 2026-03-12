---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/gal/definizioni/def-matrice-tbf/","tags":["math","uni"],"updated":"2026-03-12T21:14:07.818+01:00"}
---

Una $matrice$ $m \times n$ è una tabella rettangolare di numeri organizzati in $m$ righe e $n$ colonne: $$ A = \begin{bmatrix} a_{11} & a_{12} & \cdots & a_{1n} \\ a_{21} & a_{22} & \cdots & a_{2n} \\ \vdots & \vdots & \ddots & \vdots \\ a_{m1} & a_{m2} & \cdots & a_{mn} \end{bmatrix} $$
L'elemento $a_{ij}$ si trova alla riga $i$ e alla colonna $j$. 
___
### sistemi lineari
per ragioni che devo ancora scrivere, dato un sistema $lineare$ (polinomi di 1° grado) di $n$ variabili esiste una matrice $A$ chiamata matrice dei coefficienti che codifica l'informazione del sistema e la rappresenta in un modo "comodo" : 
$$\begin{cases}
2x_{1}+3x_{2} -x_{3} = 0 \\
5x_{1}-3x_{2}+x_{3} = 2
\end{cases}\ \ \ \ \ \ \rightarrow \ \ \  \ \ \begin{bmatrix}
2  & 3  & -1 \\
5 & -3 & 1
\end{bmatrix}$$
questo ha senso anche perché l'informazione contenuta nel sistema lineare non è influenzata dal tipo di oggetto $x_i$ ma dai coefficienti per cui sono moltiplicati e per il termine noto (tbd).
____
### informazione
Se si vedono le equazioni come dei modi per codificare delle informazioni (vettori riga), le matrici diventano naturalmente degli insiemi di informazioni (o condizioni, sono equivalenti) che devono valere allo stesso tempo. Con questa stessa prospettiva, se trovare la soluzione di un'equazione vuol dire trovare l'equazione più "semplice" possibile che contiene la stessa informazione, trovare la "soluzione" di una matrice è la stessa cosa di renderla in scala, ovvero di creare una matrice equivalente che è più "semplice".
___