---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/analisi-1/funzioni/teoremi/teoremi-funzione-derivata/teorema-derivabile-allora-continua/","tags":["math","uni"]}
---

se $f$ è [[01-uni/primo anno/analisi 1/funzioni/definizioni/def-derivata\|derivabile]] in $x_0 \implies f$ è [[01-uni/primo anno/analisi 1/funzioni/definizioni/def-continuità\|continua]] in $x_0$.
### osservazione
naturalmente non è vero il contrario, prendi la funzione $f(x) = |x|$ che è continua ma non derivabile in $x_0 = 0$ poiché pur essendo derivabile da destra e da sinistra, le rette tangenti non formano un angolo di $\pi$ tra di loro.
### dim
voglio dimostrare che 
$$\lim_{x\to x_0} f(x) = f(x_0)$$
$$\iff \lim_{h \to 0} f(x_0+h) = f(x_0) \iff \lim_{h \to 0}\  [f(x_0+h)-f(x_0)] = 0$$
$$\iff \lim_{h \to 0} \frac{f(x_0+h)-f(x_0)}{h} * h = 0$$
$$\lim_{h\to0}\frac{f(x_0+h)-f(x_0)}{h} = f'(x_0) \in \mathbb{R} \ \ (*)$$
$$\implies f'(x_0) * h \to 0 \ \ \ \ \square$$
$$(*) \text{ visto che ho definito la derivata come un limite finito}$$
è importante far notare che la definizione iniziale di continuità è quella implementabile nei [[01-uni/primo anno/analisi 1/basi funzioni/definizioni/def-punti-accumulazione-and-others\|punti di accumulazione]].