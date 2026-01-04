---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/analisi-1/successioni-funzioni/definizioni/def-serie-di-funzioni/","tags":["math","uni"]}
---

data $f_{n}: I \to \mathbb{R}$ costruiamo, come nelle [[01-uni/primo anno/analisi 1/serie/definizioni/def-serie\|serie]], la **successione delle somme parziali** di una [[01-uni/primo-anno/analisi-1/successioni-funzioni/definizioni/def-successione-funzioni\|successione di funzioni]] :  
$$s_{n}(x) = \sum_{k = 1}^n f_{k}(x) \ \ \forall x \text{ fissato}$$
il concetto è sempre quello di una successione di funzioni, ad ogni $n$ associ una funzione che in questo caso non è più "una singola funzione" ma una somma di più funzioni. Immagina di fissare un punto $x$, definisci $s_{n}(x)$ come la somma di $n$ funzioni tutte della variable $x$ :
$$s_{n}(x) = f_{1}(x)+f_{2}(x)+\dots+f_{n}(x)$$
quindi come prima hai una "macro funzione" $s_{n}$ 
che dipende sia da $n$ sia da $x$.a
# convergenza puntuale
come nelle [[01-uni/primo-anno/analisi-1/successioni-funzioni/definizioni/def-successione-funzioni#convergenza puntuale\|successioni di funzioni]] diciamo che $s_{n}$ **converge puntualmente in $x$ se** :
$$\exists  \in \mathbb{R}\lim_{ n \to \infty } \sum_{k=1}^n f_{k}(x)$$ e lo chiamiamo:
$$S(x) :=\lim_{ n \to \infty } \sum_{k=1}^n f_{k}(x), \ \ s_{n} \to S$$
# convergenza uniforme
uguale alle [[01-uni/primo-anno/analisi-1/successioni-funzioni/definizioni/def-successione-funzioni#convergenza uniforme\|successioni di funzioni]], anche stessa notazione :
$$s_{n} \xrightarrow{u} S $$
# convergenza totale
una serie di funzioni $\sum f_{n}:I \to \mathbb{R}$ ==converge totalmente== se 
$$\exists \text{ una successione } ;M_{n} \ge 0 : $$
$$\tag{1} \sup_{x \in I}|f_{n}(x)| \le M_{n}$$
$$\tag{2} \sum_{n = 1}^\infty M_{n} \in \mathbb{R}$$
questo concetto è molto utile poiché ==implica la convergenza uniforme== ed è più semplice da applicare praticamente.
### esempio
$$I = [0,1], \ \sum_{n= 1}^\infty \frac{(-x)^n}{n^2}$$
$$\sup_{x \in I}|f_{n}(x)| = \sup_{x \in I} \bigg|\frac{(-x)^n}{n^2} \bigg| \le \frac{1}{n^2}$$
$$\sum \frac{1}{n^2} \text{ converge } \implies \sum_{n= 1}^\infty \frac{(-x)^n}{n^2} \text{ converge}$$
### osservazione importante
se scelgo $M_{n}$ come la successione del $\sup$ di $f_n$ e la serie di $M_{n}$ non converge allora sicuramente la serie originale ==non converge totalmente==, ciò non vuol dire che non converge in generale ma vuol dire che il nostro criterio è inconcludente.