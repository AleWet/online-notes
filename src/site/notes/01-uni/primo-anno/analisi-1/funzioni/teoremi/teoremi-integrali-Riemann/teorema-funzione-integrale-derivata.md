---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/analisi-1/funzioni/teoremi/teoremi-integrali-riemann/teorema-funzione-integrale-derivata/","tags":["math","uni"]}
---

sia $f:[a,b] \to \mathbb{R}$ tale che $f \in R(a,b)$ (guarda [[01-uni/primo-anno/analisi-1/funzioni/definizioni/def-primitiva#notazione interna al corso\|qui per definizione]]) e sia $I(x)$ la [[01-uni/primo-anno/analisi-1/funzioni/definizioni/def-funzione-integrale\|funzione integrale]] di $f$ allora se $f$ è continua in $x_0 \in [a,b]$ avrò che:
$$I(x) \text{ è derivabile in } x_{0}$$
$$I'(x_{0}) = f(x_{0})$$
$$\implies \left[ \int_{a}^{x_{0}} f(t)dt \right]' = f(x_{0}) $$
### corollario importante
se $f$ è continua su tutto $[a,b]$ avrò che :
$$\forall x \in [a,b], I'(x) = f(x)$$
allora mettendo insieme questa conclusione a [[01-uni/primo-anno/analisi-1/funzioni/teoremi/teoremi-funzioni-continue/teorema-funzione-continua-integrabile\|questo teorema]] si ha che:
$$\text{ se } f \ \text{ è continua } \implies f \in R_{P}(a,b)$$
### osservazione del corollario
non è vero che se $f \in R_{P}(a,b) \implies f$ è continua, un esempio è 
$$F:[0,1] \to \mathbb{R}$$
$$F(x) = \begin{cases}
x^2\sin\left( \frac{1}{x} \right) & x \ne {0} \\ \\
0  & x=0
\end{cases}$$
$$f(x) = \begin{cases}
2x\sin\left( \frac{1}{x} \right) -\cos\left( \frac{1}{x} \right)  & x\ne 0 \\ \\
0 & x=0
\end{cases}$$
$f$ ha un solo punto di [[01-uni/primo-anno/analisi-1/funzioni/definizioni/def-punti-discontinuità#discontinuità di II specie\|discontinuità di seconda specie]] e altrove è continua quindi [[01-uni/primo-anno/analisi-1/funzioni/teoremi/teoremi-integrali-Riemann/teorema-finite-discontinuità-integrabile-(tbf)\|è integrabile]], inoltre $f$ ammette primitiva (la $F$) e quindi $f \in R_P(a,b)$.
### dim
sia $x_{0} \in [a,b]$, mostrerò che $I_{+}'(x_{0}) = f(x_{0})$, la dimostrazione per la derivata sinistra è analoga.
fissato $\varepsilon>0$
$$\exists \delta > 0 : |x_{0}-t|<\delta \implies |f(x_{0})-f(t)|<\varepsilon$$
dalla definizione di [[01-uni/primo-anno/analisi-1/funzioni/definizioni/def-continuità\|continuità]]. Sia poi $h>0$ e definisco la seguente quantità:
$$\star :=\left| \frac{{I(x_{0}+h)-I(x_{0})}}{h} - f(x_{0}) \right|$$
voglio dimostrare che se 
$$\exists \delta>0 : 0<h<\delta \implies \star<\varepsilon$$
in pratica se $h$ è abbastanza piccolo allora la derivata $I_{+}'(x_{0})$ e $f(x_{0})$ si avvicinano arbitrariamente.
$$\star = \left| \frac{{\int_{a}^{x_{0+h}}f(t)dt - \int_{a}^{x_{0}} f(t)dt}}{h} - f(x_{0}) \right|$$
e usando l'[[01-uni/primo-anno/analisi-1/funzioni/teoremi/teoremi-integrali-Riemann/teorema-additività-integrale\|additività integrale]]:
$$= \left| \frac{1}{h} \int_{x_{0}}^{x_{0}+h}[f(t)dt] - f(x_{0}) \right|$$
a questo punto noto che 
$$f(x_{0}) = \bigg[\frac{1}{h}\int_{x_{0}}^{x_{0}+h}f(x_{0})dt\bigg] = \bigg[\frac{f(x_{0})}{h}\int_{x_{0}}^{x_{0}+h}dt \bigg] = \frac{f(x_{0})}{h}*h$$
$$\implies \star= \left| \frac{1}{h} \int_{x_{0}}^{x_{0}+h}[f(t)-f(x_{0})]dt \right|$$
usando la [[01-uni/primo-anno/analisi-1/funzioni/teoremi/teoremi-integrali-Riemann/teorema-linearità-integrale\|linearità dell'integrale]]
$$\implies \star\leq \frac{1}{h} \int_{x_{0}}^{x_{0} h} |f(t)-f(x_{0})|dt$$
usando il [[01-uni/primo-anno/analisi-1/funzioni/teoremi/teoremi-integrali-Riemann/teorema-disuguaglianza-modulo\|teorema-disuguaglianza-modulo]]. Qui noto che se $h<\delta$ e se $t \in [x_{0}, x_{0}+h]$ 
$$\implies|t-x_{0}|<h<\delta \implies|f(t)-f(x_{0})|<\varepsilon$$
$$\implies \left| \frac{I(x_{0}+h)-I(x_{0})}{h} - f(x_{0})\right| \leq \frac{1}{h}  \int_{x_{0}}^{x_{0} h} |f(t)-f(x_{0})|dt \leq \frac{1}{h} \int_{x_{0}}^{x_{0}+h}\varepsilon = \frac{1}{h}\varepsilon h = \varepsilon$$
usando il [[01-uni/primo-anno/analisi-1/funzioni/teoremi/teoremi-integrali-Riemann/teorema-confronto-integrali\|teorema-confronto-integrali]]. Ho quindi dimostrato che:
$$\star \leq \varepsilon$$
$$\implies I_{+}'(x_{0}) = f(x_{0}) \ \ \ \ \ \square $$
