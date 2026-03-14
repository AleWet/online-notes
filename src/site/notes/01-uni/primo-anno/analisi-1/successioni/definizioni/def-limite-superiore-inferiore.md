---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/analisi-1/successioni/definizioni/def-limite-superiore-inferiore/","tags":["math","uni"],"updated":"2026-02-24T15:52:00.487+01:00"}
---

### definizione
sia $a_n$ definiamo $\text{limite sup di } a_n$ $\limsup a_n$ OPPURE $\overline{\lim} a_n$
- se $a_n$ non è superiormente limitata allora definiamo $\overline{\lim} a_n = +\infty$ 
- se $a_n$ è limitata superiormente allora:
  costruiamo una successione $b_n$ :  
$$b_n := \text{sup}\{ a_n, a_{n+1}, a_{n+2}, ...\} \ \forall n$$
  (dove sup = [[01-uni/primo-anno/analisi-1/successioni/teoremi/teorema-monotona-allora-regolare\|converge]] a $l \in [-\infty, +\infty)$ poniamo $\overline{\lim} a_n = lim \ b_n$
### proprietà minori
- $\overline{\lim} a_n \ge \underline{\lim} a_n$
- $\overline{\lim} a_n = \underline{\lim} a_n \iff a_n \rightarrow l \in \overline{\mathbb{R}} \implies lim \ a_n = \overline{\lim} a_n = \underline{\lim} a_n$
- quindi naturalmente se $a_n$ oscilla allora $\overline{\lim} a_n < \underline{\lim} a_n$
### teorema equivalente alla definizione
il limite superiore è il più grande tra i [[01-uni/primo-anno/analisi-1/successioni/definizioni/def-limiti-sottosuccessionali\|limiti sottosuccessioniali]]