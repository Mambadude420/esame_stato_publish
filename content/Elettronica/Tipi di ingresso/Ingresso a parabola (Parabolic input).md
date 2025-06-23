---
lastSync: Thu May 15 2025 13:45:02 GMT+0200 (Ora legale dell’Europa centrale)
---
Un ingresso a parabola rappresenta un segnale che varia quadraticamente nel tempo a partire da un certo istante, come l'accelerazione costante di un oggetto.

- Forma matematica:
	$$
	u(t) =
	\begin{cases}
	0, t < 0 \\
	\frac{Ct^2}{2}, t \geq 0
	\end{cases}
	$$
	Dove $C$ è legata all'accelerazione. Se $C = 1$, si parla di parabola unitaria. Il fattore $1/2$ è spesso incluso per semplificare la sua trasformata di Laplace.

- Trasformata di Laplace: $U(s) = \frac{C}{s^3}$
	È utilizzato per analizzare la capacità di un sistema di seguire segnali con accelerazione costante e per valutare l'erroe di inseguimento a regime in queste condizioni. È meno comune degli ingressi a gradino e rampa, ma utile per sistemi che devono gestire variazioni di accelerazione.


---
### Precedente


### Successivo


### Riferimenti
[Ingresso a gradino (Step input)](Ingresso%20a%20gradino%20(Step%20input).md)
[Ingresso a rampa (Ramp input)](Ingresso%20a%20rampa%20(Ramp%20input).md)