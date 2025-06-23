---
lastSync: Thu May 29 2025 16:47:30 GMT+0200 (Ora legale dell’Europa centrale)
---
La precisione di un sistema di controllo si riferisce alla sua capacità di seguire il segnale di riferimento senza errori significativi in condizioni di regime permanente (cioè, dopo che la risposta transitoria si è esaurita).

L'**errore a regime** è la differenza tra il segnale di riferimento e l'uscita del sistema quando il tempo tende all'infinito

Nei sistemi di controllo, quando si parla di errori calcolabili in riferimento alla precisione a regime (o statica) di un sistema retroazionato, ci si riferisce tipicamente a tre tipi di segnali di ingresso canonici:
## Errore di Posizione ($e_{p}$)
Errore che si calcola quando l'ingresso al sistema è un gradino unitario $R(s) = \frac{1}{s}$. L'errore di posizione a regime $(e_{p \infty})$ è il valore finale dell'errore quando il tempo tende all'infinito: 

$$
e_{p∞}​= \lim_{ s \to \infty } sE(s) \left( \frac{1}{1 + G(s) H(s)} \right) \frac{1}{s} = \frac{1}{1 + K_{p} }
$$
La costante $K_{p} = \lim_{ s \to 0 } G(s) H(s)$ è detta **costante di errore statico di posizione**. L'errore $e_{p \infty}$ sarà nullo se il sistema in catena aperta $G(s)H(s)$ ha almeno un polo nell'origine (cioè il sistema è di tipo 1 o superiore).

## Errore di Velocità ($e_{v}$)
Questo errore di calcola quando l'ingresso al sistema è una rampa unitaria $\left( R(s) = \frac{1}{s^2} \right)$. L'errore di velocità a regime $e_{p \infty}$ è il valore finale dell'errore:
$$
e_{p∞}​= \lim_{ s \to \infty } sE(s) \left( \frac{1}{1 + G(s) H(s)} \right) \frac{1}{s^2} = \frac{1}{K_{v} }
$$
La costante $K_{v} = \lim_{ s \to 0 } sG(s) H(s)$ è detta **costante di errore statico di velocità**. L'errore $e_{v \infty}$ sarà nullo se il sistema in catena aperta $G(s) H(s)$ ha almeno due poli nell'origine (cioè il sistema è di tipo 2 o superiore)

## Errore di Accelerazione ($e_{a}$)
Questo errore si calcola quando l'ingresso al sistema è una parabola unitaria $\left( R(s) = \frac{1}{s^3} \right)$. L'errore di accelerazione a regime $e_{p \infty}$ è il valore finale dell'errore:

$$
e_{p∞}​= \lim_{ s \to \infty } s^{2} E(s) \left( \frac{1}{1 + G(s) H(s)} \right) \frac{1}{s^3} = \frac{1}{K_{a} }
$$
La costante $K_{a} = \lim_{ s \to 0 } {s^2} G(s) H(s)$ è detta **costante di errore statico di accelerazione**. L'errore $e_{v \infty}$ sarà nullo se il sistema in catena aperta $G(s)H(s)$ ha almeno tre poli nell'origine (cioè il sistema è di tipo 3 o superiore).

---
### Precedente


### Successivo
[Tipo di sistema](Tipo%20di%20sistema.md)

### Riferimenti
[Transitorio esaurito](Transitorio%20esaurito.md)