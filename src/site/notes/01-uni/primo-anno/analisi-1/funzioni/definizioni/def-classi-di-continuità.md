---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/analisi-1/funzioni/definizioni/def-classi-di-continuita/","tags":["math","uni"]}
---

# $D$
si definisce $D^1(I)$ la classe delle funzioni [[01-uni/primo-anno/analisi-1/funzioni/definizioni/def-derivata#derivabilità\|derivabili]] in $I$. A partire da questo definisco $D^N(I)$ come la classe delle funzioni [[01-uni/primo-anno/analisi-1/funzioni/definizioni/def-derivata#derivabilità\|derivabili]] $n$ volte in $I$:
$$D^n(I) = \{f : I\to \mathbb{R}  : f \text{ derivabile n volte in } I\}$$
dove per derivabile $n$ volte in un punto si intende che $\exists f^n(x_0)$ ovvero la derivata di $f^{n-1}(x_0)$ se $f^{n-1}(x_0)$ è definita in $u(x_0)$.
# $C$ 
si definisce $C^n(I)$ la classe delle funzioni [[01-uni/primo-anno/analisi-1/funzioni/definizioni/def-derivata#derivabilità\|derivabili]] $n$ volte e la cui derivata $n-esima$ è [[01-uni/primo-anno/analisi-1/funzioni/definizioni/def-continuità\|continua]] sull'intervallo di partenza $I$:
$$C^n(I)=\{f : I \to \mathbb{R} : f \text{ derivabile n volte in } I \ \land f'(I) \text{ è continua }\}$$
e con $C^0$ o semplicemente $C$ intendo che la funzione è solo continua su $I$.
### osservazione
naturalmente si ha che 
$$C^n(f)\subset D^n(f) \subset ... \subset C^3(f) \subset D^3(f)\subset C^2(f) \subset ...$$
perché tutte le funzioni in $D^n(f)$ possono appartenere alla classe "superiore" $C^n(f)$ le quali sono le uniche che possono essere derivate ulteriormente ([[01-uni/primo-anno/analisi-1/funzioni/teoremi/teoremi-funzione-derivata/teorema-derivabile-allora-continua\|derivabile allora continua]]) il che vuol dire che **possono** appartenere a $D^{n+1}(f)$.
