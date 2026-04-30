---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/analisi-1/funzioni/definizioni/def-integrale-improprio-tbf/","tags":["math","uni"],"updated":"2026-02-24T15:52:00.481+01:00"}
---

### ipotesi
- $f:(a,b) \to \mathbb{R}$ , dove : $-\infty \le a \le b \le +\infty$
- $f$ è **LOCALMENTE** integrabile, cioè $\forall [c,d] \in (a,b) \text{ si ha che } f \in R(c,d)$.
### definizione intervallo unico
Di conseguenza non integro $f$ direttamente sul mio intervallo brutto $(a,b)$ ma su $[c,d]$ dove per ipotesi $f \in R(c,d)$ e applico un **DOPPIO LIMITE**:
$$\lim_{\begin{smallmatrix} d \to b & \\ c \to a \end{smallmatrix}} \int_{c}^d f(x)dx$$
se questo limite $\exists$ **FINITO** diciamo che $f$ è integrabile impropriamente su $(a,b)$. Poi però verrà data un'altra definizione di localmente integrabile che si basa su questa, guarda fine di questa nota per più dettagli.
### notazione interna al corso
diciamo che una funzione è integrabile impropriamente su un intervallo $(a,b)$ come:
$$f \in I(a,b)$$
quindi come una [[01-uni/primo-anno/analisi-1/funzioni/definizioni/def-classi-di-continuità\|classe]] di funzioni come quelle di Riemann.
### osservazioni importante 1
1) se $a = -\infty$ oppure $b = \infty$ o entrambi avrò $(a,b)$ non limitato e quindi non posso implementare la procedura di Riemann direttamente. 
2) Può anche essere che $f$ non sia limitata nell'intervallo $(a,b)$ e anche questa è un'ipotesi della procedura dell'[[01-uni/primo-anno/analisi-1/funzioni/definizioni/def-integrale-Riemann\|integrale di Riemann]].
### osservazione importante 2
Nell'applicare il limite doppio bisogna fare attenzione, non bisogna prendere una "velocità di convergenza" a caso, dimostrare che è finito e basta, ma bisogna dire PER OGNI "velocità" arbitraria con cui ci si avvicina al limite devo trovare sempre lo stesso risultato:
$$\forall a_{n},b_{n} \in D(f) : a_{n}\to a^+, b_{n}\to b^-$$
$$\lim_{ n \to \infty } \int_{a_{n}}^{b_{n}} f(x)dx = l \in \overline{\mathbb{R}}$$
il seguente esempio spiega chiaramente questo concetto:
$$\int_{-1}^1f(x)dx,\ \ f(x) = \frac{2x}{1-x^2} $$
$$I = \lim_{ \varepsilon \to 0 } \int_{-1+\varepsilon}^{1+\varepsilon}f(x)dx$$
$$f \text{ è dispari }\implies I = 0$$
se prendo però una "velocità" di convergenza diversa da una parte e dall'altra ottengo:
$$I = \int_{-1+\varepsilon}^{1-\varepsilon^2}f(x)dx$$
e se lo risolvi ottieni che con $\varepsilon \to 0, I = +\infty$ e concludo (uguale alla [[01-uni/primo-anno/analisi-1/funzioni/definizioni/def-continuità#continuità successionale\|continuità successionale]]) che il limite doppio non esiste.
### osservazione 3
Negli esercizi spesso non ti viene richiesto di calcolare il valore dell'integrale ma il comportamento (uguale al discorso fatto con le [[01-uni/primo-anno/analisi-1/serie/definizioni/def-serie\|serie]]). se invece ti chiedono di calcolare l'integrale improprio è esattamente la stessa cosa di un integrale definito solo con uno o più limiti agli estremi.
### osservazione 4
Una [[01-uni/primo-anno/analisi-1/serie/definizioni/def-serie\|serie]] è semplicemente un integrale improprio speciale definito a tratti, infatti posso vedere la successione $a_{n}$ come:
$$f(x) = a_{n} \ \ \ x \in [n-1,n]$$
$$\sum_{n}^\infty a_{n} \text{ converge } \iff \int_{0}^\infty f(x)dx \in \mathbb{R}$$
### osservazione 5 (tbf)
Tutti i teoremi e le osservazioni che quindi si potevano fare per le serie valgono anche per gli integrali impropri: 
- $f(x)>0$ allora o converge o diverge 
- [[01-uni/primo-anno/analisi-1/serie/teoremi/teorema-confronto-serie\|teorema-confronto-serie]]
- teorema del panino imbottito
- teorema confronto asintotico
- teorema convergenza assoluta
- $...$
importante citare che se $f \in I(a,b) \not \Rightarrow |f| \in I(a,b)$ come per il [[01-uni/primo-anno/analisi-1/serie/teoremi/criterio-Leibnitz\|criterio-Leibnitz]].
___
### definizione con partizione di intervalli
diciamo che $f$ è localmente integrabile se $\exists$ una partizione dell'intervallo $[a,b]$ t.c. 
$$a =x_{0}<x_{1}<\dots<x_{n} = b$$
t.c. la funzione è [[01-uni/primo-anno/analisi-1/funzioni/definizioni/def-integrale-improprio-(tbf)#definizione intervallo unico\|localmente integrabile nel senso di prima]] in ogni intervallo $(x_{k-1},x_{k})$. In tal caso:
$$\int_{a}^b f(x)dx = \sum_{k=1}^n \int_{x_{k-1}}^{x_{k}} f(x)dx$$
in pratica se dividi $[a,b]$ in tanti intervalli e in ognuno di questi la tua funzione è integrabile impropriamente allora l'integrale della funzione su $[a,b]$ è la somma dell'integrale di $f$ su tutti i piccoli intervalli: 
$$f \in I(a,b) \iff f \in I(x_{k-1},x_{k}) \forall k \in [1,n] \ \cap \mathbb{N}$$
di conseguenza quando cerchi di studiare la convergenza di un integrale improprio ti puoi soffermare solo sugli intervalli compresi tra due "punti critici", ovvero punti in cui la funzione non è limitata o estremi di integrazione non finiti (es : $a = -\infty, b = +\infty, x = 1, x = 0 \dots$)
Quindi alla fine negli esercizi studi l'integrale improprio solo in intorni di punti critici dove $f$ è a segno costante così puoi usare il [[01-uni/primo-anno/analisi-1/serie/teoremi/criterio-confronto-asintotico\|criterio-confronto-asintotico]] che è uguale dalle serie