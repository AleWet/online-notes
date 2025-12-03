---
{"dg-publish":true,"permalink":"/uni/primo-anno/analisi-1/funzioni/definizioni/def-punto-cambio-concavita/","tags":["math","uni"]}
---

Sia $f:[a,b] \to \mathbb{R}$ e sia $x_0 \in (a,b)$. 

Diciamo che $x_0$ è un **punto di cambio di concavità/convessità** se:

$$\exists \ \varepsilon >0 : \begin{cases}
f \text{ è convessa in } [x_0-\varepsilon, x_0] \text{ e concava in } [x_0, x_0+\varepsilon] \\\\
\text{oppure} \\\\
f \text{ è concava in } [x_0-\varepsilon, x_0] \text{ e convessa in } [x_0, x_0+\varepsilon]
\end{cases}$$

In altre parole, esiste un intorno di $x_0$ dove la funzione "cambia curvatura": da convessa a concava o viceversa. Per le definizioni di funzione convessa/concava, vedi [[uni/primo anno/analisi 1/funzioni/definizioni/def-funzione-convessa\|qui]].
### relazione con i punti di flesso
Se $f$ è [[uni/primo anno/analisi 1/funzioni/definizioni/def-derivata#derivabilità\|derivabile]] in $x_0$ (punto di cambio di concavità), allora $x_0$ è un [[uni/primo anno/analisi 1/funzioni/definizioni/def-punto-di-flesso\|punto di flesso]].
### osservazione importante 1
se $f$ è due volte [[uni/primo anno/analisi 1/funzioni/definizioni/def-derivata#derivabilità\|derivabile]] in $x_0$, punto di cambio di concavità, allora:
$$f''(x_0) = 0$$
e si dimostra nel seguente modo: 
$f'$ (definita in un intorno di $x_0$) ha un estremo locale in $x_0$ poiché è crescente/decrescente prima e decrescente/crescente dopo (se no non sarebbe un punto di cambio di concavità). 
La tesi segue dal [[uni/primo anno/analisi 1/funzioni/teoremi/teoremi funzione derivata/teorema-Fermat\|teorema-Fermat]]: se $f'$ ha un estremo locale in $x_0$ e $f'$ è derivabile in $x_0$, allora $(f')'(x_0) = f''(x_0) = 0$.
