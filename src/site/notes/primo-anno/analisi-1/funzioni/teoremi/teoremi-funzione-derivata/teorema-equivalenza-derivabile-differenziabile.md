---
{"dg-publish":true,"permalink":"/primo-anno/analisi-1/funzioni/teoremi/teoremi-funzione-derivata/teorema-equivalenza-derivabile-differenziabile/","tags":["math","uni"],"updated":"2026-02-24T15:52:00.483+01:00"}
---

$f$ è [[primo-anno/analisi-1/funzioni/definizioni/def-differenziabilità\|differenziabile]] in $x_0 \iff f$ è [[primo-anno/analisi-1/funzioni/definizioni/def-derivata\|derivabile]] in $x_0$, e in tal caso $L$ è esattamente $f'(x_0)$.
### osservazione
in pratica la derivata esprime come la funzione si comporta lungo una *direzione* mentre il differenziale esprime come si comporta una funzione nell'[[primo-anno/analisi-1/basi-funzioni/definizioni/def-intorni\|intorno]] collassano sulla stessa definizione. Questo non sarebbe lo stesso in altre dimensioni come $\mathbb{R}^2$. 
### dim $\Rightarrow$
$$f(x) = f(x_{0})+L(x-x_{0}) +o(x-x_{0}) \ \  \text{ where } L \in \mathbb{R}$$
$$\iff f(x)-f(x_{0})= L(x-x_{0}) + o(x-x_{0})$$
$$\iff \frac{{f(x)-f(x_{0})}}{x-x_{0}} = L + \frac{o(x-x_{0})}{x-x_{0}}$$
$$\implies \lim_{ x \to x_{0} } \frac{f(x)-f(x_{0})}{x-x_{0}} = L + \lim_{ x \to x_{0} } \frac{o(x-x_{0})}{x-x_{0}}$$
$$\implies f'(x_{0}) = L \in \mathbb{R}$$
### dim $\Leftarrow$
$$\lim_{ h \to 0 } R(f,x_{0},h) = f'(x_{0}) \in \mathbb{R}$$
$$\frac{{f(x_{0}+h) - f(x_{0})}}{h} = L + \omega(h) \ \ \ \text{where } \omega(h) \to 0 \text{ if } h \to 0$$
$$f(x_{0}+h)- f(x_{0}) = hL + h\omega(h)$$
$$\iff f(x)=f(x_{0})+L(x-x_{0})+o(x-x_{0})$$

