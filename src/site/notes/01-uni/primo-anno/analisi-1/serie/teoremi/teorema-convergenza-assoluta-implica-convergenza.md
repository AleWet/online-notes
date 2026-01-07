---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/analisi-1/serie/teoremi/teorema-convergenza-assoluta-implica-convergenza/","tags":["math","uni"]}
---

se $\begin{equation} {\textstyle \sum^{}}a_n\end{equation}$ [[01-uni/primo-anno/analisi-1/serie/definizioni/def-convergenza-assoluta\|converge assolutamente]] allora [[01-uni/primo-anno/analisi-1/serie/definizioni/def-serie\|converge]] . Questo è di solito molto utile perché la serie dei valori assoluti è a termini positivi e puoi applicare gli asintotici.
### osservazioni
$\exists$ serie che convergono ma non convergono assolutamente, un esempio è:
$$\sum \frac{(-)^n}{n}$$
##### ==dim== (1)
$$\sum |a_n| \text{ converge per ipotesi}$$
$$0 \le\sum (|a_n| - a_n) \le 2\sum|a_n|$$
questo per il [[01-uni/primo-anno/analisi-1/serie/definizioni/def-serie#proprietà\|operazioni tra limiti]]:
$$\sum (|a_n| - a_n) \text{ (converge) }+ \sum -|a_n| \text{ (converge) }$$
$$ = \sum a_n \text{ converge per operazioni tra limiti}$$

