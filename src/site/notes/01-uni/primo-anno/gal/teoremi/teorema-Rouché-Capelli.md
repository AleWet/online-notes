---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/gal/teoremi/teorema-rouche-capelli/","tags":["math","uni"],"updated":"2026-03-24T11:19:09.689+01:00"}
---

Sia $A \underline{x}= \underline{b}$ un sistema lineare in $n$ incognite allora :
1) se [[01-uni/primo-anno/gal/definizioni/def-rango-(tbf)\|rango]]$([A| \underline{b}]) = rank(A) + 1$ il sistema non ha soluzioni
2) se $rank([A|\underline{b}]) = rank(A) = n$ il sistema ha un'unica soluzione
3) se $rank([A|\underline{b}]) =rank(A) < n$ il sistema ha infinite soluzione "disposte" come il [[01-uni/primo-anno/gal/definizioni/def-kernel\|nucleo]] di $A$
### intuizione 1
Il teorema di Rouché-Capelli ti dice in pratica se un dato sistema lineare è risolvibile o meno. Sia dato un sistema lineare :
$$A \underline{x}$$
rappresentato da una [[01-uni/primo-anno/gal/definizioni/def-matrice-(tbf)\|matrice]] $A$ nelle incognite $\underline{x}$, voglio sapere se un certo "vettore" $\underline{b}$ (qui inteso come insieme ordinato di numeri e basta) è una possibile soluzione di questa equazione :
$$\exists  \underline{x} :A \underline{x} = \underline{b} ?$$
questo è equivalente a scrivere : 
$$\begin{cases}
a_{11}x_{1}+a_{12}x_{2}+\dots+a_{1n} = b_{1} \\
a_{21}x_{1}+a_{22}x_{2}+\dots+a_{2n} = b_{2} \\
\vdots \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \  \vdots  \ \ \ \ \ \ \ \ \  \ddots  \ \ \ \ \ \ \ \ \ \ \ \ \ \  \vdots \\
a_{m 1}x_{1} + a_{m 2}x_{2} + \dots +a_{mn} = b_{n} 
\end{cases} $$
per fare questo calcolo usi quasi sempre il [[01-uni/primo-anno/gal/definizioni/def-metodo-eliminazione-gauss-(tbf)\|MEG]] trovando la matrice a scala $U| \underline{b}$ :
$$\begin{cases}
a_{11}x_{1}+a_{12}x_{2}+\dots+a_{1n}  &  = b_{1} \\
0+\dots    & =b_{2}-\alpha \\
\vdots \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \  \vdots  \ \ \ \ \ \ \ \ \  \ddots  \ \ \ \ \ \ \ \ \ \ \ \ \ \  &  \vdots \\ 
0+0+0+0+0+\dots+\gamma & =b_{n}-\beta
\end{cases}$$ da questo sistema si vede subito se il sistema è risolvibile, basta che dall'ultima equazione sostituisci all'indietro e trovi uno e un solo vettore $\underline{x}$. Questo è uno dei casi possibili, se ci sono variabili libere (il rango non è massimo) allora tutte le soluzioni hanno un grado di libertà (quindi sono infinite, tutta una retta di vettori $\underline{x}$ viene mappata ad un punto $\underline{b}$). Se però il rango della matrice $A|\underline{b} > rank(A)$ questo equivale a dire che nell'ultima equazione hai una cosa del tipo:
$$\tag{in A|b}0+0+\dots+0 = b_{n}-\gamma$$
mentre la matrice originale $A$ avevi semplicemente tutti $0$ (lo zero alla fine era sottinteso) : 
$$0+0+\dots+0 = 0 \tag{in A}$$
naturalmente visto che $rank(A|\underline{b}) < rank(A)$ il termine dopo l'uguale $b_{n}-\gamma \neq 0$ se no il rango sarebbe uguale e avremmo infinite soluzioni come nel caso prima. (questo caso è possibile naturalmente solo quando il rango della matrice non è massimo).