---
lastSync: Fri May 30 2025 16:48:35 GMT+0200 (Ora legale dell’Europa centrale)
---
La probabilità condizionata entra in gioco quando la probabilità di un evento dipende dal fatto che un altro evento si sia già verificato.

In altre parole, la probabilità condizionata risponde alla domanda: "Qual è la probabilità che l'evento A si verifichi, _dato che_ l'evento B si è già verificato?".

Sia indica con $P(A|B) = \frac{{P(A \cap B)}}{P(B)}$
Dove:
- $P(A|B)$ è la probabilità che si verifichi l'evento A, dato che si è verificato l'evento B.
- $M(A \cap B)$ ("P di A intersezione B") è la probabilità che si verifichino sia l'evento A che l'evento B contemporaneamente (la probabilità dell'intersezione dei due eventi).
- $P(B)$ è la probabilità che si verifichi l'evento B.

**Esempio:**
Si immagini di lanciare un dado a sei facce:
- Evento A: Ottenere un numero pari ({2, 4, 6})
- Evento B: Ottenere un numero maggiore di 3 ({4, 5, 6})
Vogliamo calcolare $P(A|B)$, ovvero la probabilità di ottenere un numero pari, *dato* che il numero p maggiore di 3.