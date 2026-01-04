---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/analisi-1/serie/definizioni/def-serie-armonica-generalizzata/","tags":["math","uni"]}
---

definisco la serie armonica generalizzata come:
$$\sum_{n=1}^{+\infty} \frac{1}{n^a}$$
di conseguenza essa è a [[01-uni/primo-anno/analisi-1/serie/definizioni/def-serie-termini-positivi\|a termini positivi]] allora è regolare e si comporta nel seguente metodo:
- $a>1$ converge
- $a \le 1$ diverge
naturalmente il caso $a = 1$ coincide con la serie armonica.
### osservazione
per $a>1$ so che le serie convergono perché posso dire la seguente cosa:
$$\begin{equation}{\sum} \frac{1}{n^2}\end{equation} < \sum \frac{2}{n(n+1)}$$
dove il termine a destra è $2$* la [[01-uni/primo-anno/analisi-1/serie/definizioni/def-serie-telescopica\|serie di mengoli]] e per il [[01-uni/primo anno/analisi 1/serie/teoremi/teorema-confronto-serie\|01-uni/primo anno/analisi 1/serie/teoremi/teorema-confronto-serie]] allora la serie a sinistra converge.
### Eulero-Mascheroni
$$\sum_1^\infty \frac{1}{n} \sim \log(n)$$
$$S_n - \log(n) \rightarrow \gamma$$
dove $\gamma =$ costante di Eulero-Mascheroni $\simeq0,5772 ...$
### dim
dimostro che la serie armonica $\sum \frac{1}{n} \rightarrow +\infty$:
$$\text{P.A.} \sum \frac{1}{n} \rightarrow l \in \mathbb{R}$$
$$S_n = \frac{1}{1} + \frac{1}{2} + \frac{1}{3} + ... + \frac{1}{n}$$
$$S_{2n} = \frac{1}{1} + \frac{1}{2} + ... + \frac{1}{2n-1} + \frac{1}{2n}$$
$$S_n ,S_{2n} \rightarrow l \text{ (tutte le sottosuccessioni convergono allo stesso limite)}$$
$$S_{2n}-S_n \rightarrow0$$
$$S_{2n} - S_{n} = \frac{1}{n+1}+\frac{1}{n+2}+\frac{1}{n+3}+...+\frac{1}{2n} \rightarrow 0$$
$$S_{2n}-S_n = \frac{1}{n+1} + \frac{1}{n+2} + ... +\frac{1}{2n} \ge \frac{1}{2n} + \frac{1}{2n}+ ... + \frac{1}{2n} = (2n-n) * \frac{1}{2n} = \frac{1}{2}$$
$$\text{qui arrivi all'assurdo :  } S_{2n}-S_n \rightarrow0 \land S_{2n} - S_n \ge \frac{1}{2} \forall n \ \ \ \ \ \square$$

