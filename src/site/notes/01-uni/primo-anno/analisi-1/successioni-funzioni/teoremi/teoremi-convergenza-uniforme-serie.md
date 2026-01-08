---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/analisi-1/successioni-funzioni/teoremi/teoremi-convergenza-uniforme-serie/","tags":["math","uni"]}
---

uguali ai teoremi per le [[01-uni/primo-anno/analisi-1/successioni-funzioni/teoremi/teoremi-convergenza-uniforme-successioni\|successioni di funzioni]] ma applicati alle [[01-uni/primo-anno/analisi-1/successioni-funzioni/definizioni/def-serie-di-funzioni\|serie]].
### teorema 1 continuità
se ogni $f_{n}:I \to \mathbb{R}$ è [[01-uni/primo-anno/analisi-1/funzioni/definizioni/def-continuità\|continua]] e $s_{n} \xrightarrow{u} S$ si ha che:
$$\sum_{n=1}^\infty f_{n}(x) = S(x) \ \text{ è continua}$$
### teorema 2 integrabilità
se ogni $f_{n}:[a,b] \to \mathbb{R} \in R(a,b)$ e $s_n \xrightarrow{u} S$ si ha che:
$$\sum_{n=1}^\infty f_{n}(x) = S(x) \in R(a,b)$$
$$\int_{a}^b \sum_{n=1}^\infty f_{n}(x) = \sum_{n=1}^\infty \int_{a}^bf_{n}(x) $$
in pratica puoi portare dentro fuori l'operazione di integrale.
### teorema 3 derivabilità
sia $f_{n}:[a,b] \to \mathbb{R}$  [[01-uni/primo-anno/analisi-1/funzioni/definizioni/def-derivata#derivabilità\|derivabile]] allora se:
- $\exists x_{0} \in [a,b] : \sum_{n=1}^\infty f_{n}(x_{0}) = l \in \mathbb{R}$
- $\sum f_{n}' \xrightarrow{u} g$
$$\implies \sum f_{n} \xrightarrow{u} S \ \ \ \ \ \ \ \ \ \ $$
$$\implies\left( \sum_{n=1}^\infty f_{n}(x) \right)' = \sum_{n=1}^\infty f_{n}'(x)$$
ovvero che $S$ è derivabile
___
### dimostrazioni
questi teoremi non sono stati dimostrati.
