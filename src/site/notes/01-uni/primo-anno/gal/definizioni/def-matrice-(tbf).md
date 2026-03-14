---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/gal/definizioni/def-matrice-tbf/","tags":["math","uni"],"updated":"2026-03-14T16:45:44.328+01:00"}
---

Una $matrice$ $m \times n$ è una tabella rettangolare di numeri organizzati in $m$ righe e $n$ colonne: $$ A = \begin{bmatrix} a_{11} & a_{12} & \cdots & a_{1n} \\ a_{21} & a_{22} & \cdots & a_{2n} \\ \vdots & \vdots & \ddots & \vdots \\ a_{m1} & a_{m2} & \cdots & a_{mn} \end{bmatrix} $$
L'elemento $a_{ij}$ si trova alla riga $i$ e alla colonna $j$. Il modo più generale che mi viene in mente per definire una matrice è il seguente: una matrice è un modo molto comodo per rappresentare [[01-uni/primo-anno/gal/definizioni/def-funzione-lineare\|funzioni lineari]], non si può dire che le matrici **sono** funzioni lineari ma in pratica sono un modo abbreviato per scrivere funzioni lineari. 

 ( non sono sicuro della seguente informazione : L'insieme delle funzioni lineari $L : V \to W$ è **isomorfo** a quello delle matrici costruibili tra i due spazi ma non hanno le stesse caratteristiche, sono oggetti diversi. )
#### esempio
Data una funzione (lineare) $f:\mathbb{R} \to \mathbb{R}, \ \ f(x) = 3x$ posso definire una matrice $A$ che mi generalizza questa funzione lineare in una variabile generica : $A = [3]$. Questa non è un'analogia, è il caso specifico dove $n = m = 1$. la funzione $f$ a questo punto può essere rappresentata come :
$$f(x) = T(x) = Ax= 3x$$
$A$ non è una funzione, $T$ lo è.
___
### osservazione 1 (tbf)
per ragioni che devo ancora scrivere, dato un sistema $lineare$ (polinomi di 1° grado) di $n$ variabili esiste una matrice $A$ chiamata matrice dei coefficienti che codifica l'informazione del sistema e la rappresenta in un modo "comodo" a prescindere dalle variabili utilizzate: 
$$\begin{cases}
2x_{1}+3x_{2} -x_{3} = 0 \\
5x_{1}-3x_{2}+x_{3} = 2
\end{cases}\ \ \ \ \ \ \rightarrow \ \ \  \ \ \begin{bmatrix}
2  & 3  & -1 \\
5 & -3 & 1
\end{bmatrix}$$
questo ha senso anche perché l'informazione contenuta nel sistema lineare non è influenzata dal tipo di oggetto $x_i$ ma dai coefficienti per cui sono moltiplicati e per il termine noto.
_____
### osservazione 2
presa una matrice $A$ di $n$ colonne $c_{1}, c_{2}, \dots , c_{n} \in \mathbb{R}^m$ e un vettore $v \in R^n$ il prodotto vettore-matrice può essere visto esattamente come [[01-uni/primo-anno/gal/definizioni/def-combinazione-lineare\|combinazione lineare]] delle colonne di $A$ con i "pesi" del vettore $v$ : 
$$Av := x_{1}c_{1} + x_{2}c_{2} + \dots, x_{n}c_{n}$$
allora il sistema $Av = b$ è risolubile $\iff$ $b$ è una **combinazione lineare** delle colonne di $A$.
____
### osservazione 3
Se si vedono le equazioni come dei modi per codificare delle informazioni (vettori riga), le matrici diventano naturalmente degli insiemi di informazioni (o condizioni, sono equivalenti) che devono valere allo stesso tempo. Con questa stessa prospettiva, se trovare la soluzione di un'equazione vuol dire trovare l'equazione più "semplice" possibile che contiene la stessa informazione, trovare la "soluzione" di una matrice è la stessa cosa di renderla in scala, ovvero di creare una matrice equivalente che è più "semplice".
___