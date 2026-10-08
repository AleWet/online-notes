---
{"dg-publish":true,"permalink":"/primo-anno/analisi-1/basi-successioni/numeri-complessi/teorema-radici-complesse/","tags":["math","uni"],"updated":"2026-02-24T15:52:00.480+01:00"}
---

sia $n \in \mathbb{N} \ \ge1, z\in\mathbb{C}$ t.c. $z = \rho e^{i\theta}$ allora esistono esattamente $n$ radici $n$-esime distinte di $z$ date da:
$$w_k = \rho^{1/n} e^{i\theta_k}, \ \ \ \theta_k = \frac{\arg(z)+2k\pi}{n }$$
$$k \in \{0,1,2,3,...,n-1\}$$
### dim
la dimostrazione è incredibilmente lunga ma è concettualmente semplice, fai per assurdo che ci sono altre radici con angoli fuori dal range di $\{0,1,2,3,...,n-1\}$ e ti vengono tre casi: 
- ogni numero intero $p \not\in[0, n-1] \cap \mathbb{N}$ t.c. $|p|>n$ può essere scritto come $p = dn + r$ e (lo dividi per $n$) e il termine $dn$ dentro l'espresione $\frac{2(k)\pi}{n}$ ti diventa una cosa simile a : $\frac{2(dn+r)\pi}{n} = 2\pi d * \frac{2\pi r}{n}$ dove naturalmente il primo termine è irrilevante
- i numeri interi $p \in [-(n-1), -1]$ sono leggermente diversi : devi moltiplicare per $e^{i2\pi}$ e ti verrà una cosa del genere : $\frac{i2\pi (n-|p|)}{n}$ dove $(n-|p|) \in \{0,1,2,3,...,n-1\}$ e quindi contro ipotesi