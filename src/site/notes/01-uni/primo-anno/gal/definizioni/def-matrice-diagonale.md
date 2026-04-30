---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/gal/definizioni/def-matrice-diagonale/","tags":["math","uni"],"updated":"2026-04-28T19:01:47.671+02:00"}
---

Sia $L$ un'[[01-uni/primo-anno/gal/definizioni/def-funzione-lineare\|endomorfismo]] di $V$ con base $B = (b_{1},b_{2},\dots,b_{n})$ allora dico che la [[01-uni/primo-anno/gal/definizioni/def-matrice-(tbf)\|matrice]] rappresentativa $A$ di $L$ è diagonale se e solo se :
$$L(v_{k}) = \lambda v_{k} \ \ k \in [1,n] \cap \mathbb{N}$$
ovvero $A = diag(\lambda_{1}, \dots, \lambda_{n}$ che è un modo corto per dire :
$$A = \begin{bmatrix}
\lambda_{1} & 0 & \dots & 0 \\
0 & \lambda_{2}  & \dots & 0 \\
\vdots & \vdots & \ddots & \vdots \\
0 & 0 & 0 & \lambda_{n}
\end{bmatrix}$$
la proprietà di prima equivale infatti a dire che se metti qui dentro un vettore della base $b_i$ ti esce lo stesso vettore ma scalato di un fattore $\lambda_{i}$ : 
$$x_{i} = [b_{i}]_{B} = [0,0,\dots, 1,0, \dots,0]^T \ \ \implies Ax_{i} = \lambda_{i}x_{i} $$
se espandi il prodotto lo vedi subito:
$$Ax_{i} = A = \begin{bmatrix}
\lambda_{1} & 0 & \dots & 0 \\
0 & \lambda_{2}  & \dots & 0 \\
\vdots & \vdots & \ddots & \vdots \\
0 & 0 & 0 & \lambda_{n}
\end{bmatrix} \begin{bmatrix}
0 \\
\vdots \\  
1 \\
\vdots
\end{bmatrix} = 0 \begin{bmatrix}
\lambda_{1} \\
0 \\
0 \\
\vdots  \\
\end{bmatrix}
+\dots+\lambda_{i}\begin{bmatrix}
0 \\
\vdots \\  
1 \\
\vdots
\end{bmatrix} +\dots = \lambda_{1}x_{1}
$$
