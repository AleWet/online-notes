---
{"dg-publish":true,"permalink":"/uni/primo-anno/analisi-1/funzioni/definizioni/def-integrale-riemann-tbf/","tags":["math","uni"]}
---

# costruzione dell'integrale di Riemann
sia $f:[a,b] \to \mathbb{R}$ con $f$ LIMITATA su $[a,b]$, fissiamo $n \in \mathbb{N}$ e *equipartiamo* $[a,b]$ in $n$ intervalli di lunghezza $\frac{b-a}{n}$ :
1) $x_{n} = b$
2) $x_{0} = a$
3) $x_{k} := a+\frac{b-a}{n}*k$ 
4) $I_{k}:= [x_{k-1},x_{k}]$ 
### osservazione 1
poiché $f$ è limitata per ipotesi, $\forall k$ tra $1$ e $n$ il [[uni/primo anno/analisi 1/successioni/definizioni/def-estremo-superiore-inferiore-e-max-min\|sup]] e [[uni/primo anno/analisi 1/successioni/definizioni/def-estremo-superiore-inferiore-e-max-min\|inf]] di $I_k$ è *finito* :
$$\forall k \ \ \sup_{I_{k}}f, \ \inf_{I_{k}}f \in \mathbb{R}$$
non è tuttavia garantito che abbiano $\max$ e $\min$.
### osservazione 2
esistono funzioni limitate non integrabili e come sempre usi la [[uni/primo anno/analisi 1/funzioni/definizioni/def-funzione-Dirichelt\|funzione di Dirichlet]]  $:[0,1] \to \mathbb{R}$, in ogni intervallino indipendentemente da quanto lo si fa piccolo si avrà che $\sup D$ e $\inf D$ sono sempre $1$ e $0$. 
___
# somme inferiori e superiori
definisco **somma inferiore** relativa a $f$ su $[a,b]$ di ordine $n$ la quantità
$$s_{n}= \frac{b-a}{n}\sum_{i=1}^n \inf_{I_{k}}f$$
definisco **somma superiore** in modo analogo:
$$S_{n} = \frac{b-a}{n}\sum_{i=1}^n \sup_{I_{k}}f$$
### osservazioni necessarie
$$\tag{1}\forall n, \forall m  \ \ s_{n} \le S_{n}$$
l'area del pluri-rettangolo sotto il grafico di $f$ sarà sempre minore di tutti i pluri-rettangoli che posso costruire sopra il grafico di $f$.
$$\tag{2}S_{n} \text{ non è detto che sia decrescente, } s_{n} \text{ non è detto che sia crescente}$$
per gli esempi guarda QR4.
$$\tag{3}s:=\sup s_{n}, \ S:= \inf S_{n} \implies s_{n}\le s \le S \le S_{n} \ \forall n$$
Questo puoi dirlo perché $S_{n}$ è inferiormente limitato da $s_n$ e $s_n$ è superiormente limitato da $S_n$ 
___
# Riemann integrabile
diciamo che $f$ è **Riemann integrabile** su $[a,b]$ se 
$$\lim_{ n \to \infty } s_{n} = \lim_{ n \to \infty } S_{n}\implies S = s$$
e indichiamo con $R(a,b)$ l'insieme delle funzioni integrabili secondo Riemann su $[a,b]$. Il valore $s$ = $S$ è detto *integrale* di $f$ su $[a,b]$ con notazione:
$$\int_{a}^b f(x)dx$$
### $\omega$ somme sup e inf
Definiamo poi la seguente quantità:
$$\omega_{n}(f) = S_{n}-s_{n} = \frac{b-a}{n} \sum_{k=1}^n \sup_{I_{k}}f-\inf_{I_{k}}f$$
e faccio la seguente osservazione:
$$f \in R(a,b) \iff \omega_{n}(f)\to 0 \iff s_{n},S_{n}\to l$$
per la dimostrazione guarda [[uni/primo anno/analisi 1/funzioni/teoremi/teoremi integrali Riemann/teorema-delta-somme-superiori-inferiori-TBD\|qui]]
____
# definizione equivalente
L'integrale può essere definito in molti modi, uno citato dal Pata è di definire prima l'integrabilità di una [[uni/primo anno/analisi 1/funzioni/definizioni/def-funzione-costante-a-tratti#osservazione importante\|funzione costante a tratti]] e poi dire che ogni funzione integrabile può essere "compresa" tra due funzioni costanti a tratti :
### teorema / osservazione
$$\text{ data } f : [a,b] \to \mathbb{R} \text{ sono equivalenti le affermazioni : }$$
$$(i) \ f \in R(a,b)$$
$$(ii) \ \text{ per ogni } \varepsilon > 0 \ \exists \ h^+, h^- \text{ costanti a tratti in }[a,b] : $$
$$h^- \leq f \leq h^- \ \ \ \text{ e si ha che : } \ \ h := h^+ - h^- \text{ soddisfa} \int _{a}^b h(x)dx < \varepsilon$$
per più info guarda [[Integrale.pdf|questo pdf del Pata]] 
