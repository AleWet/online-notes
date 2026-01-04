---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/analisi-1/funzioni/definizioni/def-punti-discontinuita/","tags":["math","uni"]}
---

# punti di discontinuità
un punto $x_0 \in D(f)$ è detto *punto di discontinuità* per $f$ se $f$ non è [[01-uni/primo-anno/analisi-1/funzioni/definizioni/def-continuità\|continua]] in $x_0$ : 
$$\lim_{x \to x_0} f(x) \ne f(x_0)$$
### osservazione importante
questa definizione sottintende che $x_0$ è un [[01-uni/primo anno/analisi 1/basi funzioni/definizioni/def-punti-accumulazione-and-others#punti di accumulazione\|punto di accumulazione]] per l'insieme $D(f)$ se no l'operazione di "check" che la funzione non è continua non è neanche implementabile, non ha senso fare il limite. Anzi  se $x_0$ fosse un punto isolato per $D(f)$ avremmo che $f$ è continua in $x_0$.
___
# discontinuità eliminabile (III specie)
$x_0$ è punto di *discontinuità eliminabile* se
$$\exists \text{ FINITO } \lim_{x \to x_0} f(x) \text{ ma }\ne f(x_0)$$
Si dice eliminabile poiché se definisco
$$f(x_0) := \lim_{x \to x_0} f(x) \text{ ottengo una funzione continua in } x_0$$ 
### esempio
$$f(x) = \cases{ \frac{sin(x)}{x} \ \ x\ne0 \\ \\ 0  \  \ \ \ \ \ \  \ \ \ x = 0}$$
___
# discontinuità di tipo salto (I specie)
$x_0$ è punto di discontinuità di *tipo salto* se
$$\exists \lim_{x^+ \to x_0} f(x), \exists \lim_{x^- \to x_0} f(x)$$
$$\text{ma sono diversi tra loro} $$
### esempio
$$f(x) = \cases{ 1 \ \ x>0 \\ \\ 0  \ \ \ x = 0 \\ \\ -1 \ \ \ x<0}$$
___
# discontinuità di II specie
quando uno tra i limiti (destro o sinistro) o entrambi non esistono o valgono $\pm\infty$
### esempio
$$f(x) = \cases{ \frac{1}{x} \ \ x>0 \\ \\ 0     \ \ \ x \le 0}$$
