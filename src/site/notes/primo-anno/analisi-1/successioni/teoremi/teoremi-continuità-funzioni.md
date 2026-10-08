---
{"dg-publish":true,"permalink":"/primo-anno/analisi-1/successioni/teoremi/teoremi-continuita-funzioni/","tags":["math","uni"],"updated":"2026-02-24T15:52:00.488+01:00"}
---

### ==nota importante==
in generale non è vero la seguente cosa ([[primo-anno/analisi-1/successioni/definizioni/def-asintotico#come non usarlo\|regole asintotici]]):
$$a_n \sim b_n \nRightarrow f(a_n) \sim f(b_n)$$
esempi importanti:
$\cos(a_n) \rightarrow \cos(\lim a_n)$ ma $a_n \sim b_n \nRightarrow \cos(a_n) \sim \cos(b_n)$. quindi se trovi una cosa del genere:
$$a_n  =\pi \sqrt{n^2-n}  \sim b_n = \pi n$$
$$\cos(a_n) \not\sim \cos(b_n)$$
però è vero che se $a_n - b_n \rightarrow 0$ per funzioni continue $\implies f(a_n)\sim f(b_n)$
___
### continuità logaritmi
sia $a_n$ a termini positivi t.c. $a_n \rightarrow a \in [0, +\infty]$ allora:
$$log(a_n) \rightarrow L \ \ dove\ \  L = \begin{cases}
  log(a) \ \ se \ a\in(0,+\infty) \\
  -\infty \ \ se \ a=0 \\
  +\infty \ \ se \ a = + \infty
\end{cases}$$
##### ==dim==
guarda QR2 la dimostrazione non è banale
___
### continuità esponenziale
sia $a_n$ t.c. $a_n \rightarrow a$ allora:
$$e^{a_m} \rightarrow L \ \ dove\ \  L = \begin{cases}
  e^a \ \ se \ a\in\mathbb{R} \\
  +\infty \ \ se \ a=+\infty \\
  0 \ \ se \ a = - \infty
\end{cases}$$
##### ==dim== 
guarda QR2 la dimostrazione non è banale
____
### continuità sin / cos
sia $a_n$ t.c. $a_n \rightarrow a \in \mathbb{R}$ allora :
$$sin(a_n) \rightarrow sin(a)$$
$$cos(a_n) \rightarrow cos(a)$$
se invece $a_n \rightarrow +\infty$ allora in generale $sin(a_n), cos(a_n)$ oscillano.
##### ==dim==
___
### continuità arctan
sia $a_n$ t.c. $a_n \rightarrow \overline a \in \mathbb{\overline R}$ allora:
$$\arctan(a_n) \rightarrow L \ \ dove\ \  L = \begin{cases}
  \arctan(\overline a) \ \ se \ a\in\mathbb{R} \\
  +\frac{\pi}{2} \ \ se \ \overline a=+\infty \\
  -\frac{\pi}{2} \ \ se \ \overline a = - \infty
\end{cases}$$
da qui derivi la seguente identità che è anche molto importante:
$$\forall x>0 \ \arctan\left( \frac{1}{x} \right) + \arctan(x) = \frac{\pi}{2}$$
$$\forall x<0 \ \arctan\left( \frac{1}{x} \right) + \arctan(x) = -\frac{\pi}{2}$$
##### dim
la dimostrazione è sul QR2 ed è una assoluta merda di formula di somma di arcotangenti.
____

