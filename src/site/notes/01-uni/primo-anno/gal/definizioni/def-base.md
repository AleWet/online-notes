---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/gal/definizioni/def-base/","tags":["math","uni"],"updated":"2026-03-26T11:03:51.804+01:00"}
---

sia $V$ uno [[01-uni/primo-anno/gal/definizioni/def-spazio-vettoriale\|spazio vettoriale]] e sia $B$ una $n-upla$ (un insieme ordinato di $n$ elementi) di vettori $\in V$ 
$$B = (\underline{b_{1}}, \underline{b_{2}}, \dots, \underline{b_{n}} \
): \ \underline{b_{i}} \in V$$
L'insieme $B$ si dice $base$ di $V$ **se e solo se** ogni vettore $\underline{v} \in V$ si scrive in **uno e un solo modo** della forma:
$$\underline{v} = a_{1} \underline{b_{1}} + a_{2} \underline{b_{2}} + \dots + a_{n} \underline{b_{n}}$$
dove $t_i$ sono dei parametri arbitrari. In pratica, se avessi una funzione $L_{B}$ che mappa le basi $\underline{b_{i}}$ con dei parametri $a_{1},a_{2}, \dots,  a_{n}$ a dei vettori $\underline{v} \in V$, questa funzione $L_{B}$ è **biunivoca**.
Detto in altro modo, stai dicendo che tutti i vettori di $V$ devono essere rappresentati da una e una sola combinazione lineare dei vettori della base $B$. La funzione $L_{B} : \mathbb{R}^n \to V$ 
([[01-uni/primo-anno/gal/definizioni/def-combinazione-lineare\|combinazione lineare]]) 
$$L_{B} \bigg( \begin{bmatrix}
a_{1} \\
\vdots \\
a_{n}
\end{bmatrix} \bigg) = a_{1} \underline{b_{1}} + a_{2} \underline{b_{2}} + \dots + a_{n} \underline{b_{n}}$$

a certi parametri :  $\begin{bmatrix}a_{1} \\  \vdots  \\ a_{n}\end{bmatrix}$ mappa uno e un solo vettore $\in V$ scalando ogni base $\underline{b_{i}}$ di una quantità $a_{i}$

### definizione equivalente
Equivalentemente, una $n-upla$ di elementi di $V$ è detta una $\iff$ le seguenti sono verificate :
1) $\forall u \in V \ \exists a_{1},a_{2},\dots,a_{n}  : u = a_{1}v_{1} + \dots + a_{n}v_{n}$, ovvero che sono dei generatori
2) $u_{1},\dots ,u_{n}$ sono [[01-uni/primo-anno/gal/definizioni/def-indipendenza-lineare\|linearmente indipendenti]], in breve che $\underline{0}$ si può scrivere in un solo modo come combinazione lineare degli $n$ vettori (non solo con tutti gli scalari messi $=0$)
##### esempio
pensa al piano cartesiano $x,y$, esiste una coppia di vettori $B = \{  \hat{u}, \hat{y}\}$ che, scalati con due parametri $a_{1}, a_{2}$ possono raggiungere tutti i punti del piano. L'osservazione importante da fare è che i vettori della base possono anche non essere perpendicolari, l'unico vincolo è che la funzione associata $L_{B}(a_{1},a_{2}) = a_{1}x_{1} + a_{2}x_{2}$ sia biunivoca. ovvero che 
- ogni vettore $v$ del piano cartesiano (ogni punto stessa cosa) è raggiunto da almeno una coppia di parametri $a_{1},a_{2}$
- a vettori diversi $v_{1} \neq v_{2}$ corrispondono parametri $(a_{11},a_{21}) \neq (a_{21},a_{22}$) diversi
in questo modo non lavori mai con i vettori in sé in $\mathbb{R}^2$ ma invece con le **coordinate** di questi vettori relativi alle basi che scegli (implicitamente quando scrivi $p = (1,2) \in \mathbb{R}^2$ stai dicendo che $p = 1\hat{u}_{x}+2\hat{u}_{y}$ ovvero una combinazione lineare delle basi canoniche).
___
### osservazione 1
Se ho $S$ come basi di $V$, posso dire naturalmente che :
$$V = span(v_{1},v_{2},\dots ,v_{n})$$
questo vale in generale quando $S$ è un'insieme di generatori, possono anche non essere basi (vuol dire semplicemente che ho delle informazioni-vettori superflue che possono essere derivate dalle altre).
___
### osservazione 2
Dato uno s.v. $V$ con le sue basi $B$, esse sono uniche? Presi gli stessi vettori di $B$, ogni ri-arrangiamento delle basi $B$ è un'altra base di $V$, basta cambiare l'ordine.  
___
### notazione
Dato $v \in V$ e $S = (v_{1},v_{2},\dots v_{n})$ una base di $V$, se voglio rappresentare $v$ con le basi $S$ scrivo la seguente cosa :
$$[v]_{S} = \begin{bmatrix}
a_{1} \\
\dots \\
a_{n}
\end{bmatrix}$$

è come se stessi prendendo in considerazione la sua contro-immagine della funzione $L_{B}$ definita sopra : 
$$L_{S}(\begin{bmatrix}
a_{1} \\
a_{n}
\end{bmatrix}) = v \implies [v]_{S} = \begin{bmatrix}
a_{1} \\
a_{n}
\end{bmatrix}$$