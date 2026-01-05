---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/analisi-1/funzioni/teoremi/teoremi-funzioni-continue/teorema-darboux/","tags":["math","uni"]}
---

sia $f : I \to \mathbb{R}$ dove $f$ è [[01-uni/primo-anno/analisi-1/funzioni/definizioni/def-Darboux\|ha la proprietà di Darboux]] 
### dim
siano $x,y \in I: x<y$ 
- se $f(x) = f(y)$ il valore intermedio è uno dei due estremi 
- se $f(x) \ne f(y)$ diciamo che $f(x) < f(y)$, preso un qualsiasi $\beta$ :
$$f(x)<\beta<f(y) \text{, voglio trovare } z : f(z) = \beta$$
$$g : [x,y] \to \mathbb{R}$$
$$g(t) := f(t) - \beta \tag{*}$$
$$ \implies g(y) = f(y) - \beta$$
$$\implies g(x) = f(x) -\beta$$
allora posso applicare il [[01-uni/primo-anno/analisi-1/funzioni/teoremi/teoremi-funzioni-continue/teorema-degli-zeri\|teorema-degli-zeri]] che mi dice che $\exists z \in (x,y) : g(z) = 0$
$$\implies g(z) = f(z) - \beta = 0$$
$$\implies f(z) = \beta \ \ \ \ \ \square$$
$$(*) \ g(t) \text{ è continua poiché somma di funzioni continue}$$
