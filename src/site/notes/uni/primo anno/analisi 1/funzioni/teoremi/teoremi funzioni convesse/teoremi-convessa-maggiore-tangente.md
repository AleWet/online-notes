---
{"dg-publish":true,"permalink":"/uni/primo-anno/analisi-1/funzioni/teoremi/teoremi-funzioni-convesse/teoremi-convessa-maggiore-tangente/","tags":["math","uni"]}
---

# teorema 1 $(\Rightarrow)$
sia $f:[a,b] \to \mathbb{R}$ una funzione [[uni/primo anno/analisi 1/funzioni/definizioni/def-funzione-convessa\|convessa]] e assumendo che $f$ sia [[uni/primo anno/analisi 1/funzioni/definizioni/def-derivata#derivabilità\|derivabile]] in $x_0 \in[a,b]$
$$\implies f(x) \ge r_{tangente}(x) \ \forall x \in [a,b]$$
dove $r_{tangente}$ è la retta tangente a $f$ in $x_0 ,\  r_{\text{tangente}} = f'(x_0)(x-x_0)+f(x_0)$ 
### osservazione
La retta tangente sta quindi sotto *tutto* il grafico della funzione se la funzione è convessa e questo vale per ogni punto $x_0$ in cui la funzione ammette derivata.
___
# teorema 2 $(\Leftarrow)$ 
sia $f : [a,b] \to \mathbb{R}$ tale che $f$ è [[uni/primo anno/analisi 1/funzioni/definizioni/def-derivata#derivabilità\|derivabile]] in $[a,b]$ e si ha che:
$$\forall x_0 \in [a,b], \ f(x) \ge r_{x_0}(x)$$
dove $r_{x_0}$ è la tangente al grafico di $f$ in $x_0$ $(r_{x_0} = f(x_0) + f'(x_0)(x-x_0))$
$$\implies f(x) \text{ è convessa in }[a,b]$$
___
# teorema 3 ($\iff$)
mettendo insieme il teorema precedente si ha che se $f$ è derivabile in $[a,b]$ allora:
$$f \text{ è convessa } \iff f\text{  sta sopra tutte le sue rette tangenti in } [a,b]$$
___
# dimostrazioni
### dim 1
quello che voglio dimostrare è che preso $x_{0} \in [a,b)$ per ogni punto $x > x_{0}$:
$$f(x) \geq f(x_{0}) + f'(x_{0})(x-x_{0}) \ \ \forall x \in [a,b]$$
dove $[a,b]$ è l'intervallo di convessità e $x_0$ è il punto di derivabilità e quindi :
$$r_{tan \ x_{0} }(x) = f(x_{0})+f'(x)(x-x_{0})$$
la dimostrazione per ogni punto $x < x_{0}$ è equivalente. Consideriamo i tre punti con $h>0$ sufficientemente piccolo :
$$x_{0} < x_{0}+h < x$$
$$x_{0}+h = \lambda x_{0} + (1-\lambda)x$$
$$\text{ dove } \lambda = \frac{{x-x_{0}-h}}{x-x_{0}}$$

e uso la definizione di convessità:
$$f(x_{0}+h) \leq \lambda f(x_{0}) + (1-\lambda)f(x)$$
$$f(x_{0}+h)-f(x_{0}) \leq \lambda f(x_{0})-f(x_{0})+(1-\lambda)f(x)$$
$$f(x_{0}+h)-f(x_{0}) \leq (1-\lambda)(f(x)-f(x_{0}))$$
a questo punto esplicito $\lambda$ :
$$f(x_{0}+h)-f(x_{0}) \leq \left( \frac{h}{x-x_{0}} \right)(f(x)-f(x_{0}))$$
$$\frac{{f(x_{0}+h)-f(x_{0})}}{h} \leq \frac{{f(x)-f(x_{0})}}{x-x_{0}}$$
usando il [[uni/primo anno/analisi 1/successioni/teoremi/teorema-della-permanenza-del-segno\|teorema-della-permanenza-del-segno]] con $h \to 0^+$ ottengo che:
$$\lim_{ h \to 0^+ } R(f,x_{0},h) \leq \frac{{f(x)-f(x_{0})}}{x-x_{0}}$$
$$\implies f'(x_{0}) \leq \frac{{f(x)-f(x_{0})}}{x-x_{0}}$$
$$\implies f'(x_{0})(x-x_{0}) + f(x_{0}) \leq f(x) \ \ \  \ \  \square $$
___
### dim 2 
adesso devo dimostrare il contrario, ovvero che se una funzione è derivabile in $[a,b]$ e essa si trova sopra la propria retta tangente **di ogni punto** di $[a,b]$ allora essa è convessa.
Presi due punti $x,y\in [a,b]$ e fissato $x_{0} \in (x,y)$ posso scrivere che :
$$x_{0} = \lambda x + (1-\lambda)y$$
visto che $x \leq x_{0} \leq y$, allora applico l'ipotesi a $x$ e $y$ : 
$$f(x) \geq f'(x_{0})(x-x_{0}) + f(x_{0})$$
$$f(y) \geq f'(x_{0})(y-x_{0})+f(x_{0})$$
a questo punto moltiplico la prima per $\lambda$ e la seconda per $(1-\lambda)$ e poi le sommo ottenendo a sinistra esattamente quello che voglio e a destra roba che sembra brutta : 
$$\lambda f(x) + (1-\lambda)f(y) \geq f'(x_{0})[\lambda(x-x_{0})+(1-\lambda)(y-x_{0})] + f(x_{0})$$
noto che:
$$\lambda(x-x_{0})+(1-\lambda)(y-x_{0})= \lambda x-\lambda x_{0} +y-\lambda y-x_{0}+\lambda x_{0}$$
$$= \lambda x+y-\lambda y-x_{0} = \lambda x+(1-\lambda)y-x_{0}$$
e qui uso il fatto che ho messo $x_{0}$ tra $x$ e $y$ per ipotesi per poterlo scrivere come combinazione convessa di $x,y$ allora:
$$\lambda x + (1-\lambda)y - [\lambda x + (1-\lambda)y] = 0$$
allora sostituisco nell'equazione sopra e ottengo:
$$\lambda f(x) + (1-\lambda)f(y) \geq f(x_{0}) = f(\lambda x + (1-\lambda )y)$$
___
### dim 3 TBD
la tre è una semplice combinazione dei due teoremi qui sopra.

(per più info e meno passaggi guarda il [[Derivata (1).pdf|pdf del pata]], lì mette più dettagli nelle ipotesi perché negli estremi $a,b$ dovresti essere più preciso)