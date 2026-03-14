---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/analisi-1/serie/definizioni/def-serie-telescopica/","tags":["math","uni"],"updated":"2026-02-24T15:52:00.485+01:00"}
---

una [[01-uni/primo-anno/analisi-1/serie/definizioni/def-serie\|serie]] telescopica è una serie il cui termine generale può essere espresso nel seguente modo:
$$\begin{equation}{\textstyle \sum}a_n\end{equation} \text{ dove } a_n = b_n - b_{n+1}$$
si vede subito dalla $S_n$ che questa serie si comporta in modo speciale:
$$S_n = b_0-b_1+b_1-b_2+b_2-b_3+...-b_{n+1}$$
$$S_n = b_0-b_{n+1}$$
$$\implies \begin{equation}{\textstyle \sum}a_n\end{equation} = \lim b_0+\lim b_{n+1} = b_0+\lim b_{n}$$
### serie di Mengoli
caso speciale delle serie telescopiche dove
$$a_n = \frac{1}{n}-\frac{1}{n+1}$$
### serie telescopica con gap
si può generalizzare il concetto di serie telescopica :
$$ b_n =a_n - a_{n+k}$$
$$\sum b_n = a_0-a_k+a_1-a_{k+1}+a_2-a_{k+2}+...+a_{n-1}+a_{n+k-1}+a_n-a_{n+k}$$
$$=\sum b_n = a_0+a_1+a_2+...+a_k-k*\lim a_n$$
