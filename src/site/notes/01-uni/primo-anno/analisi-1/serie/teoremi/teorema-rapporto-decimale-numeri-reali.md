---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/analisi-1/serie/teoremi/teorema-rapporto-decimale-numeri-reali/","tags":["math","uni"]}
---

la tesi è che ogni $\alpha \in \mathbb{R}$ può essere rappresentato come una [[01-uni/primo anno/analisi 1/serie/definizioni/def-serie\|serie]] :
$$\alpha \in \mathbb{R} = 0,a_1a_2a_3 ...$$
$$\text{chiamo  } \alpha_n \text{ il troncato di } \alpha \text{ alla posizione } n$$
$$\alpha_n = \frac{a_1}{10} + \frac{a_2}{100} + ... + \frac{a_n}{10^n}$$
$$\alpha_n = \sum_{k=1}^n \frac{a_k}{10^k}$$
questa può essere vista come successione delle somme parziali della serie:
$$\sum_{n=1}^\infty \frac{a_n}{10^n}$$
questa serie converge per [[01-uni/primo-anno/analisi-1/serie/teoremi/teorema-confronto-serie\|confronto]] :
$$0 \le \frac{a_n}{10^n} \le \frac{9}{10^n} = 9*\frac{1}{10^n}$$
dove naturalmente $\frac{1}{10^n}$ è il termine gen. di una [[01-uni/primo anno/analisi 1/serie/definizioni/def-serie-geometrica\|serie geometrica]] di ragione $\frac{1}{10}\le1$ che converge.
(ogni cifra $a_n$ è $\le9$ naturalmente). quindi posso scrivere la seguente disuguaglianza : 
$$\alpha_n \le \alpha \in \mathbb{R} \le \alpha_n + \frac{1}{10^n}$$
$$ \text{esempio della disuguaglianza : }0.193942 ... \le 0.193950$$
$$\alpha_n , \ \alpha_n + \frac{1}{10^n} \rightarrow l \implies \alpha = l$$
$$\implies \alpha = l = \sum_{n=1}^\infty \frac{a_n}{10^n}$$
