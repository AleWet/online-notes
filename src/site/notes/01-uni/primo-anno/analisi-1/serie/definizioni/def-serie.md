---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/analisi-1/serie/definizioni/def-serie/","tags":["math","uni"],"updated":"2026-02-24T15:52:00.485+01:00"}
---

non esiste un algoritmo che ti permette di sommare infiniti numeri, le serie non possono quindi essere trattate come serie infinite di numeri (tranne le serie per cui vale il [[01-uni/primo-anno/analisi-1/serie/teoremi/teorema-Riemann\|teorema-Riemann]]). 
Data una successione $a_n$ si costruisce un'altra successione chiamata **successione delle somme parziali** ($S_n$) :
$$S_n := a_0 + a_1 + a_2 + ... + a_n$$
Definiamo **serie** di termine generale $a_n$:
$$\sum_{n_0}^{+\infty}a_n :=\lim S_n$$
### carattere
una serie può essere:
- convergente
- divergente
- oscillante
esso non cambia se si cambia un numero finito di elementi della serie. Naturalmente se la serie converge la somma cambia ma il carattere rimane uguale.
### proprietà
- $k*\sum a_n$ =$\sum k*a_n$
- la somma delle serie converge se le due serie convergono anche nelle operazioni in [[01-uni/primo-anno/analisi-1/successioni/teoremi/teorema-operazioni-con-limiti\|operazioni con i limiti]].
### ordine di sommazione
L'ordine con cui vengono sommati gli elementi $a_n$ influisce sul comportamento della serie (QR2)

