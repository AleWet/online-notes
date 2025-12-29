---
{"dg-publish":true,"permalink":"/uni/primo-anno/analisi-1/funzioni/teoremi/teoremi-integrali-riemann/teorema-integrazione-per-parti/","tags":["math","uni"]}
---

siano $f,g \in R_{P}(a,b)$ (guarda [[uni/primo anno/analisi 1/funzioni/definizioni/def-primitiva#notazione interna al corso\|qui]]) e siano $F, G$ due loro **primitive** allora 
$$\int_{a}^b F(x)g(x)dx = FG \big|_{a}^b - \int_{a}^b f(x)G(x)dx$$
### dim
sappiamo che [[uni/primo anno/analisi 1/funzioni/teoremi/teoremi integrali Riemann/teorema-prodotto-integrabile\|il prodotto di funzioni integrabili è integrabile]] e che la [[uni/primo anno/analisi 1/funzioni/teoremi/teoremi integrali Riemann/teorema-linearità-integrale-TBF\|somma di integrabili è integrabile]] quindi 
$$h(x)= [F(x)G(x)]' = F(x)g(x)+f(x)G(x)$$
$$\implies h(x) \in R_{P}(a,b)$$
qui uso il [[uni/primo anno/analisi 1/funzioni/teoremi/teoremi integrali Riemann/teorema-fondamentale-del-calcolo\|teorema-fondamentale-del-calcolo]] e la [[uni/primo anno/analisi 1/funzioni/teoremi/teoremi integrali Riemann/teorema-linearità-integrale-TBF\|linearità]] e trovo:
$$\int_{a}^b h(x) = FG \big|_{a}^b = F(b)G(b)-F(a)G(a)$$
$$\implies \int_{a}^b F(x)g(x)dx + \int_{a}^b f(x)G(x)dx = FG \big|_{a}^b$$
questa dimostrazione tiene per scontato che le primitive siano integrabili, questo è vero perché la primitiva è per forza derivabile, [[uni/primo anno/analisi 1/funzioni/teoremi/teoremi funzione derivata/teorema-derivabile-allora-continua\|quindi è anche continua]] e quindi [[uni/primo anno/analisi 1/funzioni/teoremi/teoremi funzioni continue/teorema-continua-integrabile\|è anche integrabile]].