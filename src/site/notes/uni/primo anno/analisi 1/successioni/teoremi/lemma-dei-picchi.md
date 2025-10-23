---
{"dg-publish":true,"permalink":"/uni/primo-anno/analisi-1/successioni/teoremi/lemma-dei-picchi/","tags":["math","uni"]}
---

data una successione $a_n$, allora essa ammette una successione monotona
### ==dim==
definisco **picco** un elemento $a_{n0}$ tale che :
$$\forall n > n_0, a_n<a_{n0}$$
quindi è l'elemento della successione $a_n$ più grande da $n_0$ in poi. Da qui si distinguono due casi:

1) i picchi sono **infiniti**, allora posso prendere la sottosuccessione formata dai picchi che per come li ho definiti è [[uni/primo anno/analisi 1/successioni/definizioni/def-successione-monotona\|monotona decrescente]]
2) i picchi sono **finiti**, allora :
   detto l'ultimo picchi $a_{n0}$ posso prendere l'elemento successivo $a_{n1}$ e questo sarà il primo elemento della mia sottosuccessione. Visto che $a_{n1}$ non è un picco (poiché è $<a_{n0}$) allora è garantito dalla definizione di picco che $\exists \ n2 > n1$ tale che $a_{n2} > a_{n1}$. Sia $a_{n2}$ il prossimo elemento della sottosuccessione allora ripeto la stessa procedura (non è un picco $\implies \exists n3$ tale che ...). Tutti gli elementi della sottosuccessione sono in ordine crescente allora la sottosuccessione è [[uni/primo anno/analisi 1/successioni/definizioni/def-successione-monotona\|monotona]]