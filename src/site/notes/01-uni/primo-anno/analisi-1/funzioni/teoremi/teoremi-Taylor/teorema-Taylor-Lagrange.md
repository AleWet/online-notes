---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/analisi-1/funzioni/teoremi/teoremi-taylor/teorema-taylor-lagrange/","tags":["math","uni"]}
---

sia $x_0$ fissato e sia $f$ [[01-uni/primo-anno/analisi-1/funzioni/definizioni/def-polinomio-Taylor\|politaylor]] di ordine $n$ centrato in $x_0$ di $f$ allora:
$$\exists y \in (x_{0},x) \text{ oppure } (x,x_{0})$$
$$\text{tale che } f(x) = P_{n}(x)+R_{n}(x)$$
dove chiamiamo $R_n(x)$ il **resto di Lagrange** :
$$R_{n}(x) = \frac{f^{(n+1)}(x)}{(n+1)!}(x-x_{0})^{n+1}$$
quindi stai dicendo che la funzione e il "politaylor" differiscono di un valore $R_{n}(x)$ che "scala" con la derivata successiva della funzione $f$. Di conseguenza alcune funzioni non sono solo approssimate in un intorno di $x_{0}$ dal politaylor ma in tutto il dominio, per esempio:
$$f(x) = e^x, x_{0}=0, P_{n}(x)=\sum_{k=0}^n \frac{x^n}{k!}$$
$$\implies f(x)-P_{n}(x) = \frac{e^y}{(n+1)!}x^{n+1} \ \text{ dove y } \in (0,x)$$
$$\implies f(x)-P_{n}(x)\le e^x \frac{x^{n+1}}{(n+1)!} \ \text{ poiché }  y < x $$
$$\implies f(x)-P_{n}(x) \le M = e^x \frac{x^{n+1}}{(n+1)!}$$
$$\lim_{ n \to \infty } M = 0 \implies f(x)-P_{n}(x) = 0 \implies P_{n}(x)\to f(x)$$
