---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/gal/definizioni/def-indipendenza-lineare/","tags":["math","uni"],"updated":"2026-03-20T09:50:35.808+01:00"}
---

### indipendenza lineare
Un insieme di vettori $S = \{ v_{1},v_{2},\dots,v_{n} \}$ dello [[01-uni/primo-anno/gal/definizioni/def-spazio-vettoriale\|spazio vettoriale]] $V$ si dice $linearmente\  indipendente$ se :
$$t_{i} \in \mathbb{R}$$
$$t_{1}v_{1}+t_{2}v_{2}+\dots+t_{n}v_{n} = \underline{0} \implies t_{1}=t_{2}=\dots=t_{n} = 0$$
ovvero che il vettore nullo $\underline{0}$ di $V$ si può creare come [[01-uni/primo-anno/gal/definizioni/def-combinazione-lineare\|combinazione lineare]] degli elementi di $S$ solo se metti come pesi tutti $0$. 
### dipendenza lineare
Stessa cosa dell'indipendenza lineare, se puoi creare lo $\underline{0} \in V$ come una combinazione **non banale** (almeno uno dei pesi non nulli) allora i vettori di $S$ sono linearmente dipendenti : 
$$t_{1}v_{1}+t_{2}v_{2} +\dots+t_{n}v_{n} = \underline{0} \not \Rightarrow t_{1}=t_{2}=\dots=t_{n} = 0$$
### intuizione
Cosa c'entra che puoi creare lo $\underline{0} \in V$ con una combinazione lineare dove almeno uno dei pesi è non nullo e che sono linearmente indipendenti? In pratica ti sta dicendo che uno dei vettori di $S$ può essere "raggiunto" da una combinazione lineare degli altri elementi di $S$ :
$$S = \{ v_{1},v_{2},\dots,v_{n}, w \}$$
$$t_{1}v_{1}+t_{2}v_{2} +\dots+t_{n}v_{n} + t_{n+1}w = \underline{0} \not \Rightarrow t_{1}=t_{2}=\dots=t_{n} = t_{n+1} = 0$$
$$\implies t_{n+1}w = -(t_{1}v_{1}+t_{2}v_{2}+\dots+t_{n}v_{n})$$
$$\implies w = -\frac{1}{t_{n+1}}(t_{1}v_{1}+t_{2}v_{2}+\dots+t_{n}v_{n})$$
$$\implies w = L_{S\setminus {w}} ( \ \underline{t}\ )$$
dove con $L_{S \setminus {w}}$ intendo una combinazione lineare dei vettori $\{ v_{1},v_{2},\dots,v_{n} \}$ e con $\underline{t}$ un vettore di pesi dove almeno un $t_{i} \ne 0$. 
###### esempio
per mappare il piano cartesiano hai bisogno di almeno due vettori perpendicolari in modo che le loro combinazioni lineari possano raggiungere tutti i punti del piano. A partire dai due versori 
$$(\hat{u}_{x} \hat{u}_{y})$$
Non è possibile moltiplicare uno dei due versori per un coefficiente $\in \mathbb{R}$ in modo da arrivare sull'altro. Se invece a questa coppia aggiungo un'altro versore $\hat{u}_{xy}$ che punta nella direzione della bisettrice del 1°/3° quadrante, adesso ho effettivamente un modo per raggiungere questo terzo versore a partire dai primi due : 
$$\exists a,b \in \mathbb{R} : a\hat{u}_{x} + b\hat{u}_{y} = \hat{u}_{xy}$$
dove almeno uno tra $a,b$ è diverso da 0 (se no il vettore $\hat{u}_{xy}$ sarebbe il vettore nullo). Da questa espressione si giunge al ragionamento che si è fatto prima sul perché è utile controllare se il vettore nullo è raggiungibile da una combinazione lineare non banale, è lo stesso ragionamento fatto adesso ma al contrario, rigirando i termini dell'equazione : 
$$\exists a,b,c \in \mathbb{R} : a\hat{u}_{x} + b\hat{u}_{y} +c\hat{u}_{xy} = 0$$
