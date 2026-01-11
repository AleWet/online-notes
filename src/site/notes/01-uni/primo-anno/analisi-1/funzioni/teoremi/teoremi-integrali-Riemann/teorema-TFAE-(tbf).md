---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/analisi-1/funzioni/teoremi/teoremi-integrali-riemann/teorema-tfae-tbf/","tags":["math","uni"]}
---

le seguenti affermazioni sono equivalenti:
$$\tag{1} f \in R(a,b)$$
$$\tag{2} \forall \varepsilon > 0 \text{ esistono due funzioni definite a tratti } h^+, h^- \text{ tali che } h^- \leq f \leq h^+ \text{ e tali che :}$$
$$\int_{a}^b h(x)dx < \varepsilon \ \ \text{ dove } h(x):= h^+(x)-h^-(x)$$
### osservazioni
Alcune definizioni di integrali usano prima la seconda, definendo prima la misura di una [[01-uni/primo-anno/analisi-1/funzioni/definizioni/def-funzione-costante-a-tratti\|funzione costante a tratti]] e poi l'integrale. Riemann invece fa il contrario.
### dim $(1) \Rightarrow (2)$
Qui basta notare che nell'[[01-uni/primo-anno/analisi-1/funzioni/definizioni/def-integrale-Riemann\|integrale di Riemann]] $S_{n}$ e $s_{n}$ sono già le tue funzioni definite a tratti e la cui differenza è infinitesima, definisci quindi $h^{\pm}$ nel seguente modo:
$$h^+(x) = \sum_{k=1}^n \chi_{I_{k}} (x)\sup_{I_{k}}(f)$$
$$h^-(x) = \sum_{k=1}^n \chi_{I_{k}} (x)\inf_{I_{k}}(f)$$
### dim $(2) \Rightarrow  (1)$ (tbd)
 