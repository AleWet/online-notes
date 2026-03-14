---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/analisi-1/successioni-funzioni/teoremi/teorema-raggio-convergenza/","tags":["math","uni"],"updated":"2026-02-24T15:52:00.486+01:00"}
---

sia data una [[01-uni/primo-anno/analisi-1/successioni-funzioni/definizioni/def-serie-di-potenze\|serie di potenze]] e sia $R$ il suo raggio di convergenza allora:
$$\text{ se R } > 0$$
$$\tag{1}\implies \text{ la seire converge puntualmente in } (-R, R)$$
$$\tag{2}\implies \text{la serie converge totalmente in ogni intervallo } [-r, r] \text{ dove } 0<r<R$$
$$\tag{3}\implies \text{ la serie NON converge in ogni alcun intervallo } [-R, R]^C \text{ ovvero } |x| > R$$
(guarda [[01-uni/primo-anno/analisi-1/successioni-funzioni/definizioni/def-serie-di-funzioni#convergenza totale\|qui per convergenza totale]])
### osservazione 1
è importante notare che la convergenza totale implica quella uniforme che è solitamente più comoda perché hai più teoremi applicabili (guarda [[01-uni/primo-anno/analisi-1/successioni-funzioni/teoremi/teoremi-convergenza-uniforme-successioni\|qui]]).
### osservazione 2
se $R = +\infty$ vuol dire che la serie converge totalmente in ogni intervallo chiuso.
### osservazione 3
se trovi che $R = 0$ allora convergerà solo in $x = 0$.
____
# dimostrazioni
### dim $(1)$
Noto subito che questo punto è una conseguenza del $(2)$ quindi dimostrerò solo $(2)$ e $(3)$
### dim $(2)$
Assumo $R>0$, per la definizione di [[01-uni/primo-anno/analisi-1/successioni-funzioni/definizioni/def-serie-di-funzioni#convergenza totale\|convergenza totale]] devo fare il sup del valore assoluto e noto che il sup sarà sempre nell'estremo destro dell'insieme chiuso $[-r,r]$ : 
$$\sup_{x \in [-r,r]} |a_{n}x^n| \leq |a_{n}|r^n$$
adesso noto che:
$$\sum_{n=1}^\infty |a_{n}|r^n \text{ converge per il criterio della radice : }$$
$$\overline{\lim_{ n \to \infty } } \sup [|a_{n}|r^n]^{1/n}$$
$$= r* \overline{\lim_{ n \to \infty } } \sup |a_{n}|^{1/n} $$
$$= \frac{r}{R}$$
dove per ipotesi avevo $0<r<R \implies \frac{r}{R} <1$ allora il criterio della radice mi dice che la serie converge.
___
### dim $(3)$
se ho $R>0$ uso il criterio della radice con $x \in [-R,R]^c$  e trovo:
$$\overline{\lim_{ n \to \infty } } \sup [|a_{n}||x|^n]^{1/n}$$
come prima risolvo e ottengo:
$$\frac{|x|}{R} > 1$$
quindi per il criterio della radice il termine generale non tende a 0 quindi la serie non può convergere.