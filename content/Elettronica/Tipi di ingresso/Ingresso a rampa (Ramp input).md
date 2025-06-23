---
lastSync: Thu May 15 2025 13:45:21 GMT+0200 (Ora legale dell’Europa centrale)
---
Un ingresso a rampa rappresenta un segnale che aumenta (o diminuisce) linearmente nel tempo a partire da un certo istante. Un esempio è la velocità di un'auto che accelera costantemente.

- Forma matematica:
	$$
	u(t) =
	\begin{cases}
	0, t < 0 \\
	Bt, t \geq 0
	\end{cases}
	$$
	Dove $B$ è la pendenza della rampa (la velocità di cambiamento). Se $B = 1$, si parla di rampa unitaria

- Trasformata di Laplace: $U(s) = \frac{B}{s^2}$
	È utile per valutare la capacità di un sistema di seguire un segnale che varia nel tempo con una velocità costante, e per determinare l'errore di inseguimento a regime in tali condizioni. Ad esempio, il controllo della posizione di un robot che deve muoversi a velocità costante lungo una traiettoria.


---
### Precedente


### Successivo


### Riferimenti
[[Step input)](Ingresso a gradino (Step input|Ingresso a gradino (Step input)]].md)
[[Parabolic input)](Ingresso a parabola (Parabolic input|Ingresso a parabola (Parabolic input)]].md)