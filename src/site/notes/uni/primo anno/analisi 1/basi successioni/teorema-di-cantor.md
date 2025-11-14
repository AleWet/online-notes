---
{"dg-publish":true,"permalink":"/uni/primo-anno/analisi-1/basi-successioni/teorema-di-cantor/","tags":["math","uni"]}
---

Tesi : dato un insieme generico $A$, l'insieme delle parti $P(A)$ ha cardinalità maggiore dell'insieme di partenza : 
$$\#A < \#P(A)$$
questo vale sia per insiemi finiti che insiemi non finiti.
___
### ==g  r4dim==
Per assurdo $\exists f:A\rightarrow P(A)$ tale che $f$ è biunivoca. 
$$B=\{a \in A : a \not\in f(a)\}$$
creo l'insieme degli elementi che non sono collegati da $f$ ad un insieme che li contiene.
$$\implies \exists b \in A : f(b) = B$$
$$\implies b \in B \text{ oppure } b \not \in B$$
$$\tag*{primo caso} b \in B \implies b \not\in f(b) = B \text{ (è contenuto nella sua immagine) } $$
$$\tag*{secondo caso} b \not\in B \implies b \in B \text{ (non è contenuto nella sua immagine)}$$
allora raggiungo un antinomia $\implies$ non esiste una funzione $f$ biunivoca $\implies \#A < \#P(A)$.
