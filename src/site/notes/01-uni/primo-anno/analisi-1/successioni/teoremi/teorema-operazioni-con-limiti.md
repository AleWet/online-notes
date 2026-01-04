---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/analisi-1/successioni/teoremi/teorema-operazioni-con-limiti/","tags":["math","uni"]}
---

data $a_n \rightarrow a, b_n \rightarrow b$ allora se i limiti sono **finiti** (e quindi $\exists)$ posso dire le seguenti cose:
$$\tag*{primo}a_n +b_n \rightarrow a+b$$
$$\tag*{secondo}a_n*b_n \rightarrow ab$$
$$\tag*{terzo} b_n \ne 0, \frac{a_n}{b_n} \rightarrow \frac{a}{b}$$
___
### ==dim 1==
$$|a_n+b_n -(a+b)| \le |a_n-a|+|b_n-b| \le 2\epsilon$$
___
### ==dim 2==
$$|a_nb_n-ab|=|a_nb_n+a_nb-a_nb+ab|=|a_n(b_n-b) +b(a_n-a)| \le |a_n||b_n-b| + |b||a_n-a|$$
$$a_n,b_n \rightarrow a,b \in \mathbb{R} \implies a_n,b_n \ \  limitate \implies a_n(\epsilon_n) \rightarrow0 \ \ e \ \ b(\epsilon_n) \rightarrow0$$
$$\implies|a_nb_n-ab| \le |a_n||b_n-b| + |b||a_n-a| \le 2\epsilon$$
### ==dim 3==
la dimostrazione è equivalente a un prodotto tra $a_n$ e $\frac{1}{b_n} \implies$ devo dimostrare che 
$$ \frac{1}{b_n} \rightarrow \frac{1}{b}$$
assumo $b \ne 0$ e assumo vero il seguente teorema che dimostro dopo :
$$ \frac{1}{|a_n|} \le \frac{2}{|a|} \text{ definitivamente}$$
$$\text{ voglio dimostrare  che : }|\frac{1}{b_n} - \frac{1}{b}| \rightarrow0 $$
$$0 \le| \frac{b-b_n}{b_n*b}| = \frac{{|b-b_n|}}{|b_n ||b|} \le \frac{2}{|b|} * \frac{{|b-b_n|}}{b} \text{ (teorema da dimostrare)}$$
$$0 \rightarrow0, \ \ \frac{{2|b_n-b|}}{|b|^2} \rightarrow 0$$
per il [[01-uni/primo-anno/analisi-1/successioni/teoremi/teorema-del-confronto\|teorema-del-confronto]] la frazione iniziale $\frac{{|b-b_n|}}{|b_n ||b|}\rightarrow0$
$$\implies| \frac{1}{b_n} - \frac{1}{b}| \rightarrow0 \implies \frac{1}{b_n} \rightarrow \frac{1}{b}$$
dimostro adesso il teorema di prima:
$$a_n \rightarrow a \implies \frac{1}{|a_n|} \le \frac{2}{|a|} \text{ definitivamente}$$
$$\implies \frac{{2|a_n|-|a|}}{|a_n||a|} \ge 0 \text{ definitivamente}$$
$$a_n \rightarrow a \implies |a_n| \rightarrow |a|$$
$$\implies 2|a_n| \ge |a| \text{ definitivamente}$$
$$\left( \epsilon = \frac{|a|}{2} \implies |a|\le2|a|-\frac{|a|}{2} < 2|a_n| < \frac{5}{2}|a| \right)$$

$$$$
