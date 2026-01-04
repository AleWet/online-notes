---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/analisi-1/funzioni/teoremi/teoremi-integrali-riemann/teorema-delta-somme-superiori-inferiori-tbd/","tags":["math","uni"]}
---

sia $f \in R(a,b)$ (dove con $R(a,b)$ intendo [[01-uni/primo anno/analisi 1/funzioni/definizioni/def-integrale-Riemann-TBF\|questo]]) allora 
$$\omega _{n}(f) := S_{n} - s_{n}$$
$$f \in R(a,b) \iff \omega_{n} \to 0$$
### osservazione preliminare
è sempre vero che $s_{n} \to s$ e che $S_{n} \to S$ anche se non convergono allo stesso limite.
### dim $\Rightarrow$
se $f \in R(a,b)$ allora posso dire che :
$$s_{n}, S_{n} \to S \text{ che è l'integrale di } f $$
$$\implies w_{n} = S_{n}-s_{n} \to S - S = 0$$
### dim $\Leftarrow$
suppongo che $\omega_{n} \to 0$ allora :
$$s_{n} \leq s \leq S \leq S_{n}$$
$$0\leq s - s_{n} \leq S-s_{n} \leq S_{n}-s_{n}$$
$$\implies 0\leq s - s_{n} \leq S-s_{n} \leq \omega_{n}$$
$$s-s_{n} \to 0, \ \omega_{n} \to 0 \implies S-s_{n} \to 0$$
usando il [[01-uni/primo anno/analisi 1/successioni/teoremi/teorema-del-confronto\|01-uni/primo anno/analisi 1/successioni/teoremi/teorema-del-confronto]] 
$$s_{n} \to S, s_{n} \to s \implies S = s$$ per [[01-uni/primo anno/analisi 1/successioni/teoremi/teorema-unicità-del-limite\|01-uni/primo anno/analisi 1/successioni/teoremi/teorema-unicità-del-limite]].
