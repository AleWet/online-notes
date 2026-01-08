---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/analisi-1/successioni-funzioni/teoremi/teorema-convergenza-totale-uniforme/","tags":["math","uni"]}
---

se una [[01-uni/primo-anno/analisi-1/successioni-funzioni/definizioni/def-serie-di-funzioni\|serie di funzioni]] converge totalmente allora la serie converge uniformemente.
### dim
prima dimostro che se converge totalmente allora converge anche puntualmente:
sia $f_{n}:I\to \mathbb{R}$ e sia $M_{n} : \sup_{x\in I} |f_{n}| \leq M_{n}$ e $\sum M_{n}$ convergente allora fisso $x_{0} \in I$ e noto che:
$$|f_{n}(x_{0})| \leq \sup_{x \in I}|f_{n}(x)|\leq M_{n}$$
allora uso il [[01-uni/primo-anno/analisi-1/serie/teoremi/teorema-confronto-serie\|teorema-confronto-serie]] e trovo:
$$0\leq \sum|f_{n}(x_{0})| \leq \sum M_{n} \implies \sum|f_{n}(x_{0})| \text{ converge assolutamente}$$
$$\implies \sum f_{n}(x_{0 }) \text{ converge }$$
adesso dimostro che $\sum f_{n} \xrightarrow{u}S$ 
$$\left| \sum_{k = 0}^\infty f_{k}(x) - \sum_{k=0}^nf_{k}(x)\right| = \left|\sum_{k = n+1}^\infty f_{k}(x) \right|$$
$$\left|\sum_{k = n+1}^\infty f_{k}(x) \right| \leq \sum_{k = n+1}^\infty \left| f_{k}(x)\right|\le \sum_{k=n+1}^\infty M_{k} \ \ \ \ \forall x$$
$$\implies \sup_{x \in I} |s_{n}(x)-S(x)| \leq \sum_{k=n+1}^\infty M_{k}$$
osservo che la coda della serie a destra tende a $0$ poiché la serie converge :  
$$\lim_{ n \to \infty } \sum_{k=n+1}^\infty M_{k} = 0$$
$$\implies \lim_{ n \to \infty } |s_{n}(x)-S(x)| = 0$$
per il [[01-uni/primo-anno/analisi-1/successioni/teoremi/teorema-del-confronto\|teorema-del-confronto]].