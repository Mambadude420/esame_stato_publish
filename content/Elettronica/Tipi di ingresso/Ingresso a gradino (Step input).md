---
lastSync: Sat Jun 14 2025 17:31:43 GMT+0200 (Ora legale dell’Europa centrale)
---
Un ingresso a gradino rappresenta un cambiamento improvviso e mantenuto costante nel valore del segnale d ingresso. Ad esempio quando si accende un interruttore: il segnale passa istantaneamente da zero a un valore costante.

- Forma matematica:
	$$
	u(t) =
	\begin{cases}
	0, t < 0 \\
	A, t \geq 0
	\end{cases}
	$$
	Dove $A$ è l'ampiezza del gradino. Se $A = 1$, si parla di gradino unitario

- Trasformata di Laplace: $U(s) = \frac{A}{s}$
	È fondamentale per valutare la [risposta transitoria](Risposta%20transitoria.md) di un sistema, come il tempo di salita, l'[overshoot](Overshoot.md), il [](Sistemi%20di%20controllo%20in%20catena%20chiusa.md#^c9f103|tempo%20di%20assestamento) e l'[](Errore%20a%20regime%20costante%20e%20non%20nullo.md#^76f787|errore%20a%20regime) quando il sistema è soggetto a un cambiamento improvviso nel riferimento o a un disturbo costante.


---
### Precedente


### Successivo


### Riferimenti
[Ingresso a rampa (Ramp input)](Ingresso%20a%20rampa%20(Ramp%20input).md)
[Ingresso a parabola (Parabolic input)](Ingresso%20a%20parabola%20(Parabolic%20input).md)