---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/gal/definizioni/def-sotto-spazio-vettoriale-tbf/","tags":["math","uni"],"updated":"2026-03-25T20:19:10.109+01:00"}
---

sia $V$ uno [[01-uni/primo-anno/gal/definizioni/def-spazio-vettoriale\|spazio vettoriale]] (abbreviato s.v.) e sia $H \subseteq V$, se $H$ è uno s.v allora esso si definisce $\text{sotto spazio vettoriale}$ di $V$. Come faccio allora a controllare che $H$ sia uno s.v.? Noto subito che la maggior parte degli assiomi d s.v. sono asserzioni che riguardato tutti gli elementi ($\forall \dots$) dello spazio e si estendono anche al sottospazio necessariamente. Le vere cose che devo controllare sono le seguenti:
$$ V \ne \emptyset \tag{0.1}$$
$$+ : V\times x \to V \tag{0.1}$$
$$\cdot : \mathbb{R} \times V \to V \tag{0.2}$$
$$\forall u \in V \ \exists u \in V : u+v = v \tag{3}$$
$$\forall u \in V \ \exists u \in V : v+u = \underline{0} \tag{4}$$
perché naturalmente non è certo che se creo un sottoinsieme l'elemento neutro e tutti gli elementi opposti siano contenuti in questo sottoinsieme e non è nemmeno certo che nell'insieme che sto creando le operazioni di $V$ siano $interne$ anche a $H$.
### teorema controllo s.s.v
$$H \subseteq V \text{ è s.s.v. di } V \iff $$
$$\tag{1} H \ne \emptyset$$
$$\tag{2} \forall h,k \in H\, \ \  h+k \in H $$
$$\tag{3}\forall a \in \mathbb{R},\forall h \in H, \ \ a\cdot h \in H$$

### dim-(tbd)
