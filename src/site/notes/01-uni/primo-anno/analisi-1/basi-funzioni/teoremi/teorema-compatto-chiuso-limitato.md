---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/analisi-1/basi-funzioni/teoremi/teorema-compatto-chiuso-limitato/","tags":["math","uni"]}
---

[[01-uni/primo-anno/analisi-1/basi-funzioni/definizioni/def-insiemi-aperti-chiusi#insieme chiuso\|chiuso]] e limitato
### dim $\Rightarrow$ 
##### chiuso
Sia $x$ un [[01-uni/primo-anno/analisi-1/successioni/teoremi/teorema-unicità-del-limite\|teorema-unicità-del-limite]]. Ciò implica che tutti i punti di accumulazione $x$ sono contenuti in A.
##### limitato
Per assurdo assumi che $\exists x_n \in A : x_n \to +\infty$ allora hai che $\forall x_{n_k} \ di \ x_n, x_{n_k} \to +\infty$ che è contro le ipotesi di compattezza. Di conseguenza l'unico modo per non far esistere una successione $x_n$ t.c. $x_n \to +\infty$ è di avere un insieme LIMITATO
$$\implies A \text{ è chiuso e limitato}$$
### dim $\Leftarrow$ o Heine-Borel
sia $A$ un insieme chiuso e limitato, allora sia $x_n \in A$ e poiché $A$ è limitato, $x_n$ è limitata
$$\implies \exists x \in \mathbb{R} : x_{n_k} \to x$$
per il [[01-uni/primo-anno/analisi-1/basi-funzioni/definizioni/def-punti-accumulazione-and-others#punti di accumulazione\|limiti di tutte le successioni convergenti]]). Quindi ogni successione in $A$ ammette una sottosuccessione convergente a un punto di $A$
$$\implies A \text{ è compatto }$$
