---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/analisi-1/funzioni/teoremi/teoremi-integrali-riemann/teorema-cambio-variabile/","tags":["math","uni"],"updated":"2026-02-24T15:52:00.484+01:00"}
---

sia $f:[a,b] \to \mathbb{R}$ [[01-uni/primo-anno/analisi-1/funzioni/definizioni/def-continuità\|continua]] e $\phi:[a,b] \to [\alpha, \beta]$ [[01-uni/primo-anno/analisi-1/funzioni/definizioni/def-derivata#derivabilità\|derivabile]] con $\phi' \in R(\alpha,\beta)$ trovo che :  
$$\int_{\psi(a)}^{\psi(b)}f(x)dx = \int_{\alpha}^{\beta} f(\psi(t)) \psi'(t)dt$$
### dim 
noto subito che $f(\phi(x))\phi '(x) \in R_{p}(\alpha,\beta)$ e una sua primitiva è della forma:
$$F(\phi(x))' = f(\phi(x))\phi'(x) \implies \int_{\alpha}^{\beta} f(\psi(t)) \psi'(t)dt = F(\phi(\beta)) - F(\phi(\alpha))$$
anche $f \in R_{p}(\alpha,\beta)$ allora:
$$\int_{\phi(\alpha)}^{\phi(\beta)} f(x)dx = F(\phi(\beta))-F(\phi(\alpha))$$
ovvero la tesi.

