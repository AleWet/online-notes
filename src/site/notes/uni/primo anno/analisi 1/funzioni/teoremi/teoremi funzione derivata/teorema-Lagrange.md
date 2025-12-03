---
{"dg-publish":true,"permalink":"/uni/primo-anno/analisi-1/funzioni/teoremi/teoremi-funzione-derivata/teorema-lagrange/","tags":["math","uni"]}
---

sia $f:[a,b] \to \mathbb{R}$ (definita su tutto $[a,b]$) tale che :
1) $f$ è [[uni/primo anno/analisi 1/funzioni/definizioni/def-continuità\|continua]] in $[a,b]$ ([[uni/primo anno/analisi 1/basi funzioni/definizioni/def-intervallo\|intervallo]] [[uni/primo anno/analisi 1/basi funzioni/definizioni/def-insiemi-aperti-chiusi#insieme chiuso\|chiuso]])
2) $f$ è [[uni/primo anno/analisi 1/funzioni/definizioni/def-derivata\|derivabile]] in $(a,b)$ ([[uni/primo anno/analisi 1/basi funzioni/definizioni/def-intervallo\|intervallo]] [[uni/primo anno/analisi 1/basi funzioni/definizioni/def-insiemi-aperti-chiusi#insieme aperto\|aperto]])

$$\implies \exists \ c \in (a,b) : f'(c) = \frac{f(b)-f(a)}{b-a}$$
### osservazione 1
se aggiungo alle ipotesi
3) $f(a) = f(b)$ 
allora questo viene chiamato il ==teorema di Rolle==.
### cosa succede se allento le ipotesi
1) la prendo non continua in $[a,b]$
   $$f(x) = \cases{x  \ \ \ x < 1 \\ \\ 0 \ \ \ x = 1}$$
2) se la prendo non derivabile in $(a,b)$
   $$f(x) = |x|$$
in entrambi i casi non c'è un punto dove *m* della retta tangente è $= \frac{f(b)-f(a)}{b-a} = 0$
### osservazione 2 DA RIGUARDARE LEZIONE 18/11
$a \in \mathbb{R}, \ f:u(a) \to \mathbb{R} \ \land f \in C^1(u(a))$ ([[uni/primo anno/analisi 1/funzioni/definizioni/def-classi\|classi delle funzioni]]) e sia $a_n \to a, \ a_n \ne a$ 
$$\implies f(a_n)-f(a) \sim f'(a)(a_n-a)$$
si dimostra nel seguente modo:
1) sia $b_n$ compresa tra $a$ e $a_n \implies  b_n \to a$ ([[uni/primo anno/analisi 1/successioni/teoremi/teorema-del-confronto\|teorema-del-confronto]])
2) applico Lagrange in $[a,a_n]$ oppure  $[a_n, a]$ 
$$\implies f(a_n)-f(a) = f'(b_n)(a_n-a)$$
$$f'(b_n) \to f'(a) \text{ poiché f } \in C^1(u(a)) \text{ ed equivalenza di continuità successionale}$$
Da questa relazione derivi molti [[uni/primo anno/analisi 1/successioni/definizioni/def-asintotico\|asintotici]] come $e^{a_n}-e^a \sim e^a(a_n-a).$
### dim Rolle
supponiamo $f(a) = f(b)$, poiché $f$ è continua in $[a,b]$ allora $f$ ammette massimo e minimo nell'intervallo chiuso per [[uni/primo anno/analisi 1/funzioni/teoremi/teoremi funzioni continue/teorema-Weierstrass\|teorema-Weierstrass]]. 
1) caso banale : massimo e minimo sono entrambi negli estremi $a$ e $b \implies f$ è costante
   il che vorrebbe dire che tutti i punti nell'intervallo $[a,b]$ sono estremanti
2) assumiamo allora che almeno uno tra max e min non sia realizzato negli estremi 
   $\implies \exists c \in [a,b] : c$ è estremante. In entrambi i casi il [[uni/primo anno/analisi 1/funzioni/teoremi/teoremi funzione derivata/teorema-Fermat\|teorema-Fermat]] ci dice che 
   $f'(c) = 0$ arrivando quindi all'ipotesi
### dim Lagrange
Devo quindi dimostrare il caso più generale con $f(a), f(b)$ generici. Considero allora una generica retta $y = mx + q$ dove  
$$m = \frac{f(b)-f(a)}{b-a}, \ \ \ q \text{ qualsiasi}$$e sottraggo a $f$ la mia retta :
$$g(x) := f(x) -(mx+q)$$
poiché $f$ e la retta sono entrambe continue in $[a,b] \implies$ g è continua in $[a,b]$ e per lo stesso ragionamento $g$ è derivabile in $(a,b)$. Analizzo adesso $g$ agli estremi $a,b$ : 
$$g(a) = f(a) - \frac{f(b)-f(a)}{b-a}*a-q$$
$$g(b) = f(b)-\frac{f(b)-f(a)}{b-a}*b-q$$
$$g(a) \stackrel{?}{=} g(b)$$
$$\iff f(a)-ma -q = f(b)-mb-q$$
$$\iff f(b)-f(a) = m(b-a)$$
$$\iff m = \frac{f(b)-f(a)}{b-a}$$
$$\implies g(a) = g(b) \implies \exists \ c \in [a,b] : g'(c) = 0 \text{ per il teorema di Rolle}$$
$$g'(c) = 0 \implies f'(c)-m = 0 \implies f'(c) = m$$
$$\implies f'(c) = \frac{f(b)-f(a)}{b-a} \ \ \ \ \ \square$$
