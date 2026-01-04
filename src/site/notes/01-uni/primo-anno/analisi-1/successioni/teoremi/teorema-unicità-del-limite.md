---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/analisi-1/successioni/teoremi/teorema-unicita-del-limite/","tags":["math","uni"]}
---

una successione $a_n \rightarrow l_1 \in \mathbb{R}$ (anche infinito) allora il suo limite è unico, non è vero che $a_n \rightarrow l_2 \ne l_1$   
### ==dim==
prendi $\epsilon = \frac{{|l_1-l_2|}}{4}$ o ogni altro numero $>2$ e trovi assurdo partendo da $|l_1 - l_2|$ e aggiungi e togli $a_{n0}$ poi triangolare a destra che viene $\le2 \epsilon$.
$$\text{P.A. } a_n \rightarrow l \in \mathbb{R} \ e \ a_n\rightarrow\gamma\in\mathbb{R}$$
$$\forall\epsilon>0 \ \exists n_0 : \forall n\ge n_0 \ |a_n-l|<\epsilon \ \land |a_n-\gamma|<\epsilon$$
$$\text{ fisso } \epsilon = \frac{|l-\gamma|}{2\pi}$$
$$|l-\gamma| = |l-a_n+a_n-\gamma| \le|l-a_n|+|\gamma-a_n|<2\epsilon$$
$$2\epsilon =\frac{|l-\gamma|}{\pi}$$
$$\implies|l-\gamma| < \frac{|l-\gamma|}{\pi}$$
$$\implies 1 < \frac{1}{\pi} \implies1>\pi \text{ (assurdo)} \ \ \ \square$$

