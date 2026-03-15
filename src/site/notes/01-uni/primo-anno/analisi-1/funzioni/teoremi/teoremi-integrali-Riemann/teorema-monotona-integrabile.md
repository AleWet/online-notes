---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/analisi-1/funzioni/teoremi/teoremi-integrali-riemann/teorema-monotona-integrabile/","tags":["math","uni"],"updated":"2026-01-06T10:21:53.794+01:00"}
---

una funzione $f:[a,b] \to \mathbb{R}$ monotona è automaticamente [[01-uni/primo-anno/analisi-1/funzioni/definizioni/def-integrale-Riemann\|Riemann integrabile]] ($\in R(a,b)$)
### osservazione 
una funzione monotona può avere infiniti salti e quindi infiniti punti di discontinuità ed essere comunque integrabile grazie a questo teorema ( $\neq$ da [[01-uni/primo-anno/analisi-1/funzioni/teoremi/teoremi-integrali-Riemann/teorema-finite-discontinuità-integrabile-(tbf)\|questo teorema]]). 
### dim
supponiamo che $f$ sia crescente, per $f$ decrescente la dimostrazione è analoga e prendo per semplicità $[a,b] = [0,1]$ in modo da avere $\frac{1}{n}$ come lunghezza di ogni partizione $I_{k}$.
$$S_{n} = \frac{1}{n}\left[ f\left( \frac{1}{n} \right) + f\left( \frac{2}{n} \right) + \dots +f\left(  \frac{n-1}{n}   \right) + f\left( \frac{n}{n} = 1 \right) \right]$$
questo perché in ogni intervallo, visto che $f$ è monotona, troverò il $\sup_{I_{k}}$ nell'estremo destro che so essere sempre a $k/n$, con lo stesso ragionamento:
$$s_{n} = \frac{1}{n}\left[ f(0)+f\left( \frac{1}{n} \right) + \dots+f\left(  \frac{n-1}{n} \right) \right]$$
$$\tag{*}\implies \omega(f) = S_{n}-s_{n} = \frac{f(1)-f(0)}{n} \to 0$$
$$\implies f \in R(a,b)$$
$(*)$ guarda [[01-uni/primo-anno/analisi-1/funzioni/teoremi/teoremi-integrali-Riemann/teorema-delta-somme-superiori-inferiori\|questo teorema]].