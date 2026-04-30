---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/gal/teoremi/lemma-fondamentale/","tags":["math","uni"],"updated":"2026-03-27T14:14:10.360+01:00"}
---

sia $V$ uno [[01-uni/primo-anno/gal/definizioni/def-spazio-vettoriale\|spazio vettoriale]] con un insieme di generatori di cardinalità $m$, allora se $S$ è un insieme di vettori [[01-uni/primo-anno/gal/definizioni/def-indipendenza-lineare\|linearmente indipendenti]] si ha che :
$$\#S =n\leq m$$
e si ha che $V$ avrà [[01-uni/primo-anno/gal/definizioni/def-dimensione\|dimensione]] finita ($\leq m$).
### dimostrazione
Prima di dimostrare questo devi dimostrare che se hai $n$ vettori indipendenti di $\mathbb{R}^m$ allora si ha che $n\leq m$, sembra che non c'entri nulla ma poi ti serve : 
#### prima parte
sia $S = \{ c_{1},c_{2},\dots,c_{n} \}$ dove $c_{i} \in \mathbb{R}^m$ e dove tutti i vettori $c_{i}$ sono linearmente indipendenti. Prendi poi la matrice $A = [c_{1}|c_{2}|\dots|c_{n}]$, avrai che il [[01-uni/primo-anno/gal/definizioni/def-rango\|rango]] di $A$ è $n\ \  (*)$. Se $A$ ha rango $n$ e $rank(A) \leq m$ ottieni : 
$$n\leq m$$
#### seconda parte
prendo $S = \{ w_{1},w_{1},\dots,w_{m} \}$ di vettori $\in V$ **generatori** di $V$. Poiché $S$ è insieme di generatori, la funzione delle combinazioni lineari di $S$ è **suriettiva** in V :
$$\forall  \underline{u} \in V \ \exists x_{1},x_{2},\dots,x_{m} \in \mathbb{R} : $$
$$x_{1} w_{1}+x_{2}w_{2}+\dots+x_{m}w_{m} = \underline{u}$$
Chiamo questa funzione $L_{S}$ (guarda [[01-uni/primo-anno/gal/definizioni/def-combinazione-lineare\|qui]]) 
$$L_{S} : \mathbb{R}^m \to V$$
$$L_{S}( \underline{x}) = \underline{u} \in V,\ \ \  \ \ \ \underline{x} = (x_{1},x_{2},\dots,x_{m})$$
Adesso devo dimostrare che se ho un'insieme di $n>m$ vettori di $V$, questo sarà linearmente **dipendente**. Prendo quindi $n > m$ vettori di $V$ : 
$$v_{1},v_{2},v_{3},\dots,v_{n} \ \ \ \ \  (n>m)$$
poiché $L_S$ è suriettiva esistono sicuramente $n$ vettori di scalari $c_{1},c_{2},\dots,c_{n} \in \mathbb{R}^m$ tali che:
$$L_{S}( c_{1}) =v_{1}$$
$$L_{S}(c_{2}) = v_{2}$$
$$\dots$$
$$L_{S}(c_{n}) =v_{n}$$
Adesso usi quello dimostrato nella prima parte : i vettori $c_{1},\dots c_{n}$ sono sicuramente linearmente **dipendenti** poiché $n>m$, formerebbero una matrice $A = [c_{1}|\dots|c_{n}]$ dove $rank(A) \leq m <n$ e quindi il $Kern(A)$ non è formato solo da $\underline{0}$. Se sono linearmente dipendenti trovi che :
$$\exists t_{1},t_{2},\dots,t_{n} \text{ non tutti nulli} \ : t_{1}c_{1}+t_{2}c_{2}+\dots+t_{n}c_{n} = \underline{0}$$
che è esattamente quello che vuol dire linearmente dipendenti, che puoi fare lo $\underline{0}$ in più modi non banali. Adesso applichi $L_{S}$ da entrambe le parti :
$$L_{S}(t_{1}c_{1}+\dots+t_{n}c_{n}) = L_{S}( \underline{0})$$
$$\iff t_{1}L_{S}(c_{1}) + t_{2}L_{S}(c_{2})+\dots+t_{n}L_{S}(c_{n}) = L_{S}( \underline{0})$$
$$\iff t_{1}v_{1}+\dots+t_{n}v_{n} = \underline{0}$$
dove per ipotesi $t_{1},\dots,t_{n}$ non sono tutti nulli, allora anche $v_{1},\dots,v_{n}$ sono linearmente **dipendenti**.
___
$(*)$ per dimostrare questo basta usare la condizione di indipendenza lineare sulle colonne di $A$, imponi che $A\underline{x} = \underline{0}$ sia unica che, usando [[01-uni/primo-anno/gal/teoremi/teorema-Rouché-Capelli-(tbf)\|R.C.]], è equivalente a chiedere che il rango di $A$ sia $n$.