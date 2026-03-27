---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/analisi-1/funzioni/teoremi/teoremi-integrali-riemann/teorema-linearita-integrale/","tags":["math","uni"],"updated":"2026-01-05T16:52:24.606+01:00"}
---

siano $f,g \in R(a,b)$ (dove con $R(a,b)$ si intende [[01-uni/primo-anno/analisi-1/funzioni/definizioni/def-integrale-Riemann\|questo]]) allora 
$$\tag{1}f+\lambda g \in R(a,b)$$
$$\tag{2}\int_{a}^b [f(x)+\lambda g(x)] )= \int_{a}^b f(x)dx+\lambda\int_{a}^b g(x)dx$$
### osservazione importante
prima di dimostrare questo teorema è necessaria la seguente osservazione :
siano $f,g:I \to \mathbb{R}$ allora:
$$\sup_{I}(f,g) \le \sup_{I}f+\sup_{I}g$$
$$\inf_{I}(f,g) \ge \inf_{I}f+\inf_{I}g$$
dimostro brevemente:
$$\text{sia } x \in I \implies f(x)\le \sup_{I}f, \ \ g(x) \le \sup_{I}g$$
$$\forall x \in I , \ f(x)+g(x) \le \sup_{I}f+\sup_{I}g$$
$$\implies \sup_{I}(f,g) \le \sup_{I}f +\sup_{I}g \ \text{ per la permanenza del segno}$$
lo stesso ragionamento si fa con l'$\inf$ però la relazione è al contrario, l'$\inf$ della somma è $\geq$ della somma degli $\inf$.
### dim
prendo $\lambda = 1$ per comodità, la dimostrazione è analoga con $\lambda$ generico.
Fissato $I_{k}$ ottengo che :
$$ \inf_{I_{k}}f+ \inf_{I_{k}}g \leq\inf_{I_{k}} (f+g) \leq \sup_{I_{k}}(f+g)\leq \sup_{I_{k}}f + \sup_{I_{k}}g$$
e noto che queste sono le altezze dei rettangoli delle somme superiori e inferiori dell'integrale
$$\implies s_{n}(f)+s_{n}(g) \leq s_{n}(f+g) \leq S_{n}(f+g) \leq S_{n}(f) + S_{n}(g)$$
e poiché le singole funzioni sono integrabili ho che :
$$s_{n}(f)+s_{n}(g) \to \int_{a}^b f(x)dx + \int_{a}^b g(x)dx$$
$$ S_{n}(f) + S_{n}(g)\to \int_{a}^b f(x)dx + \int_{a}^b g(x)dx$$
allora utilizzo il [[01-uni/primo-anno/analisi-1/successioni/teoremi/teorema-del-confronto\|teorema-del-confronto]] due volte e ottengo:
$$s_{n}(f+g) , S_{n}(f+g)\to \int_{a}^b f(x)dx + \int_{a}^b g(x)dx$$
$$h:=f+g$$
$$\int_{a}^b h(x)dx = \int_{a}^bf(x)dx + \int_{a}^b g(x)dx$$
$$\implies \int_{a}^b f(x)+g(x)dx = \int_{a}^b f(x)dx + \int_{a}^b g(x)dx$$
