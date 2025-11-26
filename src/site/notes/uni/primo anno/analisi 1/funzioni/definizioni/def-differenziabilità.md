---
{"dg-publish":true,"permalink":"/uni/primo-anno/analisi-1/funzioni/definizioni/def-differenziabilita/","tags":["math","uni"]}
---

# intuizione
presa una funzione $f$ derivabile in $x_0$, più ci si avvicina al punto $x_0$ più la funzione diventa approssimabile con la retta tangente in $x_0$, prendi per esempio:
$$sin(x), \ \ r_0(x) = (x-0) + sin(0) = x$$
è da qui che viene l'[[uni/primo anno/analisi 1/successioni/definizioni/def-asintotico\|asintotico]], sto approssimando la mia funzione con una retta.
# definizione
$f:(a,b) \to \mathbb{R}, \ \ \  x_0 \in (a,b)$, $f$ è **differenziabile** in $x_0$ se
$$\exists L \in \mathbb{R} \text{ e una funzione } \omega(h) : \omega(h) \to 0 \text{ quando } h \to 0 \text{ tali che } $$
$$f(x_0+h) = f(x_0) + Lh + h\omega(h)$$
questa definizione diventa chiara se prendo $h = x-x_0$ :
$$f(x) = f(x_0) + L(x-x_0) + (x-x_0)\omega(x-x_0)$$
ovvero una retta : 
$$r_{x_0} = f(x_0) + L(x-x_0)$$
e un errore che va  0 "più veloce" di una retta, l'approssimazione lineare è il termine dominante : 
$$error(h) = \omega(x-x_0) * (x-x_0)$$
questo è quindi un termine che quando $x\to x_0, \ \omega(x-x_0) \to 0$ ma questo errore non è il termine dominante, è trascurabile rispetto all'approssimazione della retta :
$$\lim_{x \to x_0} \frac{errore(x)}{x-x_0} = 0$$
### osservazione
in $\mathbb{R}^1$, ovvero la retta dei reali, questa nozione è equivalente alla nozione di [[uni/primo anno/analisi 1/funzioni/definizioni/def-derivata\|derivabilità]] come dice il [[uni/primo anno/analisi 1/funzioni/teoremi/teorema-equivalenza-derivabile-differenziabile\|seguente teorema]].