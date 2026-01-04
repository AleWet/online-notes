---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/analisi-1/funzioni/definizioni/def-primitiva/","tags":["math","uni"]}
---

sia $f:[a,b] \to \mathbb{R}$ definiamo una *primitiva* di $f$ una funzione [[01-uni/primo-anno/analisi-1/funzioni/definizioni/def-derivata#derivabilità\|derivabile]] in ogni punto del dominio :
$$F:[a,b] \to \mathbb{R} : F'(x) = f(x) \ \ \forall x$$
### notazione interna al corso
se $f$ ammette **primitiva** e se $f$ è **Riemann-integrabile** su $[a,b]$ allora diciamo che
$$f \in R_{P}(a,b)$$
### osservazione 1
Una funzione generica $f$ per ammettere primitiva deve avere la [[01-uni/primo-anno/analisi-1/funzioni/definizioni/def-Darboux\|proprietà di Darboux]] poiché sappiamo che [[01-uni/primo anno/analisi 1/funzioni/teoremi/teoremi funzione derivata/teorema-derivata-Darboux\|la funzione derivata ha sempre la proprietà di Darboux]]. Di conseguenza non può avere discontinuità di tipo salto o eliminabili. Posso quindi dire che tutte le $f$ con di Darboux ammettono primitiva? No, è solo necessario
### osservazione 2
Supponiamo che $f$ ammetta primitiva, allora tutte le sue primitive saranno della forma:
$$F(x) + c , \ c \in \mathbb{R}$$
### osservazione 3
assumiamo che $F$ e $G$ siano primitive di $f \implies F = G+c, \ c \in \mathbb{R}$ e questa cosa si dimostra velocemente :
$$F,G \text{ primitive di } f$$
$$(F-G)' = F'-G' = f-f = 0$$
$$\implies (F-G) \text{ è una funzione costante } h(x) = c$$
l'ultimo passaggio si deriva da [[01-uni/primo anno/analisi 1/funzioni/teoremi/teoremi funzione derivata/teorema-derivata-monotonia\|questo teorema]], dice che una  funzione con derivata nulla è costante.
### osservazione 4
consideriamo le seguenti affermazioni:
$$\tag{1} f \text{ ammette primitiva in } [a,b]$$
$$\tag{2} f \in R(a,b)$$
dove con $R(a,b)$ si intende la [[01-uni/primo-anno/analisi-1/funzioni/definizioni/def-integrale-Riemann-TBF\|seguente cosa]], allora 
$$(1) \not\Rightarrow (2)$$
poiché le [[01-uni/primo-anno/analisi-1/funzioni/definizioni/def-funzione-costante-a-tratti\|funzioni costanti a tratti]] non ammettono primitiva poiché non sono Darboux
$$(2) \not\Rightarrow (1)$$
e si può fare il seguente controesempio:
$$f(x) = \begin{cases}
2x\sin\left( \frac{1}{x^2} \right) + x^2\cos\left( \frac{1}{x^2} \right)(-2x^{-3})  & x \ne 0 \\ \\
0  & x=0
\end{cases}$$
$$F(x) = \begin{cases}
x^2\sin\left( \frac{1}{x^s} \right) \ \ \ x \ne 0 \\  \\
0 \ \ \ \ \ \ \ \ \  \ \ \ \ \ \ \ \ \ \ \ x = 0
\end{cases}$$
e trovi che $f$ ammette primitiva ma non è limitata su $[a,b]$ di conseguenza non può essere integrabile secondo Riemann. Il Pata ha anche detto che esiste un esempio di una funzione limitata che ammette primitiva ma che non è integrabile ma non l'ha esplicitato.