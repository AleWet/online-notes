---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/analisi-1/serie/teoremi/criterio-leibnitz/","tags":["math","uni"],"updated":"2026-01-05T09:25:10.869+01:00"}
---

$$\text{sia } \sum_{n=0}^{+\infty}a_n$$
$$dove \ a_n = (-1)^n*b_n \ \land \ b_n\downarrow0$$
quindi se :  $b_n \ge 0 \ , b_n \rightarrow0 \ ,b_{n+1} \le b_n$
$$\tag*{prima conclusione}\text{allora }\begin{equation}
   {\textstyle \sum_n^{+\infty}}a_n
\end{equation} \text{ converge}$$
$$\tag*{seconda conclusione} \text{allora } |S_n - S|\le b_{n+1} \text{ per } n\ne0 $$
### osservazioni
 - $b_n$ basta che sia decrescente definitivamente
 - la serie può partire anche da $0$ o $n_0$ è uguale
 - è anche possibile che  $b_n\uparrow0$ 
 - caso speciale del [[01-uni/primo-anno/analisi-1/serie/teoremi/criterio-Dirichlet\|criterio-Dirichlet]]
### ==dim== 
sul QR2 non banale:
$$\text{sia } S_n \text{ la successione delle somme parziali di } a_n$$
$$S_{2n} = b_0-(b_1-b_2)-(b_3-b_4)-...-(b_{2n-1}-b_{2n})$$
$$S_{2n+1} = (b_0-b_1)+(b_2-b_3)+...+(b_{2n}-b_{2n+1})$$
e tu sai che $b_n > b_{n-1} \ \forall n$ e che quindi $S_{2n} \downarrow \land \ S_{2n+1}\uparrow$. 
Inoltre : 
$$S_{2n} > S_{2n+1} \ \forall n $$
questo perché $S_{2n} - S_{2n+1} = + a_{2n+1} > 0 \text{ (esponente dispari)}$.
Inoltre ti viene che $a_n \rightarrow 0$ ([[01-uni/primo-anno/analisi-1/successioni/definizioni/def-successione-infinitesima\|infinitesima * limitata = infinitesima]]).
di conseguenza puoi usare il [[01-uni/primo-anno/analisi-1/successioni/teoremi/teorema-cuoricino\|teorema-cuoricino]] che ti dice che :
$$\lim S_{2n} =\lim S_{2n+1} = l \in \mathbb{R}$$
$$\implies S_n \rightarrow l \text{ poiché tutti i itermini convergono a }l$$

adesso posso trovare la stima della somma rispetto al limite :
$$|S_{2n} - S_{2n+1}| =|a_{2n+1}|$$
$$|S_{2n} - S| \le |S_{2n} - S_{2n+1}| = b_{2n+1} \text{ (decrescente sopra il limite)}$$
(Lo stesso ragionamento può essere fatto per la successione crescente sotto il limite tanto è con il valore assoluto, trovi lo stesso risultato sempre minorato dal termine a sinistra qui sopra)
$$|S_n-S|<b_{n+1}$$

