---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/analisi-1/funzioni/teoremi/teoremi-funzioni-continue/teorema-degli-zeri/","tags":["math","uni"]}
---

sia $f : [a,b] \to \mathbb{R}$ [[01-uni/primo anno/analisi 1/funzioni/definizioni/def-continuità\|continua]] (definita e continua su tutto l'intervallo $[a,b]$)
$$\text{se } f(a)*f(b) <0 \implies \exists \ c \in (a,b) : f(c) = 0$$
ciò ti dice anche che $f(a), f(b) \ne 0$ se no la prima condizione non è verificata.
### dim 1 (brutta)
metodo di bisezione, fai una ricerca binaria con $c = \frac{a+b}{2}$ e riesci a trovare il tuo punto di $0$ con precisione arbitraria.
### dim 2 
$$f(a) > 0,\ \ f(b) <0$$
$$P = \{x \in [a,b] : f(x) > 0\}$$
$\text{ noto che : }$
1) $P \ne \emptyset$ poiché $f(a) \in P$
2) $P \text{ è superiormente limitato}$ 
3) $\exists \ c = supP \in [a,b]$ per la [[01-uni/primo anno/analisi 1/basi successioni/definizioni/def-assioma-completezza\|completezza di R]]
$$\text{allora abbiamo dimostrato che } \exists P_n \in P : P_n \to c\tag{*}$$
$$\text{dalla continuità }\implies f(P_n) \to f(c)$$
$$\text{ma } f(P_n) >0 \text{ per come ho definito l'insieme }P$$
$$\implies f(c) \ge 0 \text{ per permanenza del segno}$$
$$\text{notiamo che } c<b$$
$$\text{prendo una qualsiasi }X_n := c+\frac{1}{n} \ \forall n$$
$$X_n \ge c \ \land\ X_n \to c$$
$$X_n \not\in P \text{ poiché sono tutti gli elementi "dopo" il sup che non possono} \in P$$
$$\implies f(X_n) \le0 \ \land f(X_n) \to f(c) \implies f(c) \le 0 \text{ permanenza del segno}$$
$$\implies f(c) \ge 0 \land f(c) \le 0 \implies f(c) = 0$$
$$(*)  \text{ guarda problema 2 del parziale del 2024} : \gamma- \frac{1}{n}\le a_n \le \gamma$$