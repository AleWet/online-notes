---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/analisi-1/successioni-funzioni/definizioni/def-serie-di-potenze/","tags":["math","uni"],"updated":"2026-01-08T15:08:49.262+01:00"}
---

# definizione
chiamiamo **serie di potenze** una [[01-uni/primo-anno/analisi-1/successioni-funzioni/definizioni/def-serie-di-funzioni\|serie di funzioni]] della seguente specie:
$$\sum_{n=0}^\infty a_{n} x^n$$
$$= a_{0}+a_{1}x+a_{2}x^2+a_{3}x^3+\dots$$
dove $a_{n}$ è una [[01-uni/primo-anno/analisi-1/successioni/definizioni/def-successione\|successione]] assegnata e interpretiamo $0^0=1$ come al solito.
### raggio di convergenza
chiamiamo **raggio di convergenza** di una serie di potenze la quantità:
$$R = \frac{1}{L} \in [0,+\infty]$$
$$L = \overline{\lim_{ n \to \infty } } \sqrt[n]{ |a_{n} }$$
$$L = 0 \implies R = +\infty$$
$$L = +\infty \implies R = 0$$
per capire a cosa serve il raggio di convergenza è necessario guardare [[01-uni/primo-anno/analisi-1/successioni-funzioni/teoremi/teorema-raggio-convergenza\|seguente teorema]].
### osservazione 1
spesso il $\overline{\lim_{ n \to \infty }}$ diventa semplicemente un $\lim_{ n \to \infty }$ normale, serve solo nelle **serie lacunari**, ovvero serie a cui mancano dei termini di una certa specie:
$$\sum_{n=0}^\infty \frac{(-1)^n}{2n+1}x^{2n+1}$$
dove per calcolare il limite escludo i termini "nulli" della serie, ovvero tutti i termini pari:
$$L = \overline{\lim_{ n \to \infty }} \sqrt[2n+1]{ |a_{n} |}$$
$$=\overline{\lim_{ n \to \infty }} \sqrt[2n+1]{ \frac{1}{2n+1} }$$
### osservazione 2
se $a_{n}$ è polinomiale o una funzione razionale generica, il raggio di convergenza $R$ sarà sempre $=1$:
$$\sqrt[n]{ |a_{n}| } = |a_{n}|^{ 1/n } = e^{ \frac{1}{n}\log(|a_{n}|)}$$
$$a_{n} \sim n^p  \implies e^{ \frac{1}{n}\log(|n^p|)} \to 1$$
$$\implies R = 1, L = 1$$
### osservazione 3
$a_n$ contiene un fattoriale $\implies R = +\infty$ :
$$(n!)^{ 1/n } = e^{ \frac{1}{n} \log{n!}}$$
$$ \frac{1}{n} \log(n!) \sim \log n$$
quindi la [[01-uni/primo-anno/analisi-1/serie/definizioni/def-serie-fattoriale\|serie fattoriale]] ha un raggio di convergenza $+\infty$ :
$$\sum_{0}^\infty a_{n}x^n = \sum_{0}^\infty\frac{x^n}{n!}$$
$$L = 0 \implies R = +\infty$$
### osservazione 4
sia data $\sum_{0}^\infty a_{n}x^n$ allora 
$$\text{se } \bigg|\frac{a_{n+1}}{a_{n}}\bigg| \to L \implies \sqrt[n]{|a_{n}}| \to L$$
ma il contrario non è vero, equivalentemente sto dicendo che il [[01-uni/primo-anno/analisi-1/serie/teoremi/criterio-della-radice\|criterio-della-radice]] è sempre meglio di [[01-uni/primo-anno/analisi-1/successioni/teoremi/criterio-del-rapporto-successioni\|quello del rapporto]]. Questa cosa l'ha dimostrata il pasto a lezione guarda QR5.
___
# negli estremi  TBD
la serie di potenze negli estremi $\pm R$ in generale non so come si comporti, è importante citare però il [[01-uni/primo-anno/analisi-1/successioni-funzioni/teoremi/teorema-Abel\|teorema-Abel]].
