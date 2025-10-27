---
{"dg-publish":true,"permalink":"/uni/primo-anno/analisi-1/successioni/definizioni/def-asintotico/","tags":["math","uni"]}
---

### def
due successioni sono asintotiche se
$$\tag*{def}\frac{a_n}{b_n}\rightarrow1 \iff a_n \sim b_n$$
### osservazioni
##### osservazione 1
$a_n$ e $b_n$ devono essere $\ne$ 0 definitivamente se no l'asintotico perde di significato. 
Inoltre se
$$ a_n\rightarrow l\in\mathbb{R} / \{0\} \text{ allora }a_n \sim l \text{,  } \text{ e se } a_n \sim b_n \implies b_n \rightarrow l$$
##### osservazione 2
detto $A = \{\text{successioni }\ne 0 \text{ def}\}$,  $\sim$ è una relazione di equivalenza che soddisfa le tre regole di equivalenza definite sull'insieme $A$ (riflessiva, simmetrica e transitiva).
##### osservazione 3
$$a_n \sim b_n \iff b_n = a_n(1 + \mathcal{E}_n)$$
verificare che dalla parte di destra si arriva alla parte di sinistra è immediato:
$$b_n = a_n(1 + \mathcal{E}_n) \ \ \ \ \ \frac{a_n}{b_n} = \frac{a_n}{a_n}  \frac{1}{1 + \mathcal{E}_n}$$
verifico adesso che da sinistra si arriva a destra:
$$b_n = a_n\left( \frac{b_n}{a_n} \right) = a_n(\frac{b_n}{a_n}-1+1)$$
$$\frac{b_n}{a_n}\rightarrow1 \text{ per definizione, allora } \frac{b_n}{a_n} \rightarrow1 = \mathcal{E}_n$$
$$b_n = a_n(\mathcal{E}_n +1)$$
##### osservazione 4
$$\frac{a_n}{b_n} = \frac{b_n+(b_n-a_n)}{b_n} = 1+\frac{b_n-a_n}{b_n}\rightarrow1 \iff a_n-b_n \rightarrow 0 \ \wedge b_n \nrightarrow0 \text{ (il che implica che }  a_n \nrightarrow 0 )$$
### proprietà
in generale non puoi sempre usarlo nelle funzioni tranne per certe regole : 
$$a_n \sim b_n \nRightarrow f(a_n) \sim f(b_n)$$
##### esponenti
se hai una successione [[uni/primo anno/analisi 1/successioni/definizioni/def-successione-limitata\|limitata]] $c_n$ e $a_n\sim b_n$ allora:
$$a_n^{c_n} \sim b_n^{c_n} \iff e^{c_n \log{(a_n/b_n)}} \rightarrow1$$
e naturalmente l'esponente è [[uni/primo anno/analisi 1/successioni/definizioni/def-successione-infinitesima\|infinitesimo]] $\iff$ $c_n$ è limitata.
____
##### prodotti
se $a_n \sim b_n$ allora è vero che $a_nc_n \sim b_nc_n$, questo naturalmente funziona anche con le divisioni. La dimostrazione è banale visto che ti viene $\lim 1 * \lim 1 = 1$.
___
##### esponenziali
- $se \ a_n \sim b_n \implies e^{a_n} \sim b^{b_n}$ solo per certi casi, NON VERO SEMPRE :  $\lim\frac{e^{a_n}}{e^{b_n}} \rightarrow1 \iff a_n - b_n \rightarrow0$ ma questa condizione non è conseguenza del fatto che $a_n \sim b_n$. In generale funziona se una delle due è limitata : $$a_n(1-\frac{b_n}{a_n}) = a_n\epsilon_n \rightarrow0 \iff a_n \text{ limitata}$$
- risultato operativo, per dimostrazione guarda QB1 :   
$$e^{a_n} - e^{b_n} \sim e^l(a_n-b_n) \iff \lim a_n = \lim b_n \in \mathbb{R} \land a_n\ne b_n$$
___
##### logaritmi
- se $a_n \sim b_n$ e allora quando $|a_n - 1| > \epsilon \implies |b_n - 1| > \epsilon \implies \log(a_n) \sim \log(b_n)$
- se $a_n\ne b_n$ e $a_n,b_n\rightarrow l \ne 0 \implies log(a_n)-log(b_n) \sim \frac{a_n-b_n}{l}$
___
##### polinomi
Sia
$$
p_n = c_1 n^{\alpha_1} + c_2 n^{\alpha_2} + \dots + c_k n^{\alpha_k} \quad \text{allora} \quad p_n \sim c_1 n^{\alpha_1}
$$
- qui $(c_1, c_2, \dots, c_k \in \mathbb{R}) \text{ con } (c_1 \neq 0) \text{ e } (\alpha_1 > \dots > \alpha_k)$ 
- i coefficienti reali $(c_1, \dots, c_k)$ possono essere rimpiazzati da [[uni/primo anno/analisi 1/successioni/definizioni/def-successione-limitata\|successioni limitate]] o con i logaritmi
- ad esempio: $2n^2 + (1+\cos n) \sqrt{n} - 6 \sim 2n^2$
____
### come non usarlo
- se $a_n \sim b_n$  NON VUOL DIRE SEMPRE CHE $a_n + c_n \sim b_n + c_n$
- quando usando l'asintotico e  i termini dominanti si elidono non puoi usarlo, perdi informazioni dopo l'approssimazione asintotica. Devi fare attenzione a quali sono i termini dominanti soprattutto quando si tratta di infinitesimi. PER ESEMPIO:
	- $sin^2(\epsilon_n) - \log(1+\epsilon_n)$ qui puoi usarlo, il primo termine avrà ordine generale $\alpha^2$ mentre il secondo è di ordine $\alpha$ 
	- $\epsilon_n - \frac{sin(\epsilon_n)}{n}$ qui puoi dire che il primo termine è di ordine generale $\alpha$ mentre il secondo è di ordine $\alpha + 1$ poiché $\frac{1}{n}$ è di ordine 1 e $\epsilon_n$ è di ordine $\alpha$ come prima, di conseguenza tutta l'espressione è $\sim$ al termine di ordine minore per gli infinitesimi $\implies\sim\epsilon_n$ 
- $a_n \sim b_n \nRightarrow f(a_n) \sim f(b_n)$
- 
GUARDA APPUNTI SUL QR3 / QR2
### lista asintotici 
$$\tag*{1.} \sin(\mathcal{E}_n)\sim \mathcal{E}_n$$
$$\tag*{2.} \arcsin(\mathcal{E}_n)\sim \mathcal{E}_n$$
$$\tag*{3.} \tan(\mathcal{E}_n)\sim \mathcal{E}_n$$
$$\tag*{4.} \arctan(\mathcal{E}_n)\sim \mathcal{E}_n$$
$$\tag*{5.} 1 - \cos(\mathcal{E}_n) \sim \frac{\mathcal{E}_n^2}{2}$$
$$\tag*{6.} \sinh(\mathcal{E}_n)\sim \mathcal{E}_n$$
$$\tag*{7.} \tanh(\mathcal{E}_n)\sim \mathcal{E}_n$$
$$\tag*{8.} \cosh(\mathcal{E}_n) - 1 \sim \frac{\mathcal{E}_n^2}{2}$$
$$\tag*{9.} (1 + \mathcal{E}_n)^{1/\mathcal{E}_n} \sim e$$
$$\tag*{10.} e^{\mathcal{E}_n} - 1 \sim \mathcal{E}_n$$
$$\tag*{11.a} \log(1 + \mathcal{E}_n) \sim \mathcal{E}_n$$
$$\tag*{11.b} \log a_n \sim a_n - 1 \quad [\text{se } a_n \to 1, a_n \ne 1]$$
$$\tag*{12.a} (1 + \mathcal{E}_n)^\alpha - 1 \sim \alpha \mathcal{E}_n \quad [\alpha \in \mathbb{R}]$$
$$\tag*{12.b} (1 + \mathcal{E}_n)^{a_n} - 1 \sim a_n \mathcal{E}_n \quad [\text{se } 0 \ne a_n \mathcal{E}_n \to 0]$$
$$\tag*{13.} n! \sim e^{-n} n^n \sqrt{2 \pi n} \quad (\text{de Moivre-Stirling})$$
$$\tag*{14.} \log n! \sim n \log n$$
$$\tag*{15.} \sum_{k=1}^n \frac{1}{k} \sim \log n \quad (\text{Euler-Mascheroni})$$
