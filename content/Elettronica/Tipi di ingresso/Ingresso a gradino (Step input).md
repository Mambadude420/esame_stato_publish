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
	È fondamentale per valutare la [[Risposta transitoria.md|risposta transitoria]] di un sistema, come il tempo di salita, l'[[Overshoot.md|overshoot]], il [[Sistemi di controllo in catena chiusa.md#^c9f103|tempo di assestamento]] e l'[[Errore a regime costante e non nullo.md#^76f787|errore a regime]] quando il sistema è soggetto a un cambiamento improvviso nel riferimento o a un disturbo costante.


---
### Precedente


### Successivo


### Riferimenti
[[Ramp input)](Ingresso a rampa (Ramp input|Ingresso a rampa (Ramp input)]].md)
[[Parabolic input)](Ingresso a parabola (Parabolic input|Ingresso a parabola (Parabolic input)]].md)