---
{"dg-publish":true,"permalink":"/primo-anno/statistica/schemi-primo-parziale/","tags":["uni"],"updated":"2026-04-21T15:08:12.756+02:00"}
---

# grafici
- istogramma usa densità (dividi per la larghezza della classe)
- box plot ha come rettangolo la IQR, la riga in mezzo è la mediana e le due linee tratteggiate (il range degli outliers) sono 
	- Q1- 3/2 IQR (o min val)
	- Q3 + 3/2 IQR 
___
# formule generali
$$E(X) = \sum x f(x) = \int_{-\infty}^{+\infty} xf(x)dx$$
$$Var(X) = E(X^2)-E(X)^2$$
$$\overline{X} = \frac{1}{n}\sum_{i = 1}^n x$$
$$S^2 = \frac{1}{n-1}\sum(x- \overline{X})^2$$
(questa la usi sui campioni)
___
# V.A. discrete
### binomiale
Eventi indipendenti con $n$ ripetizioni dove la probabilità dell'evento è $p$.  $X$ rappresenta quindi il numero di successi, se $X = 1$ vuol dire che in $n$ ripetizioni hai avuto un successo. 
$$X \sim Bin(n, p)$$
$$f(x) = \binom{n}{x}p^x(1-p)^{n-x}$$
$$E(X) = np$$
$$Var(X) = np(1-p)$$
### poisson 
Come nella binomiale gli eventi sono indipendenti ma questa non hai $n$ ripetizioni ma hai un'intervallo continuo di possibilità (decadimento di particelle -> volume). Il parametro $\lambda$ è il valore atteso nell'intervallo (l'intervallo è costante e identicamente distribuito).
$$X \sim Poisson(\lambda)$$
$$f(x) = e^{-\lambda} \frac{\lambda^x}{x!}$$
$$E(X) = \lambda$$
$$Var(X) = \lambda$$
____
# V.A. continue
### esponenziale
$$X \sim Exp(\lambda)$$
$$f(x) = \lambda e^{-\lambda x}$$
$$E(X) = \frac{1}{\lambda}$$
$$Var(X) = \frac{1}{\lambda^2}$$
### gaussiana
$$X \sim N(\mu, \sigma^2)$$
$$f(x) = \dots$$
$$E(X) = \mu$$
$$Var(X) = \sigma^2$$

### Teorema Centrale del Limite
Siano $X_i \sim i.i.d.(\mu, \sigma^2)$ con $n \to \infty$: 
$$\text{ somma : }S_n \approx N(n\mu, n\sigma^2) \implies Z = \frac{S_n - n\mu}{\sigma\sqrt{n}}$$
$$\text{ media : }\bar{X}_n \approx N(\mu, \frac{\sigma^2}{n}) \implies Z = \frac{\bar{X}_n - \mu}{\sigma/\sqrt{n}}$$
