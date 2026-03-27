---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/analisi-1/funzioni/teoremi/teoremi-funzione-derivata/teorema-derivata-monotonia/","tags":["math","uni"],"updated":"2026-01-09T17:21:34.622+01:00"}
---

sia $f:[a,b] \to \mathbb{R}, f$ soddisfa le ipotesi di [[01-uni/primo-anno/analisi-1/funzioni/teoremi/teoremi-funzione-derivata/teorema-Lagrange-(tbf)\|Lagrange]] $\implies$
$$f(x) \text{ è crescente } \iff f'(x) \ge0 \ \forall\  x\in (a,b)$$
$$f(x) \text{ è decrescente} \iff f'(x) \le 0 \ \forall \ x \in (a,b)$$
### osservazione 1
non è vero che se $f \text{ è setrettamente crescente } \implies f'(x) > 0$, un esempio è $f(x) = x^3$. Si può fare la stessa osservazione per $f \text{ strettamente decrescente}$. 
### corollario
$$f \text{ è costante} \iff f'(x) = 0$$
### dim $\Rightarrow$ 
siano $x<y$ con $x,y \in [a,b]$ voglio mostrare che $f(x) \le f(y)$.
Inizio applicando [[01-uni/primo-anno/analisi-1/funzioni/teoremi/teoremi-funzione-derivata/teorema-Lagrange-(tbf)\|Lagrange]] a $f$ sull'intervallo $[x,y]$
$$\implies \exists c \in (x,y) : \frac{f(y)-f(x)}{y-x}=f'(c)$$
$$\implies f'(c)(y-x) = f(y)-f(x)$$
$$y-x > 0, \ f'(c) \ge 0 \implies f(y)-f(x) \ge 0 \ \ \ \ \square$$
ovvero stai dicendo che per ogni due numeri $x,y$ appartenenti all'intervallo di partenza, passando per Lagrange, $f(y) \ge f(x) \iff f'(c) \ge 0$.
### dim $\Leftarrow$ 
questa è la parte più interessante del teorema poiché ci dice fornisce informazioni riguardo la funzione originale studiandone la derivata:
sia $x \in (a,b)$ so che $f$ è [[01-uni/primo-anno/analisi-1/funzioni/definizioni/def-derivata#derivabilità\|derivabile]] in $x$ per ipotesi e quindi
$$f'_+(x) = f'(x)$$
$$f'_+(x) = \lim_{h\to 0+} \frac{f(x+h)-f(x)}{h} \ \ \text{dove } h>0 \ \text{ e} \ \ f(x+h)-f(x) \ge0 $$
$$\implies f'_+(x) \ge0 \implies f'(x) \ge 0 \text{ usando il teorema della permanenza del segno}$$
### dim corollario 
questo segue dal fatto che una funzione costante è contemporaneamente *crescente* e *decrescente* ricordando che crescente e decrescente impongono $\ge, \le$ non disuguaglianza stretta,
$$\implies f'(x) \ge0 \ \land f'(x) \le0 \implies f'(x) = 0 \ \ \ \square$$
questa cosa si può dimostrare anche per assurdo nel seguente modo:
siano due punti $x,y$ t.c. $f(x) \ne f(y)$ allora:
$$\exists c \in (x,y) : \frac{f(x)-f(y)}{y-x} = f'(c)$$
e per ipotesi $x \ne y, \ f(x) \ne f(y) \implies f'(c) \ne 0$ il che è assurdo.
