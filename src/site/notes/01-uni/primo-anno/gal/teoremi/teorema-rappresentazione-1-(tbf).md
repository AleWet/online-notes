---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/gal/teoremi/teorema-rappresentazione-1-tbf/","tags":["math","uni"],"updated":"2026-03-30T16:17:45.559+02:00"}
---

Sia $L$ una [[01-uni/primo-anno/gal/definizioni/def-funzione-lineare\|funzione lineare]] definita da uno [[01-uni/primo-anno/gal/definizioni/def-spazio-vettoriale\|spazio vettoriale]] di scalari come $\mathbb{R}^n$ a un'altro spazio di scalari come $\mathbb{R}^m$, allora esiste un'unica [[01-uni/primo-anno/gal/definizioni/def-matrice-(tbf)\|matrice]] $A$ che rappresenta $L$ : 
$$L : \mathbb{R}^n \to \mathbb{R}^m$$
$$\iff$$
$$A = [ \underline{c_{1}} | \underline{c_{2}}, \dots | \underline{c_{n}}]$$
c'è quindi una corrispondenza biunivoca tra le matrici definite tra $\mathbb{R}^n$ e $\mathbb{R}^m$ e le funzioni lineari definite tra gli stessi insiemi. La matrice $A(L)$ è definita nel seguente modo :
$$A = [L(e_{1}) | L(e_{2})| \dots | L(e_{n})]$$
dove $e_{i}$ sono le basi canoniche di $R^n$. Posso sempre associare a una matrice $A$ una funzione lineare $L_{A}$ e a una funzione lineare $L$ una matrice $A(L)$. 
### intuizione 1
In pratica stai dicendo che puoi vedere le matrici come funzioni lineari tra vettori di scalari e il suo comportamento è definito univocamente da dove vengono mappate le basi canoniche. Qui capisci perché il prodotto matrice-vettore è definito come combinazione lineare delle colonne, perché vuoi rappresentare una funzione lineare. Prima definisci le funzioni lineari e poi trovi un modo comodo per rappresentarle come matrice.
### intuizione 2 (da riscrivere)
Le funzioni lineari sono particolari perché l'immagine della somma è la somma delle immagini, ovvero che se sommo due vettori nel dominio, la somma delle loro immagini deve essere mappata all'immagine della somma dei due vettori. Questo mi permette di fare la seguente osservazione : visto che posso descrivere tutti i vettori del dominio come somme delle basi (qui canoniche) posso descrivere esattamente come si comporta la matrice nella sua totalità analizzando dove vanno a finire le basi canoniche : $L(e_{i})$.
Per sapere dove va a finire un vettore generico, prima vedo dove finiscono le basi canoniche, poi le scalo e sommo per arrivare alla "somma delle immagini". Prima vedo le basi canoniche nel codominio, una volta lì le compongo per formare il mio nuovo vettore che sarà la "somma delle immagini" che per le funzioni lineari è "l'immagine della somma".
### dimostrazione
Si dimostra vedendo che il prodotto matrice-vettore è combinazione lineare delle colonne della matrice con i pesi il vettore :
$$x = x_{1}e_{1}+x_{2}e_{2}+\dots+x_{n}e_{n}$$
$$L(x) = L(x_{1}e_{1}+\dots+x_{n}e_{n})$$
$$L(x) = L(x_{1}e_{1})+L(x_{2}e_{2})+\dots+L(x_{n}e_{n})$$
qui visto che $x_i$ sono scalari e $e_i$ sono vettori, posso portare fuori $x_i$ :
$$L(x) = x_{1}L(e_{1})+x_{2}L(e_{2})+\dots+x_{n}L(x_{n})$$
se rinomino ogni vettore $L(e_{i})$ come $c_{i}$ (che poi diventano le colonne della mia matrice) trovo :
$$L(x) = c_{1}x_{1}+c_{2}x_{2}+\dots+c_{n}x_{n}$$
questo equivale a creare una matrice $A$ che ha come colonne $c_{i}$ : 
$$\iff Ax = c_{1}x_{1}+\dots+c_{n}x_{n}\ \ \ \ \ \ \ \ \ \  \ \square$$
