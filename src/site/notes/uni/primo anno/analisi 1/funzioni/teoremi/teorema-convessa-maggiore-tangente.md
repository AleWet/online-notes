---
{"dg-publish":true,"permalink":"/uni/primo-anno/analisi-1/funzioni/teoremi/teorema-convessa-maggiore-tangente/","tags":["math","uni"]}
---

# $\Rightarrow$
sia $f:[a,b] \to \mathbb{R}$ una funzione [[uni/primo anno/analisi 1/funzioni/definizioni/def-funzione-convessa\|convessa]] e assumendo che $f$ sia [[uni/primo anno/analisi 1/funzioni/definizioni/def-derivata#derivabilità\|derivabile]] in $x_0 \in[a,b]$
$$\implies f(x) \ge r_{tangente}(x) \ \forall x \in [a,b]$$
dove $r_{tangente}$ è la retta tangente a $f$ in $x_0 ,\  r_{\text{tangente}} = f'(x_0)(x-x_0)+f(x_0)$ 
### osservazione
La retta tangente sta quindi sotto *tutto* il grafico della funzione se la funzione è convessa e questo vale per ogni punto $x_0$ dell'intervallo di convessità.
### dim TBD
___
# $\Leftarrow$ 
sia $f : [a,b] \to \mathbb{R}$ tale che $f$ è [[uni/primo anno/analisi 1/funzioni/definizioni/def-derivata#derivabilità\|derivabile]] in $[a,b]$ e si ha che:
$$\forall x_0 \in [a,b], \ f(x) \ge r_{x_0}(x)$$
dove $r_{x_0}$ è la tangente al grafico di $f$ in $x_0$ $(r_{x_0} = f(x_0) + f'(x_0)(x-x_0))$
$$\implies f(x) \text{ è convessa in }[a,b]$$
### osservazione importante
mettendo insieme il teorema precedente si ha che se $f$ è derivabile in $[a,b]$ allora:
$$f \text{ è convessa } \iff f\text{  sta sopra tutte le sue rette tangenti in } [a,b]$$
### dim TBD
