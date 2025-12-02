---
{"dg-publish":true,"permalink":"/uni/primo-anno/analisi-1/funzioni/teoremi/teoremi-funzioni-continue/teorema-weierstrass/","tags":["math","uni"]}
---

sia $f:[a,b] \to \mathbb{R}$ una funzione [[uni/primo anno/analisi 1/funzioni/definizioni/def-continuità\|continua]] allora $f$ ammette [[uni/primo anno/analisi 1/successioni/definizioni/def-estremo-superiore-inferiore-e-max-min\|massimo e minimo]] dove $[a,b]$ è un intervallo [[uni/primo anno/analisi 1/basi funzioni/definizioni/def-insiemi-aperti-chiusi\|chiuso]] e limitato.
### osservazione 1
$[a,b]$ può essere sostituito da un [[uni/primo anno/analisi 1/basi funzioni/definizioni/def-insieme-compatto\|insieme compatto]].
### cosa succede se allento le ipotesi
1) funzione continua, intervallo limitato ma non chiuso
   controesempio = $f:(0,1] \to \mathbb{R} , \ \ f(x) = \frac{1}{x}$
   
2) funzione continua, intervallo chiuso ma non limitato
   controesempio = $f:[0,+\infty) \to \mathbb{R}, \ \ f(x) = \arctan(x)$
   
3) intervallo chiuso e limitato ma funzione non continua
   controesempio = $f:[0,1] \to \mathbb{R}, \ \ f(x) = \cases{\frac{1}{x} \ x > 0 \\ \\ 0 \ \ x = 0}$
### dim
##### lemma
prima di dimostrare il teorema è necessario il seguente lemma:
presa una successione $x_n \in [a,b] \implies \exists x \in [a,b]$ e una [[uni/primo anno/analisi 1/successioni/definizioni/def-sottosuccessione\|sottosuccessione]] $x_{n_k}$ di $x_n$ t.c. $x_{n_k} \to x$.
Importante notare che questa è la definizione di [[uni/primo anno/analisi 1/basi funzioni/definizioni/def-insieme-compatto\|compattezza]] di un insieme.
##### dim lemma
$x_n \in [a,b] \implies x_n$ è limitata $\implies \exists x_{n_k} \to x \in \mathbb{R}$ grazie a [[uni/primo anno/analisi 1/successioni/teoremi/teorema-bolzano-weierstrass\|BW]]. Posso poi dire che:
$$\tag{1} x_{n_k} \le b \ \forall n \implies x \le b$$
$$\tag{1} x_{n_k} \ge a \ \forall n \implies x \ge a$$
usando 2 volte il [[uni/primo anno/analisi 1/successioni/teoremi/teorema-della-permanenza-del-segno\|teorema-della-permanenza-del-segno]] :
$$\implies x \in [a,b]$$
##### dim Weierstrass
devo dimostrare che $f$ ammette [[uni/primo anno/analisi 1/successioni/definizioni/def-estremo-superiore-inferiore-e-max-min\|massimo]] allora parto col definire $M := supf , M \in (-\infty, +\infty]$ ammettendo anche che $f$ non sia superiormente limitata.
Posso poi fare la seguente osservazione:
$$\exists \ x_n \in [a,b] : f(x_n) \to M$$
questo per definizione di [[uni/primo anno/analisi 1/successioni/definizioni/def-estremo-superiore-inferiore-e-max-min\|estremo superiore]]: fai che $\forall \varepsilon >0 \ \exists x \in [a,b] : M-\varepsilon < f(x) \le M$ (cambia con $\forall K>0$ nel caso in cui $M = +\infty$) e quindi :
$$\forall n \ \exists x : f(x) \in \left( M-\frac{1}{n} ,M\right] \implies \text{crei } x_n :f(x_n) \to M$$
adesso devo mostrare che $\exists x \in [a,b] : f(x) = M$ e quindi che $M$ è finito.
dal [[uni/primo anno/analisi 1/funzioni/teoremi/teoremi funzioni continue/teorema-Weierstrass#lemma\|lemma qui sopra]] sai che
$$\exists x_{n_k} \in [a,b] : x_{n_k} \to x \in [a,b]$$
$$\text{se }f(x_n) \to M \implies \text{ presa una generica sottosuccessione } x_{n_k} \ , \ f(x_{n_k}) \to M$$
$$\text{ poiché dal lemma } x_{n_k} \to x \in [a,b], f(x_{n_k}) \to M$$
e poiché $x \in [a,b]$ e $f(x)$ è [[uni/primo anno/analisi 1/funzioni/definizioni/def-continuità#funzione continua\|continua]] in $[a,b]$ e quindi anche in $x$ 
$$\implies f(x_{n_k}) \to f(x) \implies f(x) = M$$
si fa lo stesso ragionamento con l'estremo inferiore per trovare il $\min$.
___



