---
{"dg-publish":true,"permalink":"/primo-anno/analisi-1/funzioni/teoremi/teoremi-funzioni-convesse/teorema-convessita-derivata-prima/","tags":["math","uni"],"updated":"2026-02-24T15:52:00.483+01:00"}
---

eoremsia $f:[a,b] \to \mathbb{R}$ [[primo-anno/analisi-1/funzioni/definizioni/def-funzione-convessa\|convessa]] $\iff f'(x)$ è crescente
### osservazione
la parte più interessante di questa relazione è $\Leftarrow$ poiché la derivata ci sta dando informazioni riguardo la funzione ed è infatti l'unica parte che abbiamo dimostrato.
### dim $\Leftarrow$
Parto per ipotesi dal fatto che $f'(x)$ è crescente e voglio dimostrare che $f$ è convessa, per fare ciò dimostro che $f(x)$ è sopra tutte le sue rette tangenti in $[a,b]$ e grazie a [[primo-anno/analisi-1/funzioni/teoremi/teoremi-funzione-derivata/teorema-Lagrange-(tbf)\|teorema di Lagrange]] all'intervallo $[x_0,x]$ ($f$ è derivabile e continua in quell'intervallo, posso dire che è continua [[primo-anno/analisi-1/funzioni/teoremi/teoremi-funzioni-convesse/teorema-convessa-continua\|grazie a questo teorema]])
$$\implies \exists y \in (x_0,x) : f(x)-f(x_0) = f'(y)(x-x_0)$$
$$f(y)' \ge f(x_0)' \text{ poiché f' è crescente per ipotesi}$$
$$f(x) = f'(y)(x-x_0)+f(x_0) \ge f(x_0)'(x-x_0)+f(x_0)$$
$$\implies f(x) \ge f'(x_0)(x-x_0)+f(x_0) = r_{x_0}(x) \ \ \ \ \forall x > x_0$$
dove $r_{x_0}(x)$ è la retta tangente al grafico di $f$ nel punto $x_0$. Fatto lo stesso ragionamento $\forall x < x_0$
puoi usare il [[primo-anno/analisi-1/funzioni/teoremi/teoremi-funzioni-convesse/teoremi-convessa-maggiore-tangente\|seguente teorema]] che ti dice che se una funzione sta sempre sopra tutte le proprie tangenti allora è convessa.
### dim $\Rightarrow$
la dimostrazione la trovi sul [[PDF-Derivata-Pata.pdf#page=28|pdf del Pata]] ma non l'abbiamo fatta a lezione.
