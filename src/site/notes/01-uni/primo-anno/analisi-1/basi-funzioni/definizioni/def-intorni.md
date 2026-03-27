---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/analisi-1/basi-funzioni/definizioni/def-intorni/","tags":["uni","math"],"updated":"2026-01-05T09:25:10.874+01:00"}
---

# intorno
Definiamo $u(x)$ come intorno di $x$ nel seguente modo : 
$$\forall x \in \overline{\mathbb{R}} , u(x) = \cases {(x-\varepsilon, x+\varepsilon)  \text{ con } \varepsilon>0 \text{ if } x \in \mathbb{R} \\ \\ (M, +\infty)  \text{ con } M>0 \text{ if } x = +\infty \\ \\ (-\infty, -M) \text{ con } M>0 \text{ if } x = -\infty}$$
### osservazione importante
$$X_n\rightarrow x \iff \forall u(x), X_n \in u(x) \text{ definitivamente}$$
se una successione converge allora essa appartiene ad ogni del suo limite intorno definitivamente.
___
# intorno bucato
Definiamo $\dot{u}(x)$ come intorno bucato di $x$ nel seguente modo : 
$$\dot{u}(x) = \cases{ u(x) \text{ if } x = \pm \infty \\  \\ u(x) \setminus \{x\}\text{ negli altri casi} }$$
$$u(x) \setminus \{x\} = (x-\varepsilon, x) \cup(x,x+\varepsilon)$$

(per più info riguardo queste note guarda il [[PDF-Limiti-Pata.pdf|questo link del Pata]]) 