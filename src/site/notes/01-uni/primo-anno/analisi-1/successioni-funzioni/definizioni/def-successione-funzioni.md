---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/analisi-1/successioni-funzioni/definizioni/def-successione-funzioni/","tags":["math","uni"],"updated":"2026-01-08T10:26:53.889+01:00"}
---

# definizione
sia $I$ un intervallo reale definiamo una **successione di funzioni** il seguente oggetto:
$$\forall n \in \mathbb{N} \text{ sia } f_{n}:I\to \mathbb{R}$$
$$\{f_{n}\}\text{ è detta successione di funzioni}$$
in pratica stai associando a ogni etichetta $n$ non più un punto in $\mathbb{R}$ come una normale successione ma una $funzione$ che ha come dominio lo stesso intervallo, un modo chiaro per farlo capire è con il seguente esempio:
$$I = [0,1], \ \ \ f_{n}(x) = x^n$$
a ogni numero naturale associ una funzione con lo stesso dominio $I$, un nuovo oggetto che non solo prende come "input" $x \in I$ ma anche un indice $n$. 
### osservazione 1
per ogni punto $x_{0} \in I$ fissato, $\{f_{n}(x)\}$ è una normale [[01-uni/primo-anno/analisi-1/successioni/definizioni/def-successione\|successione numerica]] :
$$f_{1}(x),\ f_{2}(x),\ f_{3}(x)\dots$$
questo è chiaro dal fatto che uno dei due "input" della successione di funzioni, ovvero $x \in I$ è fissato, di conseguenza non si ha più una funzione che varia su un intero intervallo ma un singolo punto che varia al variare di $n \in \mathbb{N}$ che è esattamente la definizione di successione numerica.
___
# convergenza puntuale
diciamo che $\{f_{n}\}$ **converge puntualmente** se 
$$\forall x \in I, \ \{f_{n}(x)\} \ \text{ converge } \in \mathbb{R}$$
$$\text{ e definiamo } f : I \to \mathbb{R} \text{ come funzione limite}$$
$$f(x):= \lim_{ n \to \infty } f_{n}(x)$$
quindi solo quando il **limite esiste ed è finito**, la notazione standard è $f_{n} \to f$.
Guarda [[01-uni/primo-anno/analisi-1/successioni-funzioni/teoremi/teoremi-convergenza-puntuale-successioni-(tbd)\|qui]] per la trattazione fatta a lezione di questa proprietà che risulta molto debole.
___
# convergenza uniforme
visto che la convergenza puntiforme risulta abbastanza debole come concetto di convergenza (come puoi vedere nel link qui sopra) è necessaria una definizione di convergenza più potente.

diciamo che $f_{n} : I \to \mathbb{R}$ **converge uniformemente** a $f : I \to \mathbb{R}$ se :
$$\forall \varepsilon > 0 \ \exists n_{0} : \ \forall n \ge n_{0} \ $$
$$|f_{n}(x)-f(x)| < \varepsilon \ \ \forall x \in I$$
questo può sembrare analogo alla convergenza puntuale ma c'è una grande differenza nei quantificatori, infatti qui stiamo dicendo che dato un $\varepsilon > 0$ arbitrario si trova sempre un indice $n_0$ tale per cui in **tutti i punti** di $I$ la funzione $f_n$ è vicina $\varepsilon$ a $f$ (questo è molto simile al discorso fatto nella [[01-uni/primo-anno/analisi-1/funzioni/definizioni/def-uniformemente-continua\|continuità uniforme]]). 
Come per la convergenza delle successioni, immagina un "tubo" di $2 \varepsilon$ nella quale tutte le future $f_{n}$dovranno essere contenute. Questo è inoltre equivalente a dire la seguente cosa:
$$ \iff \sup_{x \in I} |f_{n}(x) - f(x)| < \varepsilon$$
$$\iff\lim_{ n \to \infty }  \sup_{x \in I} |f_{n}(x) - f(x)| = 0 \tag*{(**)}$$
la notazione che usa il Pata è
$$f_{n} \xrightarrow{u} f$$
è importante citare che con questo concetto di convergenza molte delle proprietà delle funzioni della successione si traslano alla funzione limite, per i teoremi guarda [[01-uni/primo-anno/analisi-1/successioni-funzioni/teoremi/teoremi-convergenza-uniforme-successioni\|qui]].
### osservazione importante
Si usa sempre la relazione $(* *)$ nei calcoli, è quella più utile. Ci sono eccezioni ma dovrebbe essere il tuo standard negli esercizi. Se è complesso capire dov'è il $\sup f_{n}$, è utile fare la derivata di $f_{n}$ e trovare il massimo assoluto / locale, spesso ti verrà un'espressione che dipende da $n$. A questo punto calcoli il tuo limite $(* *)$ nel punto $x = \sup$, se per esempio ti viene $x = \frac{1}{n}$ fai $f_{n}\left( \frac{1}{n} \right)$. Un esempio utile che ha fatto il Pata è :
 $$f_{n}(x) = \frac{\sqrt{ n }x}{1+n^2x^2}$$
 $$g_{n}(x) = \frac{nx}{1+n^2x^2}$$
 trovi che entrambe convergono puntualmente a $0$ ma $g_n$ ha come sup "costante" $g_{n}\left( \frac{1}{n} \right) = \frac{1}{2}$ il che vuol dire che $\forall n \ \sup g_{n} = \frac{1}{2}$ e visto che $g = 0, g_{n} \not \xrightarrow{u}g$.
 