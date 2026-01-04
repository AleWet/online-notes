---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/analisi-1/funzioni/teoremi/teoremi-funzione-derivata/teorema-derivata-darboux/","tags":["math","uni"]}
---

sia $f : I \to \mathbb{R}$ [[01-uni/primo anno/analisi 1/funzioni/definizioni/def-derivata\|derivabile]] in $I$ allora la [[01-uni/primo anno/analisi 1/funzioni/definizioni/def-derivata#funzione derivata\|funzione derivata]] $f'$ ha la proprietà di [[01-uni/primo anno/analisi 1/funzioni/definizioni/def-Darboux\|Darboux]].
### dim
==sui miei appunti ho scritto che questa dimostrazione non verrà chiesta all'esame==
siano $x,y \in I, x<y :$
1) se $f'(x) = f'(y)$ la derivata assume già tutti i valori compresi tra $f'(x)$ e $f'(y)$
2) se $f'(x) \ne f'(y)$ assumo allora $f'(x) < f'(y)$ arbitrariamente e sia $\gamma :$
$$f'(x) < \gamma < f'(y)$$
$$\text{voglio dimostrare che } \exists z \in (x,y) : f'(z) = \gamma$$
$$g:[x,y] \to \mathbb{R}, \ \ g(t) = f(t)-\gamma t$$
$$g\text{ è derivabile in } I \text{ poiché somma di funzioni derivabili, } \ g'(t) = f'(t)-\gamma$$
$$g\text{ allora è anche continua e assume massimo e minimo in } I \tag{*}$$
$$g'(x) = f'(x)-\gamma < 0$$
$$g'(y) = f'(y)-\gamma >0$$
$$\implies g \text{ non assume minimo in x e massimo in y, se no } g'(y) = g'(x) = 0$$
$$\implies \exists z \in (a,b) : z \text{ è il massimo di }g \implies g'(z) = 0 \tag{**}$$
$$\implies g'(z) = f'(z) -\gamma \implies f'(z) = \gamma \ \ \ \square$$

$(*)$ questo per il [[01-uni/primo anno/analisi 1/funzioni/teoremi/teoremi funzioni continue/teorema-Weierstrass\|01-uni/primo anno/analisi 1/funzioni/teoremi/teoremi funzioni continue/teorema-Weierstrass]].
$(**)$ questo per il [[01-uni/primo-anno/analisi-1/funzioni/teoremi/teoremi-funzione-derivata/teorema-Fermat\|teorema-Fermat]].