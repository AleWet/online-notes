---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/analisi-1/funzioni/definizioni/def-funzione-costante-a-tratti/","tags":["math","uni"],"updated":"2026-01-06T11:25:16.038+01:00"}
---

una funzione $h : \mathbb{R} \to \mathbb{R}$ è detta costante a tratti se esistono $N$ numeri reali $\lambda_{1}, \lambda_{2}, \dots \lambda_{N}$ e $N$ [[01-uni/primo-anno/analisi-1/basi-funzioni/definizioni/def-intervallo\|intervalli]] reali $K_{1}, \dots K_{n}$ tali che : 
$$h(x) = \sum_{k=1}^n \lambda_{k}\ \chi_{K_{n}}(x)$$
### osservazione importante 
sia $h:[a,b] \to \mathbb{R}$ una funzione costante a tratti, essa è [[01-uni/primo-anno/analisi-1/funzioni/definizioni/def-integrale-Riemann#Riemann integrabile\|Riemann integrabile]] e si dimostra immediatamente:
$$\int_{a}^bh(x)dx = \sum_{k=1}^n\lambda_{k}\int_{a}^b \chi_{I_{k}}(x)dx$$
usando la [[01-uni/primo-anno/analisi-1/funzioni/teoremi/teoremi-integrali-Riemann/teorema-linearità-integrale\|linearità integrale]]
$$\int_{a}^b \chi_{I_{k}}(x)dx = l(I_{k})$$
guarda [[01-uni/primo-anno/analisi-1/funzioni/definizioni/def-misura-secondo-Riemann#osservazione 2\|qui]] per questo passaggio, in pratica ti dice che l'integrale della funzione indicatrice di un intervallo è la lunghezza (= alla misura) dell'intervallo
$$\implies \int_{a}^b h(x)dx = \sum_{k = 1}^n \lambda_{k}  * l(I_{k})$$
stai quindi "sommando" insieme delle lunghezze di degli intervalli scalate di una costante $\lambda$, per più dettagli guarda QR4.
