---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/analisi-1/funzioni/teoremi/teoremi-funzione-derivata/teorema-de-l-hopital/","tags":["math","uni"],"updated":"2026-01-05T09:42:31.136+01:00"}
---

sia $x_{0} \in \overline{\mathbb{R}}$ e siano $f,g$ [[01-uni/primo-anno/analisi-1/funzioni/definizioni/def-derivata#derivabilità\|derivabili]] in $\dot{u} (x_0)$
inoltre (importante ma te lo dimentichi sempre)  : $g'(x) \ne 0 \ \forall x \in \dot{u}(x_{0})$ 
Assumiamo che 
- $\lim_{ x \to x_{0} }f(x) = \lim_{ x \to x_{0} }g(x)$
OPPURE
- $\lim_{ x \to x_{0} }g(x) = \pm\infty$
allora
$$\lim_{ x \to x_{0} } \frac{f'(x)}{g'(x)} = \lim_{ x \to x_{0} } \frac{f(x)}{g(x)} = l \in \overline{\mathbb{R}} $$
### osservazione importante
questo teorema ci fornisce una condizione sufficiente non necessaria per il calcolo del limite.
### osservazione ipotesi
se $\exists x \in \dot{u}(x_{0}) : g'(x) = 0$ la tesi diventa falsa, l'esempio patologico non lo riporto ma è sul solito pdf.
### dim
il Pata ha dimostrato un caso di questo teorema, non penso uscirà mai all'esame, se vuoi c'è nel [[PDF-Derivata-Pata.pdf|pdf del Pata]].