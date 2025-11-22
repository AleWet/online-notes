---
{"dg-publish":true,"permalink":"/uni/primo-anno/analisi-1/funzioni/definizioni/def-funzione-convessa/","tags":["math","uni"]}
---

# combinazione convessa
dati $x,y \in \mathbb{R}, \ \ x\ne y$ chiamiamo combinazioni convesse di $x,y$ tutti i numeri della forma:
$$z_{\lambda} = \lambda x + (1-\lambda)y \ \ \ \lambda \in [0,1]$$
	ovvero i numeri che ottieni "scorrendo" l'intervallo $[0,1]$ con un parametro $\lambda$.
### osservazione
tutti e soli i numeri compresi tra $x$ e $y$ sono della forma $z_\lambda$ dove $\lambda = \frac{y-z}{y-x}$.
# funzione convessa
una funzione $f:[a,b] \to \mathbb{R}$ è detta convessa se:
$$\forall x,y \in [a,b] \text{ dove } x<y, \ \forall\lambda\in(0,1) \text{ si ha che }$$
$$f(\lambda x+(1-\lambda)y) \le \lambda f(x) + (1-\lambda)f(y)$$
### interpretazione geometrica
preso un intervallo $[x,y]\subset[a,b]$ e sia $r$ la retta passante per i punti $(x, f(x))$ e $(y, f(y))$
$$\implies r(t) = \frac{f(y)-f(x)}{y-x}(t-x) + f(x)$$
$$\forall t \in [x,y], f(t) \le r(t)$$
$$t = z_{\lambda} \implies\forall \lambda \in [0,1] \text{ si ha che } f(z_\lambda) \le r(z_\lambda)$$
$$r(z_\lambda) = \frac{f(y)-f(x)}{y-x}(x\lambda + (1-\lambda)y - x)  +f(x)$$
$$r(z_\lambda) = \frac{f(y)-f(x)}{y-x}(1-\lambda)(y-x) + f(x)$$
$$r(z_\lambda) = (f(y)-f(x))(1-\lambda)+f(x) = \lambda f(x) + (1-\lambda)f(y)$$
$$f \text{ è convessa se } f(t) \le r(t)\ \forall t \in [x,y]$$
quindi la convessità ti dice che in ogni intervallo chiuso $[x,y]$ contenuto nell'intervallo di partenza  $[a,b]$ la funzione è $\le$ rispetto alla retta $r_{x,y}$ passante per gli estremi dell'intervallo $[x,y]$. 
### osservazione
$\forall x<y \in [a,b], \forall z_\lambda \text{ di } x,y$ detta $r$ la retta passante per $x, z_\lambda$ e detta $p$ la retta passante per $z_\lambda, y$ si ha che $\text{coefficiente angolare}(r) \le \text{coefficiente angolare}(p)$. 
GUARDA QR3 (fine) per più info DA DIMOSTRARE
### definizione intervallo generale
$$f:I\to \mathbb{R} \text{ è detta convessa se per ogni } [a,b] \subset I$$
$$f \text{ è convessa in } [a,b]$$
### funzione concava
banalmente una funzione $f:[a,b] \to \mathbb{R}$ è concava se $-f$ è convessa oppure se inverti la disuguaglianza di prima:
$$f(\lambda x+(1-\lambda)y) \ge \lambda f(x) + (1-\lambda)f(y)$$
quindi la retta passante per gli estremi deve stare "sotto" la funzione.
