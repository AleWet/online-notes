---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/analisi-1/funzioni/teoremi/teoremi-taylor/teorema-taylor-peano/","tags":["math","uni"]}
---

sia $f$ [[01-uni/primo-anno/analisi-1/funzioni/definizioni/def-polinomio-Taylor\|polinomio di Taylor]] di ordine $n$ centrato in $x_0$ allora:
$$\lim_{x \to x_0} \left[\frac{f(x)-P_n(x)}{(x-x_0)^n} \right] = 0$$
in pratica sto dicendo che nell'approssimare $f$ con il "politaylor" di grado $n$ sto commettendo un errore ma più alto è il grado del "politaylor" più piccolo è l'errore. è più chiaro se lo scrivi con $h = x-x_{0}$ :
$$f(x_0+h) = \sum_{k = 0}^n \left[ \frac{f^{k}(x_0)}{k!}h^n \right] + h^nw(h)$$
$$w(h) \to 0 \ \text{ if } \ h \to 0 $$
$$\lim_{h\to0} \frac{h^nw(h)}{h^n} = 0 \implies h^nw(h) = o(h^n)$$
$$\implies f(x_0+h)-P_n(x_0+h) = o(h^n)$$
il che ti dice che, preso $x_0 = 0$ per semplicità, quando $x \to 0$ l'errore che stai commettendo nel dire che $P_n(x) = f(x)$ è più piccolo di $x^n$.
### resto di Peano
Se prendi $h^nw(h)$ dal punto precedente, questo si chiama *resto di Peano* e, come già detto, mi dice che sto migliorando la mia approssimazione di grado in grado. Prendi l'approssimazione del [[01-uni/primo-anno/analisi-1/successioni/definizioni/def-asintotico\|asintotico]], lì avevi un errore che scalava più che "lineare" o grado $1$, Taylor invece di permette di arrivare ad un errore "arbitrariamente" piccolo. 
### osservazione 1
Sempre riguardo la [[01-uni/primo-anno/analisi-1/funzioni/definizioni/def-differenziabilità\|differenziabilità]], si può osservare che il primo ordine di Taylor è esattamente la definizione di differenziabilità:
$$f(x_0+h) = f(x_0) +f'(x_0)(x-x_0)+hw(h)$$
che è il polinomio di Taylor di grado $1$.
### osservazione 2
Se provi ad usare Taylor sulla funzione esponenziale in $x_0 = 0$ troverai esattamente la successione delle somme parziali della [[01-uni/primo-anno/analisi-1/serie/definizioni/def-serie-fattoriale\|serie fattoriale]].
### osservazione 3
Se ho un polinomio $P_{n}(x)$ di grado $\le n$ tale che (prendendo $x_{0}=0$) :
$$ \frac{P_{n}(x)-f(x)}{x^n} \to 0$$
non posso sempre trovare questo "polibello" con la procedura di Taylor poiché essa è sufficiente e non necessaria. Esempio : $f(x) = x^3\sin\left( \frac{1}{x} \right)$ per cui $\not \exists \ f''(0) \implies \not\exists P_{taylor}(x)$ ma se prendo $Q(x) = 0$ questo è un "polibello" che funziona con il $grado-2$ :
$$\lim_{x\to 0} \frac{f(x)-Q(x)}{x^2} = \lim_{ x \to 0 } \frac{f(x)}{x^2} =0$$
ho quindi trovato un "polibello" di $\text{ordine 2}$ ma non esiste un "politaylor" di $\text{ordine 2}$.
### dim
ipotesi : prendo $x_{0} = 0$ per semplicità, $f$ è [[01-uni/primo-anno/analisi-1/funzioni/definizioni/def-derivata#derivabilità\|derivabile]] $n$ volte in $0$, allora :
$$P(x) = \sum_{k=0}^n \frac{f^{(k)}(0)}{k!}(x-0)^k$$
definisco $g(x)$ come:
$$g(x):=f(x)-P_{n}(x)$$
e voglio dimostrare che :
$$\lim_{ x \to 0 } \frac{g(x)}{x^n} = 0$$
per fare ciò analizzo $\lim_{ x \to 0^+ }$ e per $\lim_{ x \to 0^- }$ la dimostrazione è analoga come sempre:
sia $x$ sufficientemente piccolo t.c. $f,f',f'',f''',...,f^{n-1}$ siano tutte definite in $[0,x]$.
Noto che 
$$g(0) = g'(0) = g''(0) = g'''(0) = g^{(n)}(0) = 0$$
$$f(0)-P_{n}(0)=0$$
$$f'(0)-P'_{n}(0)=0$$
$$\dots.$$
$$f(0)^{(n)}-P_{n}^{(n)}(0)=0$$
a questo punto il Pata ha detto che si dovrebbe procedere per induzione ma è uguale se non lo fai, quindi non lo farai all'esame:
applico il [[01-uni/primo-anno/analisi-1/funzioni/teoremi/teoremi-funzione-derivata/teorema-Lagrange-(tbf)\|teorema-Lagrange-(tbf)]] su $g$ nell'intervallo $[0,x$] 
$$\implies \exists x_{1} \in (0,x):g(x)-g(0) = g'(x_{1})(x-0) = g'(x_{1})x$$
$$\implies g(x) = g'(x_{1})x$$
applico di nuovo Lagrange a $g'$ nell'intervallo $[0,x_{1}]$ 
$$\implies \exists x_{2} \in (0,x_{1}):g'(x_{1})-g'(0) = g''(x_{2})x_{1}$$
$$\implies g'(x_{1})-0 = g''(x_{2})x_{1}$$
$$g'(x_{1}) = g''(x_{2})x_{1}$$
$$\implies g(x) = g''(x_{2})x_{1}x$$
a questo punto applico Lagrange finché non arrivo allo "step" $n-2$ :
$$\exists x_{n-1}\in(0,x_{n-2}):g^{(n-2)}(x_{n-2})-0 =g^{(n-1)}(x_{n-1})x_{n-2}$$
a differenza degli altri passaggi, non so se $g^{(n-1)}$ è derivabile su tutto l'intervallo $[0,x_{n-1}]$. Nelle ipotesi avevo che $f$ è derivabile $n$ volte in $x_0 = 0$ ma questo non mi garantisce che $f$ sia derivabile in tutto un intorno $u(0)$ $n$ volte, potrei avere la derivata $n-esima$ solo in $0$ e non averla per tutti gli altri punti (esistono funzioni continue in $u(x_{0})$ ma derivabili solo in $x_{0}$). 
Devo quindi cambiare approccio e usare la [[01-uni/primo-anno/analisi-1/funzioni/definizioni/def-differenziabilità\|differenziabilità]] di $g^{(n-1)}$ in $0$ 
$$g^{n-1} (t) = g^{(n-1)}(0) + g^n(0)(t-0) + o(t-0)$$
e la applico a $x_{n-1}$ ottenendo : 

$$g^{(n-1)} (x_{n-1}) = g^{(n-1)}(0) + g^n(0)(x_{n-1}) + o(x_{n-1}) $$
$$\implies g^{(n-1)}(x_{n-1}) = o(x_{n-1}) = x_{n-1}\omega (x_{n-1})$$
dove $\omega (x_{n-1})$ è una generica funzione che tende a $0$ quando $x \to x_{n-1}$.
Mettendo insieme tutte le espressioni ottieni:
$$g(x) = g'(x_{1})x$$
$$g(x) =  g''(x_{2})x_{1}x$$
$$g(x) = g'''(x_{3})x_{2}x_{1}x$$
$$\dots$$
$$g(x) = x_{n-1}\ \omega(x_{n-1})\ x_{n-2}x_{n-3}x_{n-4}\dots x_{2}x_{1}x$$
$$\implies g(x) = x^n \frac{{x_{n-1} x_{n-2}x_{n-3}x_{n-4}\dots x_{2}x_{1}x}}{x^n} * \omega(x_{n-1})$$
il termine con la frazione noto che è completamente contenuto tra $0$ e $1$ facendo il seguente ragionamento:
$$c := \frac{x_{n-1}}{x} \frac{x_{n-2}}{x}\dots \frac{x_{2}}{x} \frac{x_{1}}{x}1$$
e seguendo tutte le applicazioni del teorema di Lagrange so che $x_{n-1}<x_{n-2}<\dots<x$ di conseguenza $c \in (0,1)$ perché tutti i membri sono compresi tra $0$ e $1$.
$$\implies \frac{g(x)}{x^n} =  c  \ \frac{{x^n \omega(x_{n-1})}}{x^n} = c \omega (x_{n-1})$$
e noto che quando $x \to 0^+$ anche $x_{n-1} \to 0^+$ sempre per il discorso degli intervalli del teorema di Lagrange usando il [[01-uni/primo-anno/analisi-1/successioni/teoremi/teorema-del-confronto\|teorema-del-confronto]], ottengo quindi il seguente limite : 
$$\lim_{ x \to 0^+ }c \omega(x_{n-1}) = 0 $$
