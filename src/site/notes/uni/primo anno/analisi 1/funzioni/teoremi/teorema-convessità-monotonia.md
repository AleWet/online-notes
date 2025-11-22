---
{"dg-publish":true,"permalink":"/uni/primo-anno/analisi-1/funzioni/teoremi/teorema-convessita-monotonia/","tags":["math","uni"]}
---

sia $f:[a,b] \to \mathbb{R}$ [[uni/primo anno/analisi 1/funzioni/definizioni/def-derivata#derivabilità\|derivabile]] su tutto $[a,b]$ allora $f$ è [[uni/primo anno/analisi 1/funzioni/definizioni/def-funzione-convessa\|convessa]] $\iff f'(x)$ è crescente
### osservazione
la parte più interessante di questa relazione è $\Leftarrow$ poiché la derivata ci sta dando informazioni riguardo la funzione ed è infatti l'unica parte che abbiamo dimostrato.
### dim $\Leftarrow$
$f'$ è crescente allora la tesi diventa che $f$ vive sopra la retta tangente in ogni punto per ogni retta:
fissiamo $x_0$ qualsiasi e mostriamo che $\forall x > x_0, f(x) \ge r_{x_0}(x)$, la dimostrazione $\forall x < x_0$ è analoga.
applico il [[uni/primo anno/analisi 1/funzioni/teoremi/teorema-Lagrange\|teorema di Lagrange]] all'intervallo $[x_0,x]$ ($f$ è derivabile e continua in quell'intervallo, etc)
$$\implies \exists y \in (x_0,x) : f(x)-f(x_0) = f'(y)(x-x_0)$$
$$f'(y) \ge f'(x_0) \text{ poiché f' è crescente per ipotesi}$$
$$f(x) = f'(y)(x-x_0)+f(x_0) \ge f(x_0)(x-x_0)+f(x_0)$$
$$\implies f(x) \ge f'(x_0)(x-x_0)+f(x_0) = r_{x_0}(x) \ \ \ \ \forall x > x_0$$
dove $r_{x_0}(x)$ è la retta tangente al grafico di $f$ nel punto $x_0$. Fatto lo stesso ragionamento $\forall x < x_0$
puoi usare il [[uni/primo anno/analisi 1/funzioni/teoremi/teorema-convessa-maggiore-tangente\|seguente teorema]] che ti dice che se una funzione sta sempre sopra tutte le proprie tangenti allora è convessa.
### dim $\Rightarrow$
la dimostrazione la trovi sul [[Derivata (1).pdf#page=28|pdf del Pata]] ma non l'abbiamo fatta a lezione.
