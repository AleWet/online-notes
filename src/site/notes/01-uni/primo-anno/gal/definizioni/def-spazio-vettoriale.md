---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/gal/definizioni/def-spazio-vettoriale/","tags":["math","uni"],"updated":"2026-03-24T10:48:45.193+01:00"}
---

assumerò sempre che $V$ sia un insieme non vuoto di vettori :  $V \neq \emptyset$ e che il campo preso è $\mathbb{R}$ per semplicità. Importante citare anche che i vettori non sono solo "array" di numeri ma qualsiasi cosa su cui tu possa definire delle operazioni analoghe a quelle spiegate qui.
### assiomi
chiamo spazio vettoriale un oggetto $(V,\mathbb{R}, +, \cdot)$ formato da
- insieme di vettori $V$ 
- un [[01-uni/primo-anno/analisi-1/basi-successioni/definizioni/def-campo\|campo]] (in questo caso $\mathbb{R}$) 
- due operazioni $interne$ : 
$$+ : V\times x \to V \tag{0.1}$$
$$\cdot : \mathbb{R} \times V \to V \tag{0.2}$$
tali che hanno le seguenti proprietà:
$$\forall u, v, w \in V  \ u + (v+ w) = (u+v)+w\tag{1} $$
$$\forall u, v \in V \ u+v = v+u \tag{2}$$
$$\forall u \in V \ \exists u \in V : u+v = v \tag{3}$$
$$\forall u \in V \ \exists u \in V : v+u = \underline{0} \tag{4}$$
(equivalenti alle proprietà di [[01-uni/primo-anno/analisi-1/basi-successioni/definizioni/def-gruppo#gruppo abeliano\|gruppo abeliano]])
$$\forall a,b, \in \mathbb{R}, \forall v \in V \ (a\cdot b)\cdot v = a\cdot (b\cdot v) \tag{5}$$
$$\forall a \in \mathbb{R} \ \forall w, v \in V \ a(u+w) = au + aw \tag{6}$$
$$\forall a,b \in \mathbb{R} \ \forall u \in V \ \ (a+b)v = av + bv \tag{7}$$
$$\forall u \in V  \ \exists a \in \mathbb{R} : av = v \tag{8}$$

tutto ciò che rispetta questi assiomi è uno spazio vettoriale, per esempio se prendo $(\mathbb{R}^3, \mathbb{R}, \cdot, +)$ e definisco la somma come:
$$(a, b, c) + (d,e,f) := (a+c,b+d, c+f)$$ e il prodotto come
$$a(b,c,d) := (ab,ac,ad)$$
ottengo uno spazio vettoriale. Queste definizioni di somma e prodotto sono quello che definisce spazio vettoriale, se avessi definito altre operazioni per somma e prodotto potrei non creare più uno spazio vettoriale con l'oggetto di partenza $(\mathbb{R}^3, \mathbb{R}, \cdot, +)$. Se però tengo questa definizione di somma e prodotto $element-wise$ (elemento per elemento) otterrò sempre uno spazio vettoriale 
$$\forall n \in \mathbb{N} \setminus \{ 0 \}, \ (\mathbb{R}^n, \mathbb{R}, \cdot, +) \text{ è uno spazio vettoriale}$$
per più esempi guarda appunti lezione 9/03/26
### osservazione 1
Notare che, poiché gli spazi vettoriali devono "passare per l'origine", il sistema di equazioni associato ad uno spazio vettoriale avrà sempre come termine noto $0$, di conseguenza se creo la "matrice associata" ad uno spazio vettoriale (ovvero quella che ha i coefficienti del sistema lineare che descrive lo spazio in funzione delle [[01-uni/primo-anno/gal/definizioni/def-base\|basi]] avrò sempre sottinteso l'ultima colonna $=0$.