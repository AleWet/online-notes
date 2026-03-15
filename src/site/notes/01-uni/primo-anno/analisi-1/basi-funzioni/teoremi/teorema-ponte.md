---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/analisi-1/basi-funzioni/teoremi/teorema-ponte/","tags":["math","uni"],"updated":"2026-01-10T13:24:09.430+01:00"}
---

### tesi
$$\lim_{x \rightarrow x_0} f(x) \iff s\lim_{x \rightarrow x_0} f(x)$$
ovvero che [[01-uni/primo-anno/analisi-1/funzioni/definizioni/def-limite-successionale\|il limite successionale]] e il [[01-uni/primo-anno/analisi-1/funzioni/definizioni/def-limite-funzione\|limite "normale"]] sono equivalenti, basta che sostituisci alla $x$ una generica successione $X_n : X_n \rightarrow x_0$ e puoi calcolare il limite.
### dim
Assumi sempre che $x_0$ è un punto di accumulazione per $D(f)$ se no il limite non è implementabile.
### $\Rightarrow$
prendo una generica $a_n \ne x_0$ con $a_n \rightarrow x_0$ e voglio dimostrare che $f(a_n) \rightarrow l$ :
$$\forall u(l), \ f(a_n) \in u(l) \text{ definitivamente}$$
poiché se $a_n \rightarrow x_0 \implies a_n \in \dot{u}(x_0)$ definitivamente ([[01-uni/primo-anno/analisi-1/basi-funzioni/definizioni/def-intorni#osservazione importante\|osservazione cuoricino]])
e di conseguenza $f(a_n) \in u(l)$ poiché ogni elemento della successione $a_n$ $\in u(x_0)$ definitivamente.
### $\Leftarrow$
voglio dimostrare che $s\lim f(x) = l \implies \lim f(x) = l$ quindi uso la seguente cosa : 
se dimostro che negando la tesi nego anche l'ipotesi ho vinto, ovvero che
$$\lim f(x) \ne l \implies s\lim f(x) \ne l$$
quindi prendo la definizione di limite di funzione e la nego :
$$\forall u(l) \ \exists u(x_0) : \text{ se } x \in D(f) \cap \dot{u}(x_0) \implies f(x) \in u(l)$$
$$\exists u(l) \  \forall u(x_0) \ \exists x \in D(f) \cap \dot{u}(x_0) \text{ ma } f(x) \not\in u(l)$$
qui la dimostrazione si divide in due casi : 
### $x_0 \in \mathbb{R}$
$$u(x_0) = (x_0-\delta, x_0+\delta)$$
$$\forall n \text{ scelgo l'intorno } (x_0-\frac{1}{n}, x_0+\frac{1}{n})$$
$$\forall n \ \exists u(l) \text{ e } a_n \ne x_0 , a_n \in D(f) : |a_n-x_0|< \frac{1}{n}$$
$$\implies a_n \rightarrow x_0 \implies a_n \in u(x_0) \text{ ma } f(a_n) \not \in u(l)$$
$$\implies f(a_n) \not\rightarrow l \ \ \ \ \ \ \square$$
In pratica costruisci una successione $(a_n \to x_0)$ scegliendo, $\forall n$, un punto

$$
a_n \in \left(x_0 - \frac{1}{n},\, x_0 + \frac{1}{n}\right)
\quad\text{tale che}\quad
|f(a_n) - l| \ge \varepsilon .
$$

Poiché ogni termine della successione viola la condizione $|f(x) - l| < \varepsilon$,
si ottiene che $f(a_n) \not\to l$, e quindi si nega anche il limite successionale. Crei quindi la successione di punti che "fanno fallire il limite", per ogni intervallo $(x_0- \frac{1}{n}, x_0+ \frac{1}{n})$ prendi il punto $x$ tale per cui $|f(x) - l| \ge \varepsilon$ e lo associ ad una etichetta $n$ e sai che questa cosa vale $\forall n$ perché è nella negazione di limite per le funzioni che un punto $x$ così esiste $\forall u(x)$. 
### $x_0 \not\in \mathbb{R}$
assumo che $x_0 = +\infty$, il caso con $x_0 = -\infty$ è equivalente :
$$u(x_0) = (M, +\infty)$$
$$\forall n \text{ scelgo l'intorno } (n, +\infty)$$
$$\forall n \ \exists u(l) \text{ e } a_n \ne x_0 \in D(f) : a_n > n$$
$$\implies a_n \rightarrow x_0 \implies a_n \in u(x_0) \text{ ma } f(a_n) \not\in u(l)$$
$$\implies f(a_n) \not\rightarrow l \ \ \ \ \ \square$$
