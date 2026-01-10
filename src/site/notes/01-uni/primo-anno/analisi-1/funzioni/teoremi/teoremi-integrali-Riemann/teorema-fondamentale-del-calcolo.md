---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/analisi-1/funzioni/teoremi/teoremi-integrali-riemann/teorema-fondamentale-del-calcolo/","tags":["math","uni"]}
---

sia $f \in R_{P}(a,b)$ quindi intendiamo [[01-uni/primo-anno/analisi-1/funzioni/definizioni/def-primitiva#notazione interna al corso\|che ammette primitiva e che è integrabile]], chiamata $F$ una primitiva di $f$ si ha che:
$$\int_{a}^b f(x)dx = F(b)-F(a)  = F \big|_{a}^b$$
### dim
per comodità scelgo l'intervallo $[0,1]$ al posto di $[a,b]$ e sia quindi $F$ una primitiva di $f$ in $[a,b]$ e dividiamo l'intervallo $[0,1]$ in $n$ intervalli di lunghezza $1/n$ chiamando gli estremi di questi intervalli $x_k$ con $k = 1, 2,3,\dots ,n$ e $x_{0} = a, \ x_{n} = b$. 
Considero quindi l'intervallo generico $I_{k}$ dove $I_{k} = [x_{k-1},x_{k}]$ e applico [[01-uni/primo-anno/analisi-1/funzioni/teoremi/teoremi-funzione-derivata/teorema-Lagrange-(tbf)\|Lagrange]] a $F$ su questo intervallo generico, posso poiché per ipotesi $F$ è derivabile su tutto l'intervallo (se no non sarebbe la primitiva di $f$).
$$\implies \exists y \in(x_{k-1},x_{k}) : F(x_{k})-F(x_{k-1}) = F'(y)(x_{k}-x_{k-1})$$
$$F'(y) = f(y) \text{ per definizione di primitiva}$$
$$\implies F(x_{k})-F(x_{k-1}) = \frac{f(y)}{n}$$
$$y \in I \implies \inf_{I_{k}}f\le f \le \sup_{I_{k}}f$$
$$\implies \forall k \in [1,n]\cap \mathbb{N}$$
$$\frac{\inf_{I_{k}}f}{n} \le \frac{f(y)}{n} \le  \frac{\sup_{I_{k}}f}{n}$$
$$\implies \frac{1}{n}\inf_{I_{k}}f\  \le F(x_{k})-F(x_{k-1})\  \le  \frac{1}{n}\sup_{I_{k}}f$$
ho quindi trovato $n$ disuguaglianze diverse, una per ogni intervallo $I_{k}$, posso quindi sommarle tutte per trovare:
$$\frac{1}{n} \sum_{k=1}^n \inf_{I_{k}}f\  \le \sum_{k = 1}^n [F(x_{k})-F(x_{k-1})] \ \le \frac{1}{n}\sum_{k=1}^n \sup_{I_{k}}f$$
e qui noto che i termini ai lati sono esattamente la **somma superiore** e la **somma inferiore** di $f$ :
$$\implies s_{n}\  \le \sum_{k = 1}^n [F(x_{k})-F(x_{k-1})] \ \le S_{n}$$
e qui posso fare la seguente osservazione riguardo il termine al centro:
$$\sum_{k=1}^n [F(x_{k})-F(x_{k-1})] = F(x_{1})-F(x_{0})+F(x_{2})-F(x_{1})+\dots+F(x_{n})-F(x_{n-1})$$
infatti questa è esattamente uguale a una [[01-uni/primo-anno/analisi-1/serie/definizioni/def-serie-telescopica\|serie telescopica]] dove tutti i termini centrali si cancellano:
$$\sum_{k=1}^n [F(x_{k})-F(x_{k-1})] = F(x_{n})-F(x_{0})$$
$$\implies \sum_{k=1}^n [F(x_{k})-F(x_{k-1})] = F(b)-F(a)$$
$$\implies s_{n} \le F(b)-F(a) \le S_{n}$$
e qui uso il fatto che $f \in R(a,b)$ infatti ottengo che:
$$S_{n}(f),s_{n}(f) \to \int_{a}^b f(x)dx$$
$$\implies \int_{a}^b f(x)dx = F(b)-F(a)$$
usando il [[01-uni/primo-anno/analisi-1/successioni/teoremi/teorema-del-confronto\|teorema del confronto per le successioni]] e il fatto che $F(b)-F(a)$ è una costante e l'unico modo per una costante di tendere ad un'altra costante è se le due sono uguali.
