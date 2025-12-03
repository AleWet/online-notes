---
{"dg-publish":true,"permalink":"/uni/primo-anno/analisi-1/funzioni/definizioni/def-derivata/","tags":["math","uni"]}
---

# rapporto incrementale
sia $f:(a,b) \to \mathbb{R}$ e sia $x_0 \in (a,b)$, definiamo per $h \ne 0$ e quando $x_0+h \in (a,b)$ il seguente oggetto:
$$R(f,x_0,h)  := \frac{f(x_0+h) - f(x_0)}{h}$$
$$\text{ il rapporto incrementale della funzione f nel punto } x_0 \text{ di incremento }h$$
____
# derivabilità
$f$ è *derivabile* in $x_0$ se $\exists$ **FINITO**  il seguente limite:
$$\lim_{h \to 0} R(f,x_0,h)$$
il valore $l$ di questo limite è chiamato *derivata* di $f$ in $x_0$.
### notazione
$$\lim_{h \to 0} R(f,x_0,h) = f'(x_0) =D(f(x_0)) = \frac{df}{dx}(x_0)$$
se invece voglio fare la derivata destra o sinistra scrivo 
$$f'_{\pm} (x_0) = \lim_{h \to 0^{\pm}} R(f,x_0,h)$$
e naturalmente la derivata esiste se il limite destro e sinistro sono uguali.
### osservazione 1
la definizione geometrica di retta tangente è incompleta e si basa fondamentalmente sul concetto di derivata ed è necessario passare per via analitica : la derivata definisce la retta tangente. Di conseguenza se non posso derivare non posso definire la retta tangente nel punto $x_0$
$$r_0 = f(x_0) + f'(x_0)(x-x_0)$$
di conseguenza la derivata nel punto potrebbe intersecare il grafico della funzione infinite volte come nel caso in $x_0 = 0$ di :
$$f(x) = \cases{x^2 sin\left( \frac{1}{x} \right)  \ \ \ \ x \ne 0 \\ \\\ 0 \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \  \ \ x = 0} $$
### osservazione 2
le seguenti cose sono vere se dico che il limite di $R(f,x_0,h)$ deve essere **FINITO** : 

1) se so che la funzione è derivabile in $x_0$ so anche che è [[uni/primo anno/analisi 1/funzioni/teoremi/teoremi funzione derivata/teorema-derivabile-allora-continua\|continua]]  
2) se $f,g$ sono derivabili in $[a,b]$ e so che $\forall x\in [a,b] \ \ f'(x) =g'(x) \implies f(x) = g(x) +c$

se ammettessi che il limite del rapporto incrementale fosse $\pm \infty$ allora sorgerebbero dei problemi:
$$\tag{1} f(x) = \cases{ x^{1/3} + 1\ \ \ \ \ \ x \ge 0 \\ \\ x^{1/3} \ \ \ \ \ \ \ \ \ \  \ \  \ x < 0}$$
$$f'(0) = +\infty \text{ ma } f \text{ non è continua in } x_0$$
$$\tag{2}\text{il controesempio di Ruziewicz ti dice che salta anche la seconda proprietà}$$
### osservazione 3
sia $f : [a,b] \to \mathbb{R}$ allora dire che $f$ è derivabile in $a$ e $b$ è dire che $\exists$ rispettivamente la derivata destra e derivata sinistra ($f'_+(a) \ \  \land \ \  f'_-(b)$)
### osservazione 4
naturalmente implicito dire che quando faccio $\lim_{h \to 0} f(x_0+h)...$ sto dicendo che $f$ è definita in un [[uni/primo anno/analisi 1/basi funzioni/definizioni/def-intorni\|intorno]] $u(x_0)$ se no questo limite non è neanche "applicabile".
### osservazione 5
Nella definizione di rapporto incrementale e di derivata io non ho ipotesi riguardo la funzione $f$, ci poi sono teoremi che mi danno info sulla $f$ se $\lim_{ h \to 0 }R(f,h,x_{0}) \in \mathbb{R}$ ma a priori io definisco il rapporto incrementale senza queste informazioni.  
___
# funzione derivata
sia $f : I \to \mathbb{R}$ (definita su tutto l'intervallo) costruisco la funzione derivata di $f$ nel seguente modo:
$$D(f') = \{x \in I : f \text{ derivabile in } x\}$$
$$x\longmapsto f'(x)$$
### osservazione
non è naturalmente vero che se $f$ è continua e derivabile la sua derivata è continua, un esempio è:
$$\phi(x) = \cases{x^2sin\left( \frac{1}{x}\right) \ \ \ x \ne 0 \\ \\ 0  \ \ \ \ \ \ \ \ \ \ \ \ \ \ \  \ \ \ x = 0}$$
la funzione $f$ è continua in $x_0 = 0$ ma $f'(0)$ è undefined $\implies f'(x)$ non è continua.
