---
lastSync: Sun Jun 15 2025 18:52:37 GMT+0200 (Ora legale dell’Europa centrale)
---
L'**errore a regime** ($e_{ss}$​ o $e_{\infty}$​) è uno dei parametri di prestazione più importanti per un sistema di controllo. Ci dice quanto l'**uscita del sistema differisce dal valore di riferimento desiderato** quando il sistema si è stabilizzato, cioè dopo che tutti i transitori si sono esauriti e il tempo $t$ tende all'infinito.

Idealmente, vorremmo un errore a regime nullo, il che significherebbe che il sistema raggiunge perfettamente il suo obiettivo. Tuttavia, in molti sistemi pratici, può esserci un errore a regime costante e non nullo, o addirittura infinito.

Per calcolare l'errore a regime, ci affidiamo al **Teorema del Valore Finale** che abbiamo visto nel Modulo 1. Se E(s) è la Trasformata di Laplace del segnale di errore (la differenza tra riferimento e uscita), allora l'errore a regime è:
$$
e_{ss} = \lim_{ t \to \infty } e(t) = \lim_{ s \to 0 } sE(s)
$$
**Come si ottiene E(s)?**
Assumendo retroazione unitaria per semplicità, H(s) = 1, il segnale di errore $E(s)$ è dato dalla differenza tra il riferimento $R(s)$ e l'uscita $Y(s)$:
$$
E(s) = R(s) - Y(s)
$$
$$
E(s) = \frac{1}{1 + G(s)} R(s)
$$
Dove $G(s) = C(s)P(s)$ è la funzione di trasferimento ad anello aperto (senza il blocco di feedback se la retroazione non è unitaria, quindi $G(s)$ include controllore e processo).

Sostituendo $E(s)$ nella formula del teorema del valore finale:
$$
e_{ss} = \lim_{ s \to 0 } s \left( \frac{1}{1 + G(s)} R(s) \right)
$$
