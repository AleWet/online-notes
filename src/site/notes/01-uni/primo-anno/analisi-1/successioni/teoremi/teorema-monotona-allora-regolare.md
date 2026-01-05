---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/analisi-1/successioni/teoremi/teorema-monotona-allora-regolare/","tags":["math","uni"]}
---

### ==primo caso== 
sia $a_n$ [[01-uni/primo-anno/analisi-1/successioni/definizioni/def-successione-divergente\|diverge]]. (analogo per le decrescenti con $-\infty$)
### ==secondo caso==
sia $a_n$ monotona ma questa volta limitata, allora posso definire l'insieme $A$ della successione :
$$A :\{a_0, a_1,a_2,a_3,a_4,a_5,a_6,...\}$$
con $A\ne\emptyset$ e $A$ [[01-uni/primo-anno/analisi-1/successioni/definizioni/def-estremo-superiore-inferiore-e-max-min\|superiormente limitato]] da un elemento $\gamma\in\mathbb{R}$ dalla completezza di $\mathbb{R}$.
allora posso dire che fissato un $\epsilon>0$:
$$\exists a_{n0} \in A : \ \gamma-\epsilon\le a_{n0} \le \gamma$$
$$\text{poiché crescente} \implies \gamma-\epsilon\le a_{n0} \le a_n \le \gamma$$
ciò vale $\forall \epsilon>0 \ \land \forall n \ge n_0$ quindi è equivalente alla definizione di [[01-uni/primo-anno/analisi-1/successioni/definizioni/def-successione-convergente\|convergenza dal basso]]
$$\implies a_n \rightarrow \gamma^-$$
___
### completezza in R
dire che $\mathbb{R}$ è completo è analogo a dire che tutte le successioni monotone limitate convergono.
