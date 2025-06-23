---
lastSync: Wed May 28 2025 11:25:06 GMT+0200 (Ora legale dell’Europa centrale)
---
Il motore passo-passo ([stepper motor](Step%20motor.md)) è un attuatore che, pilotato da segnali elettrici digitali, ruota di un angolo fisso $\gamma$, chiamato *passo*, a ogni commutazione dei segnali di comando.

Il motore passo-passo vien largamente utilizzato nei posizionamenti di precisione.

La sua velocità di rotazione è strettamente legata alla frequenza di clock $f$ dei segnali digitali di comando.

Indicando con $S = \frac{{360^\circ}}{\gamma}$ il numero di passi al giro, $\frac{f}{s}$ fornisce il numero di giri al secondo e quindi la velocità $n$ del motore, espressa in giri/min, vale:
$$
n = \frac{{60f}}{S}
$$