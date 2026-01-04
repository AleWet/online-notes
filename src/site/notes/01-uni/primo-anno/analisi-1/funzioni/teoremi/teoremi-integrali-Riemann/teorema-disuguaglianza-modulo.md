---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/analisi-1/funzioni/teoremi/teoremi-integrali-riemann/teorema-disuguaglianza-modulo/","tags":["math","uni"]}
---

$f \in R(a,b)$ (dove con $R(a,b)$ si intende la [[01-uni/primo anno/analisi 1/funzioni/definizioni/def-integrale-Riemann-TBF\|seguente cosa]])
$$\implies |f| \in R(a,b)$$
$$\implies \bigg |\int_{a}^af(x)dx \bigg| \le \int_{a}^a|f(x)|dx$$
### dim
la dimostrazione usa banalmente il [[01-uni/primo-anno/analisi-1/funzioni/teoremi/teoremi-integrali-Riemann/teorema-confronto-integrali-TBF\|teorema-confronto-integrali-TBF]] dalla seguente osservazione:
$$-|f| \le f \le |f| \ \ \forall x$$
$$\implies \int_{a}^b -|f| \le \int_{a}^b f \le \int_{a}^b |f|$$
qui usi la [[01-uni/primo-anno/analisi-1/funzioni/teoremi/teoremi-integrali-Riemann/teorema-linearità-integrale-TBF\|linearità dell'integrale]] :
$$\int_{a}^b |-f| = -\int_{a}^b |f|$$
$$\implies -\int_{a}^b |f| \le \int_{a}^b f \le \int_{a}^b |f| $$
$$\iff$$
$$\int_{a}^b f \le \int_{a}^b |f|$$