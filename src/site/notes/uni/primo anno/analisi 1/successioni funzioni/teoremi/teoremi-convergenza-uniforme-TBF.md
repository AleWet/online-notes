---
{"dg-publish":true,"permalink":"/uni/primo-anno/analisi-1/successioni-funzioni/teoremi/teoremi-convergenza-uniforme-tbf/","tags":["math","uni"]}
---

guarda qui per def di [[uni/primo anno/analisi 1/successioni funzioni/definizioni/def-successione-funzioni#convergenza uniforme\|convergenza uniforme]], la notazione usata è $f_{n} \xrightarrow{u}f$.
### teorema 1 continuità
sia $f_n:I \to \mathbb{R}$ una [[uni/primo anno/analisi 1/successioni funzioni/definizioni/def-successione-funzioni\|successione di funzioni]] t.c. $\forall n, \ f_{n}$ è [[uni/primo anno/analisi 1/funzioni/definizioni/def-continuità\|continua]] allora 
$$\text{ se } f_{n} \xrightarrow{u} f \implies f \text{ è continua}$$
### teorema 2 integrabilità
Per la definizione di Riemann-integrabile guarda [[uni/primo anno/analisi 1/funzioni/definizioni/def-integrale-Riemann-TBF\|qui]].
Sia $I$ un intervallo **[[uni/primo anno/analisi 1/basi funzioni/definizioni/def-insiemi-aperti-chiusi#insieme chiuso\|chiuso]] e limitato** e sia $f_{n}:[a,b] \to \mathbb{R}$ e $\forall {n} \in R(a,b)$ allora
$$\text{ se } f_{n} \xrightarrow{u} $$
$$\tag{1} f \in R(a,b)$$
$$\tag{2} \lim_{ n \to \infty } \int_{a}^b |f_{n}(x)-f(x)|dx \to 0$$
### osservazione importante
la proprietà $(2)$ ti dice che puoi portare il "limite" dentro l'integrale, cioè:
$$\int_{a}^b \bigg|f_{n}(x)-f(x)\bigg|dx \ge \bigg| \int_{a}^b \big[f_{n}(x)-f(x)\big]dx \bigg|$$
usando la [[uni/primo anno/analisi 1/funzioni/teoremi/teoremi integrali Riemann/teorema-disuguaglianza-modulo\|disuguaglianza del modulo]]
$$= \bigg| \int_{a}^b f(x)dx -\int_{a}^b f_{n}(x)dx\bigg|$$
usando la [[uni/primo anno/analisi 1/funzioni/teoremi/teoremi integrali Riemann/teorema-linearità-integrale-TBF\|linearità dell'integrale]]
$$\implies \lim_{ n \to \infty } \int_{a}^b f_{n}(x)dx = \int^a_{b}\lim_{ n \to \infty }f_{n}(x)dx = \int_{a}^b f(x)dx$$
ma questa proprietà (quella di portare "dentro o fuori" il limite $n\to \infty$) è **più debole di quella di partenza**, per più dettagli e un esempio guarda QR5.
### teorema 3 derivabilità

