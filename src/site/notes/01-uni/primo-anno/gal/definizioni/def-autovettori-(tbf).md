---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/gal/definizioni/def-autovettori-tbf/","tags":["math","uni"],"updated":"2026-04-23T17:46:32.623+02:00"}
---

# intro
Prima di definire autovettori e autovalori è utile capire il motivo per cui sono utili. In generale una [[01-uni/primo-anno/gal/definizioni/def-funzione-lineare\|funzione lineare]] definita tra due [[01-uni/primo-anno/gal/definizioni/def-spazio-vettoriale\|spazi vettoriali]] uguali (o endomorfismo), presa una [[01-uni/primo-anno/gal/definizioni/def-base\|base]] $B$, è definita da $n^2$ numeri che formano la matrice rappresentativa, questo perché in genere un vettore della base non è "mandato" dalla trasformazione in un vettore "comodo" rispetto alla base $B$, se per esempio prendo $V = \mathbb{R}^2$ con le basi canoniche e la trasformazione $L$ : 
$$A = \begin{bmatrix}
2   &  1\\  4  & 3
\end{bmatrix}$$
vuol dire che $e_{1}$ viene mandato in $[2, 4]$ e $e_{2}$ in $[1, 3]$ che non sono "belli" rispetto alle basi canoniche. Possono notare però che **a volte** ci sono dei vettori che vengono mandati in multipli di loro stessi : 
$$\exists \ \text{(a volte)} \ v \in V : L(v) = kv \ \ \ k \in \mathbb{R}$$
se prendi per esempio una simmetria:
$$A(L) = \begin{bmatrix}
0  & 1 \\
1 & 0
\end{bmatrix}$$
ci sono almeno due vettori che non vengono "spostati dal loro [[01-uni/primo-anno/gal/definizioni/def-span\|span]]"  : 
$$v_{1} = [1, 1], \ \ v_{2} = [1, -1]$$
infatti vengono solo traslati di uno scalare da $A$ : 
$$Av_{1} = [1,1] = 1v_{1} \ \ \ \ \ \ \ \ Av_{2} = [-1, 1] = -1v_{2}$$
rispetto alla trasformazione $A$ ho trovato due vettori che variano solo di uno scalare. Questa cosa è molto utile visto che, essendo una trasformazione lineare, posso descrivere cosa succede a tutta la trasformazione se ho abbastanza vettori trasformati (in questo caso ne ho 2 e lo spazio ha [[01-uni/primo-anno/gal/definizioni/def-dimensione\|dimensione]] 2). Quindi imposto una nuova base di $\mathbb{R}^2$ : 
$$ C = ([1,1], [-1,1])$$
a questo punto devo anche cambiare la matrice $A$ che rappresenta la trasformazione $L$, per fare ciò applico la matrice a tutti i vettori della nuova base $C$ e metto le coordinate dei vettori risultanti in una nuova matrice $A'$. Tuttavia so già com'è fatta questa matrice, visto che i vettori della base li ho scelti apposta in modo che la loro immagine sia uguale ma moltiplicata per uno scalare : 
$$A(c_{1}) = c_{1} \implies [c_{1}]_{C}= [1,0] \ \ \ \ \ \ \ A(c_{2}) = c_{2} \implies [c_{2}]_{C} =  [0,-1]$$
Noto quindi che l'unica informazione contenuta nella matrice rappresentativa $A'$ sono gli scalari associati ad uno dei vettori trovati prima : 
$$A' = \begin{bmatrix}
1 & 0 \\
0  & -1
\end{bmatrix}$$
Ho quindi trovato un modo per rappresentare una trasformazione lineare invece che con $n^2$ informazioni con $n$ al costo di dover imporre le giuste basi.
___
# autovettori e autovalori
Preso sempre $L$ come endomorfismo di $L$, definisco $v$ **autovettore** di $L$ se :
$$v \neq 0 \tag{1}$$
$$\exists\  \lambda \in \mathbb{R} : L(v) = \lambda v \tag{2}$$
dove $\lambda$ è definito l'**autovalore** dell'autovettore $v$. 
Si dice quindi che la seguente è l'equazione degli autovettori e autovalori : 
$$L(v) = \lambda v$$
la quale non è lineare e non può quindi essere risolta solo con un sistema lineare (staresti cercando la coppia $(\lambda, v)$). 
### osservazione 1
Importante notare come questo è definito a priori delle basi, le funzioni lineari non operano solo su vettori di $\mathbb{R}^n$ ma su tutti gli spazi vettoriali e quindi allo stesso modo gli autovettori e autovalori sono definiti per tutti gli spazi vettoriali. 
### osservazione 2
Con questa definizione, una matrice è [[01-uni/primo-anno/gal/definizioni/def-matrice-diagonale\|diagonalizzabile]] se e solo se $V$ ha una base formata solo da autovettori. In tal caso la matrice diagonale sarà formata dagli autovalori di questa base.
___
# ricerca di autovalori e autovettori
Sempre preso lo stesso $L$ di prima, come fai trovare gli autovalori e autovettori? Il ragionamento nasce dalla seguente osservazione: trovato uno specifico autovalore $\lambda$, posso notare che tutti i vettori dello span di un'autovettore sono tutti moltiplicati per lo stesso scalare $\lambda$ dopo la trasformazione:
$$v : L(v) = \lambda v, \ \ w \in span(v) \implies \exists t \in \mathbb{R} : w = tv$$
$$\implies L(w) = L(tv) = tL(v) = t(\lambda v) = \lambda(tv)$$
questo vuol dire che tutti i vettori della retta $span(v)$ sono moltiplicati per lo stesso $\lambda$. Ergo se trovo tutti i $\lambda_{1}, \dots, \lambda_{n}$ posso poi impostare il **sistema lineare** : 
$$L(v) = \lambda _{i}v$$
che mi trova la forma generica di $v$. Questo perché tutti i vettori dello $span(v)$ soddisfano quell'equazione. Appena trovo i $\lambda _i$ ho tutto quello che mi serve per identificare (al massimo) $n$ sistemi lineari che mi trovano (al massimo) $n$ sottospazi vettoriali che mi identificano tutti gli autovettori associati a $\lambda_i$. Dopo questo ragionamento capisco che devo prima cercare $\lambda_{i}$.
Detto ciò, fisso una base $B = (b_{1},\dots,b_{n})$ di $V$, trovo la matrice rappresentativa:
$$A = [L]_{B}^B$$
e scrivo di nuovo l'equazione degli autovalori e autovettori:
$$Av = \lambda v \iff Av = \lambda Iv \iff $$
$$(A-\lambda I)v = \underline{0}$$
questa relazione è vera se in due casi :
1) quando $v$ è il vettore nullo ma è un caso che non mi interessa ($\underline{0}$ non è autovettore per definizione)
2) quanto il termine a sinistra $(A-\lambda I)$ ammette dei vettori non nulli che sono mandati in $0$, ovvero quando $dim(kern(A-\lambda I)) \geq 1$, questo è vero se e solo se:
$$\det(A-\lambda I) = 0$$
ho trovato così un modo per "isolare" $\lambda$. In pratica ti stai chiedendo se esistono dei valori di $\lambda$ per cui l'espressione $A-\lambda I$ manda dei vettori non nulli in $\underline{0}$ che saranno poi gli autovettori. 
### autospazio
Trovato un valore di $\lambda$ definisco quindi l'**autospazio** relativo al valore di $\lambda$ : 
$$V_{\lambda} = Kern(L - \lambda I) = \{ v \in V \ | \ L(v) = \lambda v \}$$
che è l'insieme di tutti gli autovettori relativi ad un autovalore $\lambda$. Questo autospazio può essere di dimensione qualsiasi, anche più di 1.
### polinomio caratteristico
Per risolvere l'equazione devo per forza espandere un minimo il determinante : 
$$\det(A-\lambda I) = 0 \iff \det(B) = 0$$
$$P_{A}(\lambda)=\det (B) = \begin{vmatrix}
a_{11}-\lambda & a_{12} & \dots & a_{1n}  \\
a_{21} & a_{22}-\lambda & \dots & a_{2n}  \\
\vdots & \vdots & \ddots & \vdots \\
a_{n1} & a_{n 2} & \dots & a_{nn}-\lambda
\end{vmatrix}$$
dove $P_{A}(\lambda)$ lo chiamo il **polinomio caratteristico** della matrice $B$. Espandendo ancora trovo:
$$P_{A}(\lambda)= \sum (\text{questa è una formula orribile non la scrivo, l'importante è la formula dopo})$$
$$P_{A}(\lambda) = (-1)^n \lambda^n + tr(A)\lambda^{n-1}+\dots+\det(A)$$
$$tr(A) = \sum_{i=1}^n a_{ii}$$
