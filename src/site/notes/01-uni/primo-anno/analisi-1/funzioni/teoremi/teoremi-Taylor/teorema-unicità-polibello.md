---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/analisi-1/funzioni/teoremi/teoremi-taylor/teorema-unicita-polibello/","tags":["math","uni"]}
---

$\exists$ al più un singolo [[01-uni/primo-anno/analisi-1/funzioni/teoremi/teoremi-Taylor/teorema-Taylor-Peano#osservazione 3\|polibello]] $P(x)$ di grado $n$ per una singola $f$.
### corollario
se $f$ è derivabile $n$ volte in $x_{0} \implies \exists$ [[01-uni/primo anno/analisi 1/funzioni/definizioni/def-polinomio-Taylor\|politaylor]] di grado $n$ per $f$ ed esso è unico.
### dim
siano per assurdo $P(x), Q(x)$ due polibelli di grado $n$ per la funzione $f$ in $x_0 = 0$ (per semplicità) allora:
$$\lim_{ x \to 0 } \frac{f(x)-P(x)}{x^n} = 0$$

$$\lim_{ x \to 0 } \frac{f(x)-Q(x)}{x^n} = 0$$
$$\implies \lim_{ x \to 0 } \frac{P(x)-Q(x)}{x^n} = 0 $$
$$\text{ma } R(x):=P(x)-Q(x) \text{ ha grado } \le n$$
$$\implies se \lim_{ x \to 0 } \frac{R(x)}{x^n} = 0 \implies R(x) = 0 \implies P(x) = Q(x)$$
quest'ultimo passaggio è intuitivo se ci pensi, l'unico modo che un polinomio di grado $\le n$ di andare a $0$ quando lo dividi per $x^n$ è se il polinomio è nullo, se no ti farebbe o una costante (se è di grado $=n$) o $\pm \infty$ perché ti andrebbe a 0 più lentamente di $x^n$ e risulterebbe della forma $\frac{1}{x^\alpha}$.
