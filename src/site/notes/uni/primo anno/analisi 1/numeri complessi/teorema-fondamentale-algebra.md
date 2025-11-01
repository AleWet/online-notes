---
{"dg-publish":true,"permalink":"/uni/primo-anno/analisi-1/numeri-complessi/teorema-fondamentale-algebra/","tags":["math","uni"]}
---

siano $a_0, a_1, a_2, ... , a_n \in \mathbb{C}$ dove $a_n \ne 0$, l'equazione
$$a_0+a_0z+a_1z^2+a_2z^3+...+a_nz^n = 0$$
ha esattamente $n$ soluzioni in $\mathbb{C}$ contate con la loro [[uni/primo anno/analisi 1/numeri complessi/def-molteplicità-radice\|molteplicità]].
Ciò vuol dire che $\mathbb{C}$ è un campo algebricamente chiuso, ovvero ogni equazione ha tutte soluzioni nel campo di partenza.
### corollario importante
se l'equazione polinomiale è a coefficienti reali ($a_0,a_1,...,a_n \in \mathbb{R}$) allora :
1) $\alpha \in \mathbb{C}$ è soluzione $\iff$ $\overline{\alpha}$ è soluzione   
2) $\alpha \in \mathbb{C}$ è soluzione $\implies$ $\overline{\alpha}, \alpha$ hanno la stessa molteplicità
### ==dim corollario==
$$p(z) = a_0z^0+a_1z^1+a_2z^2+...+a_nz^n$$
$$\text{sia } \alpha \text{ radice di } p(z) \implies p(\alpha) =0$$
$$\implies p(\alpha) = 0 = a_0+a_1\alpha +a_2\alpha^2+a_3\alpha^3+...+a_n\alpha^n$$
$$\overline0 = \overline{a_0+a_1\alpha +a_2\alpha^2+a_3\alpha^3+...+a_n\alpha^n}=$$$$=\overline{a_0} + \overline{a_1\alpha}+\overline{a_2\alpha^2}+...+\overline{a_n\alpha^n}$$
$$\forall i, \  a_i \in \mathbb{R} \implies \overline{a} = a \ \ \text{ e poiché }\overline{z^n} = \overline{z}^n$$
$$0 = a_0+a_1\overline\alpha +a_2\overline\alpha^2+a_3\overline\alpha^3+...+a_n\overline\alpha^n$$$$\implies p(\overline\alpha) = 0 \ \ \ \ \ \ \ \square$$

