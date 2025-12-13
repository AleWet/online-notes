---
{"dg-publish":true,"permalink":"/uni/primo-anno/analisi-1/successioni-funzioni/def-serie-di-funzioni/","tags":["math","uni"]}
---

data $f_{n}: I \to \mathbb{R}$ costruiamo, come nelle [[uni/primo anno/analisi 1/serie/definizioni/def-serie\|serie]], la **successione delle somme parziali** di una [[uni/primo anno/analisi 1/successioni funzioni/def-successione-funzioni\|successione di funzioni]] :  
$$s_{n}(x) = \sum_{k = 1}^n f_{k}(x) \ \ \forall x \text{ fissato}$$
# convergenza puntuale
come nelle [[uni/primo anno/analisi 1/successioni funzioni/def-successione-funzioni#convergenza puntuale\|successioni di funzioni]] diciamo che $s_{n}$ **converge puntualmente in $x$ se** :
$$\exists  \in \mathbb{R}\lim_{ n \to \infty } \sum_{n=1}^\infty f_{n}(x)$$ e lo chiamiamo:
$$S(x) :=\lim_{ n \to \infty } \sum_{n=1}^\infty f_{n}(x), \ \ s_{n} \to S$$
# convergenza uniforme
uguale alle [[uni/primo anno/analisi 1/successioni funzioni/def-successione-funzioni#convergenza uniforme\|successioni di funzioni]], anche stessa notazione :
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