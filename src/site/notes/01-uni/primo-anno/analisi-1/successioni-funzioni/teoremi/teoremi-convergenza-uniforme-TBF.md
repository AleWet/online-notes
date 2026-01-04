---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/analisi-1/successioni-funzioni/teoremi/teoremi-convergenza-uniforme-tbf/","tags":["math","uni"]}
---

wguarda qui per def di [[01-uni/primo anno/analisi 1/successioni funzioni/definizioni/def-successione-funzioni#convergenza uniforme\|convergenza uniforme]], la notazione usata è $f_{n} \xrightarrow{u}f$.
### teorema 1 continuità
sia $f_n:I \to \mathbb{R}$ una [[01-uni/primo anno/analisi 1/successioni funzioni/definizioni/def-successione-funzioni\|successione di funzioni]] t.c. $\forall n, \ f_{n}$ è [[01-uni/primo anno/analisi 1/funzioni/definizioni/def-continuità\|continua]] allora 
$$\text{ se } f_{n} \xrightarrow{u} f \implies f \text{ è continua}$$
___
### teorema 2 integrabilità
Per la definizione di Riemann-integrabile guarda [[01-uni/primo anno/analisi 1/funzioni/definizioni/def-integrale-Riemann-TBF\|qui]].
Sia $I$ un intervallo **[[01-uni/primo anno/analisi 1/basi funzioni/definizioni/def-insiemi-aperti-chiusi#insieme chiuso\|chiuso]] e limitato** e sia $f_{n}:[a,b] \to \mathbb{R}$ e $\forall {n} \in R(a,b)$ allora
$$\text{ se } f_{n} \xrightarrow{u} f$$
$$\tag{1} f \in R(a,b)$$
$$\tag{2} \lim_{ n \to \infty } \int_{a}^b |f_{n}(x)-f(x)|dx \to 0$$
### osservazione importante
la proprietà $(2)$ ti dice che puoi portare il "limite" dentro l'integrale, cioè:
$$\int_{a}^b \bigg|f_{n}(x)-f(x)\bigg|dx \ge \bigg| \int_{a}^b \big[f_{n}(x)-f(x)\big]dx \bigg|$$
usando la [[01-uni/primo anno/analisi 1/funzioni/teoremi/teoremi integrali Riemann/teorema-disuguaglianza-modulo\|disuguaglianza del modulo]]
$$= \bigg| \int_{a}^b f(x)dx -\int_{a}^b f_{n}(x)dx\bigg|$$
usando la [[01-uni/primo anno/analisi 1/funzioni/teoremi/teoremi integrali Riemann/teorema-linearità-integrale-TBF\|linearità dell'integrale]]
$$\implies \lim_{ n \to \infty } \int_{a}^b f_{n}(x)dx = \int^a_{b}\lim_{ n \to \infty }f_{n}(x)dx = \int_{a}^b f(x)dx$$
ma questa proprietà (quella di portare "dentro o fuori" il limite $n\to \infty$) è **più debole di quella di partenza**, per più dettagli e un esempio guarda QR5.
___
### teorema 3 derivabilità
siano $f_n$ derivabili in $[a,b]$ e supponiamo che:
- $\exists \text{ una funzione } g \text{ tale che } g:[a,b] \to \mathbb{R} : f_{n}' \xrightarrow{u} g$
- $\exists \ x_{0} \in [a,b] : f_{n}(x_{0}) \to l \in \mathbb{R}$
$$\text{allora si ha che } f_{n} \xrightarrow{u} f, \ f:[a,b]\to \mathbb{R}$$
$$\text{ inoltre si ha che } f \text{ è derivabile e } f' = g$$
in pratica stai dicendo che, come negli altri teoremi, puoi prendere il limite "dentro" l'operazione di derivata:
$$\lim_{ n \to \infty } f'_{n}(x) = (\lim_{ n \to \infty } f_{n})'$$
### osservazione importante
perché è importante il presupposto 2 ($\exists x_{0} : f_{n}(x) \to l$)? 
Perché l'operazione di derivazione "toglie" informazioni sulle costanti della funzione originale, di conseguenza se avessi delle costanti che farebbero divergere la funzione originaria il teorema non sarebbe verificato $\implies$ ci deve essere almeno un punto che rimane limitato al limite
___
# dimostrazione
### dim teorema 1
Fisso un generico punto $x_0 \in I$ e dimostrerò che $f$ è continua in $x_{0}$.
fisso $\varepsilon > 0$ arbitrario e poiché $f_{n} \xrightarrow{u} f$ so che $\exists n_{0} \in \mathbb{N} :$
$$|f_{n}(x) - f(x)| \leq \varepsilon \ \ \forall x \in I$$
adesso uso la continuità di $f_{n}$ e quindi so che $f_{n_{0}}$ è **continua**:
$$\exists \ \delta > 0 : \text{ se } |x - x_{0}| < \delta \ \land x \in I$$
$$\implies |f_{n_{0}}(x) - f_{n_{0}}(x_{0})| < \varepsilon$$
$$|f(x) - f(x_{0})| = |f(x)-f_{n_{0}}(x) + f_{n_{0}}(x) - f_{n}(x_{0})+f_{n}(x_{0}) - f(x_{0})|$$
$$\leq |f(x)-f_{n_{0}}(x)| + |f_{n_{0}}(x) - f_{n_{0}}(x_{0})| + |f_{n_{0}}(x_{0}) - f(x_{0})| \leq 3\varepsilon$$
$$(i) \ \ \ \ \ \ f_{n}(x) \to f(x) \ \text{ convergenza puntuale}$$
$$(ii) \ \ \ \\ \ \ \ \  \ \ \ \ \ f_{n_{0}}(x) \to f_{n_{0}}(x_{0}) \ \text{ per continuità }$$
$$(iii) \ \ f_{n_{0}}(x_{0}) \to f(x_{0})  \ \text{ convergenza puntuale}$$
$$\implies |f(x)-f(x_{0})| \leq 3\varepsilon \ \text{ con } \varepsilon \text{ arbitrario} \ \ \ \ \ \ \ \square$$
### dim teorema 2
il punto $(1)$ non verrà dimostrato, prendiamo quindi per vero che $f \in R(a,b)$, allora:
$$\int_{a}^b |f_{n}(x)-f(x)|dx \leq \int_{a}^b \sup_{t \in I}|f_{n}(t)-f(t)|dt$$
$$= (b-a) \sup_{t \in I} |f_{n}(t)-f(t)|$$
$$\text{ ma so che per convergenza uniforme : } |f_{n}(t) - f(t)| \to 0 \ \forall t$$
$$\implies \int_{a}^b |f_{n}(x)-f(x)|dx \to 0$$
### dim teorema 3 TBF
anche questa dimostrazione è semplificata e assumiamo per vero che $f_{n} \in C^1([a,b])$ (guarda [[01-uni/primo anno/analisi 1/funzioni/definizioni/def-classi-di-continuità\|qui]]) e quindi che le derivate sono continue su $[a,b]$ e supponiamo anche di prendere $x_{0} = a$ per comodità, la dimostrazione per gli altri punti è analoga:
$$f_{n}(x) = f_{n}(a) + \int _{a}^x f'_{n}(t)dt$$
usando il [[01-uni/primo anno/analisi 1/funzioni/teoremi/teoremi integrali Riemann/teorema-fondamentale-del-calcolo\|01-uni/primo anno/analisi 1/funzioni/teoremi/teoremi integrali Riemann/teorema-fondamentale-del-calcolo]] e il fatto che $f_{n}\in C^1([a,b])$ e [[01-uni/primo anno/analisi 1/funzioni/teoremi/teoremi funzioni continue/teorema-continua-integrabile\|quindi essa è integrabile]]. Definisco poi $l := \lim_{ n \to \infty } f_{n}(a)$ : 
$$f(x) = l + \int_{a}^xg(t)dt$$
osservo poi che grazie al **TEOREMA 1** enunciato qui sopra, $g$ è continua su $[a,b]$.
a questo derivo $f$ e trovo:
$$f'(x) = \left[ \int_{a}^x g(t)dt \right]' = g(x)$$
