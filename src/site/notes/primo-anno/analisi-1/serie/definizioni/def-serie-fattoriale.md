---
{"dg-publish":true,"permalink":"/primo-anno/analisi-1/serie/definizioni/def-serie-fattoriale/","tags":["math","uni"],"updated":"2026-02-24T15:52:00.485+01:00"}
---

### serie fattoriale
$$\sum_{n = 0}^\infty \frac{1}{n!} \rightarrow e $$
$$\text{più in generale : }\sum_{n = 0}^\infty \frac{x^n}{n!} \rightarrow e^x $$
### approssimazione di $e$
$$0 < e-S_n < \frac{1}{n!n} \forall n\ge1$$
### teorema di Eulero
$$e \not\in \mathbb{Q}$$
### dim 1
la dimostrazione del primo è fuori programma e la trovi alla fine del QR2
### ==dim 2==
$$\sum_{k=0}^{n} \frac{1}{k!} \rightarrow e^- \text{ serie a termini positivi allora crescente}$$
$$\implies S_n:=\sum_{k=0}^{n} \frac{1}{k!} \ - e > 0 \ \forall n$$
$$0 < e - S_n \text{ verificata}$$
$$e = \sum_{k=0}^{\infty} \frac{1}{k!}$$
$$S_n = \sum_{k=0}^{n} \frac{1}{k!}$$
$$\implies e - S_n = \sum_{k=n+1}^{\infty} \frac{1}{k!}$$
$$\sum_{k=n+1}^{\infty} \frac{1}{k!} = \frac{1}{(n+1)!} + \frac{1}{(n+2)!}+...$$
$$=\frac{1}{(n+1)!}\left( 1+\frac{1}{n+1}+\frac{1}{(n+1)(n+2)}+... \right) < \frac{1}{(n+1)!}(1+\frac{1}{n+1}+\frac{1}{(n+1)^2}+...)$$
è importante notare che la somma a sinistra è una [[primo-anno/analisi-1/serie/definizioni/def-serie-geometrica\|serie geometrica]] di ragione $q = \frac{1}{n+1}$ : 
$$\frac{1}{(n+1)!}\left( 1+\frac{1}{n+1}+... \right) = \frac{1}{(n+1)!}\left( \frac{1}{1-q} \right)=\frac{1}{(n+1)!} \frac{n+1}{n} = \frac{1}{n!n}$$
$$\implies 0<e-S_n < \frac{1}{n!n}$$
___
### ==dim 3==
$$\text{P.A. } \exists  \ p,q \in \mathbb{N} : \frac{p}{q} = e$$$$\implies0< \frac{p}{q} - S_n < \frac{1}{n!n} \ \forall n \ge1$$
$$\sum_{k=0}^{n} \frac{1}{k!} * n! = S_n * n! \in \mathbb{N} \text{ si vede dal fatto che} \sum_{k=1}^n \frac{n!}{k!} \text{ in ogni termine c'è almeno un fattore in comune}$$
$$0*n!< \frac{n!p}{q} -S_n*n! < \frac{1}{n}\le1 \ \forall n\ge1$$
$$\implies \exists n :  \frac{n!}{p} \in \mathbb{N} \text{ al massimo } n \ge p$$$$0< \frac{n!}{p} * q - S_n*n! =: m$$
$$\implies  m \in \mathbb{N} \text{ poiché differenza tra numeri naturali } \land \ e > S_n \forall n\ge1$$
$$\implies 0<m<1 \text{ dove } m \in \mathbb{N} \text{ ASSURDO}$$
