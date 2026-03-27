---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/gal/definizioni/def-funzione-lineare/","tags":["math","uni"],"updated":"2026-03-27T20:26:01.703+01:00"}
---

chiamiamo $L : V \to W$ una $funzione \ lineare$  se essa soddisfa le seguenti proprietà : 
$$ \tag{additività}\forall u,v \in V,\ \  \ L(u+v) = L(u) + L(v)$$
$$\forall a \in \mathbb{R} \ \forall v \in V, \ \ \ L(av) = aL(v) \tag{omogeneità}$$
dove $V$ e $W$ sono [[01-uni/primo-anno/gal/definizioni/def-spazio-vettoriale\|spazi vettoriali]]
##### esempi
tra i vari esempi di funzioni (o operatori) lineari ci sono
- [[01-uni/primo-anno/analisi-1/funzioni/definizioni/def-integrale-Riemann\|integrali]] : $\frac{d}{dx}:\mathbb{R}^\mathbb{R} \to \mathbb{R}^\mathbb{R}$
- [[01-uni/primo-anno/analisi-1/funzioni/definizioni/def-derivata\|derivate]] : $\int : \mathbb{R}^\mathbb{R} \to \mathbb{R}^\mathbb{R}$
____
### matrici
le matrici di per sé non sono funzioni lineari, tuttavia ogni matrice è associata univocamente ad una funzione lineare $L_{A} : \mathbb{R}^n \to \mathbb{R}^m$, questa nuova funzione è lineare : 
$$A(v+w) = Av + Aw  \ \ \land \ \ A(cv) = cA(v)$$
Esistono quindi funzioni lineari che non possono essere rappresentate da matrici finite, per esempio gli integrali, se esistesse una matrice per gli integrali la computazione sarebbe "facile".