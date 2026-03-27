---
{"dg-publish":true,"permalink":"/01-uni/primo-anno/gal/definizioni/def-rango/","tags":["math","uni"],"updated":"2026-03-27T20:26:01.703+01:00"}
---

### rango per pivots
il rango per pivots $r$ di una [[01-uni/primo-anno/gal/definizioni/def-matrice-(tbf)\|matrice]] $A$ è il numero di righe non nulle della matrice a scala $U$ ottenuta usando il [[01-uni/primo-anno/gal/definizioni/def-metodo-eliminazione-gauss-(tbf)\|MEG]] su $A$ (definizione momentanea), in pratica indica il numero di equazioni indipendenti della matrice.
### rango per righe
Il rango per righe è definito come la [[01-uni/primo-anno/gal/definizioni/def-dimensione\|dimensione]] dello [[01-uni/primo-anno/gal/definizioni/def-spazio-riga\|spazio riga]] di $A$ :
$$rank_{row}(A) = \dim { Row (A)}$$
### rango per colonne
Il rango per colonne è definito come la [[01-uni/primo-anno/gal/definizioni/def-dimensione\|dimensione]] dello [[01-uni/primo-anno/gal/definizioni/def-spazio-colonna\|spazio colonna]] di $A$ : 
$$rank_{col}(A) = \dim{Col(A)}$$
però grazie a [[01-uni/primo-anno/gal/teoremi/teorema-rango-righe-colonne-(tbd)\|questo teorema]] sai che il rango per righe è uguale al rango per colonne, rappresenta sempre il numero di "informazioni diverse" contenute nella matrice: 
- se puoi derivare una riga dalle altre vuol dire quel vincolo è superfluo
- se puoi derivare una colonna dalle altre vuol dire che quella colonna è già "raggiunta" dalle altre.
