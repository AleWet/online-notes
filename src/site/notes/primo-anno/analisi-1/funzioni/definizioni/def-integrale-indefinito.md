---
{"dg-publish":true,"permalink":"/primo-anno/analisi-1/funzioni/definizioni/def-integrale-indefinito/","tags":["math","uni"],"updated":"2026-02-24T15:52:00.481+01:00"}
---

sia $f$ una funzione che ammette [[primo-anno/analisi-1/funzioni/definizioni/def-primitiva\|primitiva]] in $[a,b]$ indichiamo con il simbolo
$$\int f(x)dx $$
$$ \text{ l'insieme di tutte le primitive di } f$$
e lo chiamiamo **integrale indefinito**. Chiamata $F$ una generica primitiva di $f$ si scrive con abuso di notazione :
$$\int f(x)dx = F(x) + c \in \mathbb{R}$$
intendendo in realtà la seguente cosa:
$$\int f(x)dx = \{\dot{F}(x)+c \ | \ \dot{F} \text{ è una primtivia di } f , c \in \mathbb{R}\}$$
### osservazione 1
naturalmente questa definizione sottintende che si devono cercare primitive nell'intervallo in cui possono esistere. Quindi vuol dire che la primitiva può e deve essere "cercata" anche dove $f$ **non sia integrabile** poiché integrabilità $\not \Rightarrow$ ammette primitiva e ammette primitiva $\not \Rightarrow$ integrabilità (guarda [[primo-anno/analisi-1/funzioni/definizioni/def-primitiva#osservazione 4\|qui]]).

