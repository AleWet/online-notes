---
{"dg-publish":true,"permalink":"/uni/primo-anno/analisi-1/funzioni/definizioni/def-funzione-convessa-tbd/","tags":["math","uni"]}
---

# combinazione convessa
dati $x,y \in \mathbb{R}, \ \ x\ne y$ chiamiamo combinazioni convesse di $x,y$ tutti i numeri della forma:
$$z_{\lambda} = \lambda x + (1-\lambda)y \ \ \ \lambda \in [0,1]$$
ovvero i numeri che ottieni "scorrendo" l'intervallo $[0,1]$ con un parametro $\lambda$.
### osservazione
tutti e soli i numeri compresi tra $x$ e $y$ sono della forma $z_\lambda$ dove $\lambda = \frac{y-z}{y-x}$.
# funzione convessa
una funzione $f:[a,b] \to \mathbb{R}$ è detta convessa se:
$$\forall\lambda\in(0,1) \text{ si ha che }$$
$$f(\lambda x+(1-\lambda)y) \le \lambda f(x) + (1-\lambda)f(y)$$
### interpretazione geometrica
sia $r$ la retta passante per i punti $(x, f(x))$ e $(y, f(y)) \implies$
$$r(t) = \frac{f(y)-f(x)}{y-x}(t-x) + f(x)$$
$$\forall t \in [x,y], f(t) \le r(t)$$
$$t = z_{\lambda} \implies\forall \lambda \in [0,1] \text{ si ha che } f(z_\lambda) \le r(z_\lambda)$$
$$r(x) = \frac{f(y)-f(x)}{y-x}(x\lambda + (1-y)\lambda - x)  +f(x)$$
$$r(x) = \frac{f(y)-f(x)}{y-x}((1-\lambda)(y-x) + f(x)$$
$$r(x) = (f(y)-f(x))(1-\lambda)+f(x) = f(x)\lambda + (1-\lambda)f(y)$$
$$\implies f(t) \le r(t) \text{ è equivalente all'equazione della definizione analitica}$$
