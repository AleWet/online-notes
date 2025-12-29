---
{"dg-publish":true,"permalink":"/uni/primo-anno/analisi-1/basi-funzioni/definizioni/def-punti-accumulazione-and-others/","tags":["math","uni"]}
---

# punti di accumulazione
sia $A \subseteq \mathbb{R}$ allora $x \in \overline{\mathbb{R}}$ è un punto di accumulazione per l'insieme $A$ se:
$$\forall u(x), \ \dot{u}(x)\cap A \ne \emptyset$$
dove $u(x)$ e $\dot{u}(x)$ sono l'[[uni/primo anno/analisi 1/basi funzioni/definizioni/def-intorni\|intorno]] e l'[[uni/primo anno/analisi 1/basi funzioni/definizioni/def-intorni\|intorno bucato]] di $x$. 
Quindi vuol dire che in ogni intorno bucato di $x$ c'è un elemento dell'insieme $A$, ovvero che esistono infiniti elementi dell'insieme $A$ che si avvicinano arbitrariamente al punto $x$ e $\ne x$.
### esempio
$$A = \left\{ 1, \frac{1}{2}, \frac{1}{3}, \frac{1}{4},... \right\}$$
$$0 \text{ è punto di accumulazione per l'insieme A}$$
____
# punti isolati
negazione del punto di accumulazione, ovvero un punto $x \in A$ t.c. : 
$$\exists u(x) : u(x)\cap A = \{x\}$$
Ovvero un intorno di $x$ dove l'unico punto in comune con l'insieme $A$ è l'elemento $x$. Quindi vuol dire che tutti gli intorni più piccoli avranno la stessa proprietà. 
### osservazione importante
da notare che a differenza del punto di accumulazione si chiede che il punto isolato appartenga all'insieme.
### esempio
$$A = [0,1]\cap\left\{  \frac{3}{2} \right\}\cap[2,3]$$
$$ \{3 / 2\} \text{ è un punto isolato dell'insieme A}$$
___
# punto di frontiera
un punto $x \in \mathbb{R}$ (NON $\overline{\mathbb{R}}$) è detto di frontiera per l'insieme $A$ se:
$$\forall u(x), \ u(x)\cap A \ne \emptyset \ \land\ u(x)\cap A^C \ne \emptyset$$
dove $A^C$ è l'insieme complementare all'insieme $A$. 
In pratica sono i punti che sono "ai lati" dell'insieme $A$. Di conseguenza tutti i punti di frontiera sono anche [[uni/primo anno/analisi 1/basi funzioni/definizioni/def-punti-accumulazione-and-others#punti isolati\|punti isolati]] poiché ricordiamo che i punti isolati sono compresi nell'insieme $A$.
### osservazione 
Chiediamo che i punti di frontiera siano finiti ma effettivamente per gli insiemi non limitati possiamo dire che $\pm\infty$ sono moralmente punti di frontiera, ci si avvicina sempre ma non lo si raggiunge mai. 
### esempio
$$A = [0,1)$$
$$\{0, 1\} \text{ sono punti di frontiera per A}$$
___
# punto interno
$x \in A$ è interno all'insieme $A$ se 
$$\exists u(x) : u(x) \subset A$$
ovvero che dato un certo $u(x)$ in poi, tutti i punti dell'intorno sono dentro l'insieme $A$. Questo vuol dire che i punti interni non possono essere punti di frontiera e viceversa.
### esempio
$$A = [0,1]$$
$$(0,1) \text{ sono tutti punti interni dell'insieme A}$$
____
# classificazione
schema fatto dal Pata molto comprensivo
- se $x\in A$ allora può essere
	- punto isolato 
	- punto di accumulazione
		- punto interno
		- punto di frontiera
- se $x \not\in A$ allora può essere
	- punto di accumulazione $\implies$ punto di frontiera
	- punto esterno, ovvero $x\in A^C$

(per più info riguardo queste note guarda il [[Limiti.pdf|questo link del Pata]])