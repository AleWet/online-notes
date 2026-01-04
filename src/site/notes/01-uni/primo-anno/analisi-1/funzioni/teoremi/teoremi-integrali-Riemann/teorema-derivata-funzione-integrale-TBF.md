---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/analisi-1/funzioni/teoremi/teoremi-integrali-riemann/teorema-derivata-funzione-integrale-tbf/","tags":["math","uni"]}
---

sia $f:[a,b] \to \mathbb{R}$, sia $I(x)$ la [[01-uni/primo anno/analisi 1/funzioni/definizioni/def-funzione-integrale\|funzione integrale]] di $f$ allora se $f$ è [[01-uni/primo anno/analisi 1/funzioni/definizioni/def-continuità\|continua]]  in $x_{0}$ si ha che 
$$I(x) \text{ è derivabile in } x_{0} \in [a,b]$$
$$I'(x_{0}) = f(x_{0})$$
### corollario importante
se $f$ è continua su tutto $[a,b]$ avrò che :
$$\forall x \in [a,b], I'(x) = f(x)$$
il che è la definizione di [[01-uni/primo anno/analisi 1/funzioni/definizioni/def-primitiva\|primitiva]] da cui $I$ diventa una primitiva di $f$. Mettendo quindi insieme questo teorema e [[01-uni/primo anno/analisi 1/funzioni/teoremi/teoremi funzioni continue/teorema-continua-integrabile\|questo teorema]] si ha che:
$$\text{ se } f \ \text{ è continua } \implies f \in R_{P}(a,b)$$
### osservazione del corollario
non è vero che se $f \in R_{P}(a,b) \implies f$ è continua, un esempio è 
$$F:[0,1] \to \mathbb{R}$$
$$F(x) = \begin{cases}
x^2\sin\left( \frac{1}{x} \right) & x \ne {0} \\ \\
0  & x=0
\end{cases}$$
$$f(x) = \begin{cases}
2x\sin\left( \frac{1}{x} \right) -\cos\left( \frac{1}{x} \right)  & x\ne 0 \\ \\
0 & x=0
\end{cases}$$
$f$ ha un solo punto di [[01-uni/primo anno/analisi 1/funzioni/definizioni/def-punti-discontinuità#discontinuità di II specie\|discontinuità di seconda specie]] e altrove è continua quindi [[01-uni/primo-anno/analisi-1/funzioni/teoremi/teoremi-integrali-Riemann/teorema-finite-discontinuità-integrabile-TBF\|è integrabile]], inoltre $f$ ammette primitiva (la $F$) e quindi $f \in R_P(a,b)$.
### dim TBD
