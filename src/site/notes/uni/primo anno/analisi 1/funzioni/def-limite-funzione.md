---
{"dg-publish":true,"permalink":"/uni/primo-anno/analisi-1/funzioni/def-limite-funzione/","tags":["uni","math"]}
---

sia $f:\mathbb{R} \rightarrow\mathbb{R}$ di dominio $D(f)$ e sia $x_0$ un [[uni/primo anno/analisi 1/basi funzioni/definizioni/def-punti-accumulazione-and-others\|punto di accumulazione]] per l'insieme $D(f)$, diciamo che $f$ ammette limite $l \in \mathbb{R}$ per $x \rightarrow x_0$ se 
$$\forall u(l) \ \exists u(x_0) : \text{if} \ x \in\dot{u}(x_0)\cap D(f)$$
$$\implies f(x) \in u(l)$$
$$\lim_{x\rightarrow x_0} f(x) = l$$
### esempio importante
$$x_0,l \in \mathbb{R}$$
$$u(l) = (l-\varepsilon,l+\varepsilon),\ \  \dot{u}(x_0) = (x_0-\delta, x_0)\cap(x_0, x_0+\delta)$$
$$\forall\varepsilon > 0 \ \exists \ \delta >0 : \text{se } x \in D(f) \land 0 < |x-x_0|<\delta$$
$$\implies |f(x) - l| < \varepsilon$$
### osservazione 1
scriviamo $\dot{u}(x_0)$ ([[uni/primo anno/analisi 1/basi funzioni/definizioni/def-intorni#intorno bucato\|intorno bucato]]) perché non ci interessa cosa fa la funzione nel punto $x_0$.
### osservazione 2
questa definizione ci permette di racchiudere tutti i casi di limite poiché:
- $x_0$ 
	- $\in\mathbb{R}$
	- $+\infty$
	- $-\infty$
- $l$
	- $\in\mathbb{R}$
	- $+\infty$
	- $-\infty$
questo perché il Pata ha definito i punti di accumulazione in [[uni/primo anno/analisi 1/successioni/definizioni/def-R-esteso\|R esteso]].
### osservazione 3
l'unico punto di accumulazione che una successione può avere è $+\infty$, motivo per cui si fanno sempre i limiti per $n \rightarrow +\infty$ e diventa sottointeso.
