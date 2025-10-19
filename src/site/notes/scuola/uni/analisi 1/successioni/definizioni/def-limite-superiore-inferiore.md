---
{"dg-publish":true,"permalink":"/scuola/uni/analisi-1/successioni/definizioni/def-limite-superiore-inferiore/","tags":["math","uni"]}
---

### definizione
sia $a_n$ definiamo $\text{limite sup di } a_n$ $\limsup a_n$ OPPURE $\overline{\lim} a_n$
- se $a_n$ non è superiormente limitata allora definiamo $\overline{\lim} a_n = +\infty$ 
- se $a_n$ è limitata superiormente allora:
  costruiamo una successione $b_n$ :  
$$b_n := \text{sup}\{ a_n, a_{n+1}, a_{n+2}, ...\} \ \forall n$$
  (dove sup = [[scuola/uni/analisi 1/successioni/definizioni/def-estremo-superiore-inferiore-e-max-min\|estremo sup]]) allora $b_n$ è monotona decrescente e limitata $\implies$ [[scuola/uni/analisi 1/successioni/teoremi/teorema-monotona-allora-regolare\|converge]] a $l \in [-\infty, +\infty)$ poniamo $\overline{\lim} a_n = lim \ b_n$
### proprietà minori
- $\overline{\lim} a_n \ge \underline{\lim} a_n$
- $\overline{\lim} a_n = \underline{\lim} a_n \iff a_n \rightarrow l \in \overline{\mathbb{R}} \implies lim \ a_n = \overline{\lim} a_n = \underline{\lim} a_n$
- quindi naturalmente se $a_n$ oscilla allora $\overline{\lim} a_n < \underline{\lim} a_n$
### teorema equivalente alla definizione
il limite superiore è il più grande tra i [[scuola/uni/analisi 1/successioni/definizioni/def-limiti-sottosuccessionali\|limiti sottosuccessioniali]]