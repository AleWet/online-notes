---
{"dg-publish":true,"permalink":"/uni/primo-anno/analisi-1/successioni-funzioni/definizioni/def-serie-di-potenze/","tags":["math","uni"]}
---

chiamiamo **serie di potenze** una [[uni/primo anno/analisi 1/successioni funzioni/definizioni/def-serie-di-funzioni\|serie di funzioni]] della seguente specie:
$$\sum_{n=0}^\infty a_{n} x^n$$
$$= a_{0}+a_{1}x+a_{2}x^2+a_{3}x^3+\dots$$
dove $a_{n}$ è una [[uni/primo anno/analisi 1/successioni/definizioni/def-successione\|successione]] assegnata e interpretiamo $0^0$ come $1$ come al solito.
### raggio di convergenza
chiamiamo **raggio di convergenza** di una serie di potenze la quantità:
$$R = \frac{1}{L} \in [0,+\infty]$$
$$L = \overline{\lim_{ n \to \infty } } \sqrt[n]{ |a_{n} }$$
$$L = 0 \implies R = +\infty$$
$$L = +\infty \implies R = 0$$
e finalmente capisci perché il Pata ha usato il [[uni/primo anno/analisi 1/successioni/definizioni/def-limite-superiore-inferiore\|limite superiore]] nel [[uni/primo anno/analisi 1/serie/teoremi/criterio-della-radice\|criterio-della-radice]] per le [[uni/primo anno/analisi 1/serie/definizioni/def-serie\|serie normali]]. 
### osservazione 1
spesso il $\overline{\lim_{ n \to \infty }}$ diventa semplicemente un $\lim_{ n \to \infty }$ normale, serve solo nelle **serie lacunari**, ovvero serie a cui mancano dei termini di una certa specie:
$$\sum_{n=0}^\infty \frac{(-1)^n}{2n+1}x^{2n+1}$$
dove per calcolare il limite escludo i termini "nulli" della serie, ovvero tutti i termini pari:
$$L = \overline{\lim_{ n \to \infty }} \sqrt[2n+1]{ |a_{n} |}$$
$$=\overline{\lim_{ n \to \infty }} \sqrt[2n+1]{ \frac{1}{2n+1} }$$
