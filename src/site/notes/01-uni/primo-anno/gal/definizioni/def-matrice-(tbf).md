---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/gal/definizioni/def-matrice-tbf/","tags":["math","uni"],"updated":"2026-03-15T10:57:09.005+01:00"}
---

Una $matrice$ $m \times n$ è una tabella rettangolare di numeri organizzati in $m$ righe e $n$ colonne: $$ A = \begin{bmatrix} a_{11} & a_{12} & \cdots & a_{1n} \\ a_{21} & a_{22} & \cdots & a_{2n} \\ \vdots & \vdots & \ddots & \vdots \\ a_{m1} & a_{m2} & \cdots & a_{mn} \end{bmatrix} $$
L'elemento $a_{ij}$ si trova alla riga $i$ e alla colonna $j$.
### intuizione 1
Le matrici sono particolarmente utili poiché, preso un sistema lineare (grado massimo di ogni incognita è $1$) di $n$ incognite e $m$ equazioni, allora esso può essere rappresentato nel seguente modo:
$$\begin{cases}
a_{11}x_{1}+a_{12}x_{2}+\dots+a_{1n} = b_{1} \\
a_{21}x_{1}+a_{22}x_{2}+\dots+a_{2n} = b_{2} \\
\vdots \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \  \vdots  \ \ \ \ \ \ \ \ \  \ddots  \ \ \ \ \ \ \ \ \ \ \ \ \ \  \vdots \\
a_{m 1}x_{1} + a_{m 2}x_{2} + \dots +a_{mn} = b_{n} 
\end{cases} \iff A \underline{x} = \underline{b}$$
dove $A$ è chiamata $\text{matrice dei coefficienti}$ del sistema, il vettore $\underline{x}$ è il vettore di "input" delle variabili e il vettore $\underline{b}$ è il vettore di "output" dei termini noti. Equivalentemente si può rappresentare il sistema senza il vettore delle variabili $\underline{x} = \{ x_{1},x_{2},\dots  , x_{}{n}\}$ che risulta superfluo : 
$$[A|b] \iff \begin{bmatrix} a_{11} & a_{12} & \cdots & a_{1n}  & b_{1n} \\ a_{21} & a_{22} & \cdots & a_{2n}  & b_{2n} \\ \vdots & \vdots & \ddots & \vdots   & \vdots\\ a_{m1} & a_{m2} & \cdots & a_{mn}  & b_{mn} \end{bmatrix}$$
Tutte le proprietà delle matrici definite a prescindere da che variabili sono usate (sono infatti definite su uno [[01-uni/primo-anno/gal/definizioni/def-spazio-vettoriale\|spazio vettoriale]] generico), l'unica cosa che concerne i teoremi e i calcoli sono i coefficienti di tali sistemi lineari, non le incognite.
____
### intuizione 2 (di questa non sono sicuro)
L'altro modo per vedere le matrici è come una "fuzione" che prende in input un vettore di $\mathbb{R}^n$ e ritorna in output un vettore $\mathbb{R}^m$ : 
$$A( \underline{x} \in \mathbb{R}^n) = \underline{b} \in \mathbb{R}^m$$
Si nota subito che il "tipo di computazione" fatta dalla matrice è una [[01-uni/primo-anno/gal/definizioni/def-combinazione-lineare\|combinazione lineare]] delle colonne $\underline{c}$ con pesi il vettore $\underline{x}$ :
$$A \underline{x} = c_{1} x_{1} + c_{2} x_{2} + \dots + c_{n}x_{n}$$
di conseguenza si dimostra subito che il prodotto matrice-vettore è una [[01-uni/primo-anno/gal/definizioni/def-funzione-lineare\|funzione lineare]] :
$$A(x+y) = Ax + Ay \ \ \ \land \ \ \ A(cx) = cA(x)$$

### intuizione da controllare
non sono sicuro della seguente informazione
Il modo più generale che mi viene in mente per definire una matrice è il seguente: una matrice è un modo molto comodo per rappresentare [[01-uni/primo-anno/gal/definizioni/def-funzione-lineare\|funzioni lineari]], non si può dire che le matrici **sono** funzioni lineari ma in pratica sono un modo abbreviato per scrivere funzioni lineari. 

 L'insieme delle funzioni lineari $L : V \to W$ è **isomorfo** a quello delle matrici costruibili tra i due spazi ma non hanno le stesse caratteristiche, sono oggetti diversi. 
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