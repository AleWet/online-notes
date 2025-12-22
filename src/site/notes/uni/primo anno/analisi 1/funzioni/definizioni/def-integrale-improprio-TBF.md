---
{"dg-publish":true,"permalink":"/uni/primo-anno/analisi-1/funzioni/definizioni/def-integrale-improprio-tbf/","tags":["math","uni"]}
---

### ipotesi
- $f:(a,b) \to \mathbb{R}$ , dove : $-\infty \le a \le b \le +\infty$
- $f$ è **LOCALMENTE** integrabile, cioè $\forall [c,d] \in (a,b) \text{ si ha che } f \in R(c,d)$.
### definizione
Di conseguenza non integro $f$ direttamente sul mio intervallo brutto $(a,b)$ ma su $[c,d]$ dove per ipotesi $f \in R(c,d)$ e applico un **DOPPIO LIMITE**:
$$\lim_{\begin{smallmatrix} d \to b & \\ c \to a \end{smallmatrix}} \int_{c}^d f(x)dx$$
se questo limite $\exists$ **FINITO** diciamo che $f$ è integrabile impropriamente su $(a,b)$.
### osservazioni importante 1
1) se $a = -\infty$ oppure $b = \infty$ o entrambi avrò $(a,b)$ non limitato e quindi non posso implementare la procedura di Riemann direttamente. 
2) Può anche essere che $f$ non sia limitata nell'intervallo $(a,b)$ e anche questa è un'ipotesi della procedura dell'[[uni/primo anno/analisi 1/funzioni/definizioni/def-integrale-Riemann-TBF\|integrale di Riemann]].
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
e se lo risolvi ottieni che con $\varepsilon \to 0, I = +\infty$ e concludo (uguale alla [[uni/primo anno/analisi 1/funzioni/definizioni/def-continuità#continuità successionale\|continuità successionale]]) che il limite doppio non esiste.
### osservazione 3
Negli esercizi spesso non ti viene richiesto di calcolare il valore dell'integrale ma il comportamento (uguale al discorso fatto con le [[uni/primo anno/analisi 1/serie/definizioni/def-serie\|serie]]) in un certo intorno di un **punto critico** dove con punto critico intendiamo un punto dove la funzione smette di essere Riemann integrabile (un asintoto verticale, $\pm \infty$). Se però ti chiedono di calcolare il valore dell'integrale improprio devi prima dimostrare che esso effettivamente è integrabile in quell'intorno, trovare la primitiva e poi dire applicare il [[uni/primo anno/analisi 1/funzioni/teoremi/teoremi integrali Riemann/teorema-fondamentale-del-calcolo\|teorema-fondamentale-del-calcolo]] con un limite.zx
### notazione interna al corso
diciamo che una funzione è integrabile impropriamente su un intervallo $(a,b)$ come:
$$f \in I(a,b)$$
quindi come una [[uni/primo anno/analisi 1/funzioni/definizioni/def-classi-di-continuità\|classe]] di funzioni come quelle di Riemann.