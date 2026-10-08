---
{"dg-publish":true,"permalink":"/primo-anno/analisi-1/serie/definizioni/def-serie-geometrica/","tags":["uni","math"],"updated":"2026-02-24T15:52:00.485+01:00"}
---

definiamo una [[primo-anno/analisi-1/serie/definizioni/def-serie\|serie]] geometrica come di ragione $q \in \mathbb{R}$
$$\sum_{n=0}^{\infty}q^n$$
$$S_n = 0+q + q^2 + q^3+...+q^n$$
essa si comporta nel seguente modo:
$$\cases{
\frac{1}{1-q} \ \text{  se } |q|<1 \\
+\infty \ \text{ se } \ q > 1 \\
\text{ oscilla se  } \ q < -1
}$$
### osservazione
è banale dimostrare che :
$$\sum_{n_0}^\infty q^n = \sum_{0}^\infty q^n - \sum_{n}^{n_0} q^n$$
___
### ==dim==
il concetto è il seguente:
$$S_n = q^0 + q^1 + q^2 + ... + q^n$$
$$qS_n = q^1+q^2+...+q^{n+1}$$
$$S_n - qS_n = q^0 - q^1+q^1-...+q^n-q^n+q^{n+1} = q^0-q^{n+1}$$
$$S_n = \frac{1-q^{n+1}}{1-q}$$


