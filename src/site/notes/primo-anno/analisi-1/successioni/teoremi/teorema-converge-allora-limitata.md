---
{"dg-publish":true,"permalink":"/primo-anno/analisi-1/successioni/teoremi/teorema-converge-allora-limitata/","tags":["math","uni"],"updated":"2026-02-24T15:52:00.488+01:00"}
---

se $a_n \rightarrow l \in \mathbb{R} \implies a_n$ è limitata
### ==dim==
il concetto è che devi fissare $\epsilon=1$ allora $\exists n_0 : \forall n\ge n_0 \ \ |a_n-l|<\epsilon$ e chiami 
$$k:=\max\{a_0,a_1,...,a_{n_0-1}, l+1\}$$
$$h:=\min\{a_0,a_1,...,a_{n_0-1},l-1\}$$
$$\implies\forall n, \ \ h\le a_n\le k$$
(sarebbe più rigoroso mostrare che vale $\forall n< n_0$ e $\forall n \ge n_0$ ma è uguale)

