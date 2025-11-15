---
{"dg-publish":true,"permalink":"/uni/primo-anno/analisi-1/funzioni/definizioni/def-continuita/","tags":["math","uni"]}
---

# definizione classica
sia $f : \mathbb{R} \to \mathbb{R}$ e sia $x_0 \in D(f)$ diciamo che $f$ è continua nel punto $x_0$ se 
$$\forall u(f(x_0)) \ \exists u(x_0) : \text{ se } x \in D(f)\cap u(x_0)$$
$$\implies f(x) \in u(f(x_0))$$
$$\iff$$
$$\forall \varepsilon > 0 \ \exists \delta > 0 : \text{ se } x \in D(f) \land |x-x_0| < \delta \implies |f(x) - f(x_0)| < \varepsilon$$
### osservazione 1
cosa cambia da questa definizione alla [[uni/primo anno/analisi 1/funzioni/definizioni/def-limite-funzione\|def-limite-funzione]]? Qui ci interessa cosa fa la funzione nel punto $x_0$, invece nei limiti cosa $f$ in $x_0$ è irrilevante. Infatti nei limiti uso $\dot{u}(x)$ mentre qui $u(x)$ quindi accetto che $x = x_0$. Inoltre cambia che al posto di usare $l$ uso $f(x_0)$.
### osservazione 2
è equivalente a dire che $x_0$ è un punto di accumulazione del dominio $D(f)$ se no il limite non è applicabile.
### osservazione 3
se $x_0$ è un punto isolato del dominio $D(f)$ allora la funzione è continua in $x_0$ poiché $\exists x \in D(f)\cap u(x_0)$ ed è sempre $x_0$ da cui $|f(x_0) - f(x_0)| = 0 < \varepsilon$.
### osservazione 4
se $x_0$ è un punto di accumulazione *bilatero* allora $f$ è continua in $x_0 \iff f$ è continua sia da destra che da sinistra. Se tuttavia in $x_0$ la funzione è continua solo da destra o solo da sinistra allora si dice che la funzione è continua in $x_0$.
___
# continuità successionale
$f$ è continua successionalmente in $x_0$ se 
$$\forall a_n \in D(f) : a_n \rightarrow x_0 \text{ si ha che } f(a_n) \to f(x_0)$$
il [[uni/primo anno/analisi 1/funzioni/teoremi/teorema-ponte-continuità\|seguente teorema]] ti dice che questa cosa è equivalente alla continuità definita sopra. 

