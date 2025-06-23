---
lastSync: Sun Jun 15 2025 16:13:34 GMT+0200 (Ora legale dell’Europa centrale)
---
#### Formula funzione di trasferimento di un sistema del secondo ordine
La formula:
$$
G(s) = \frac{{K \omega_{n}^2}}{s^{2} + 2 \zeta \omega_{n}s + \omega_{n}^{2}}
$$
rappresenta la relazione tra l'ingresso $U(s)$ e l'uscita $Y(s)$ di un sistema lineare tempo-variante (LTI) nel dominio di Laplace, dove $Y(s) = G(s)U(s)$ oppure $G(s) = \frac{Y(s)}{U(s)}$.

#### I termini:
##### G(s)
È la **funzione di trasferimento del sistema**. È una rappresentazione nel dominio della frequenza complessa $(s)$ del comportamenti dinamico del sistema.

##### K
Il **guadagno statico** del sistema.

##### $\omega_{n}$
La **frequenza (pulsazione) naturale non smorzata**. È la frequenza con cui il sistema oscillerebbe se non ci fosse smorzamento. Più $\omega_{n}$ è altra, più il sistema è "veloce" nel rispondere.

##### $\zeta$
Il **rapporto di smorzamento**. Questo parametro adimensionale determina il tipo di risposta del sistema:
- **$\zeta < 1$ (sotto-smorzato)**: Il sistema oscilla prima di assestarsi
- **$\zeta =1$ (criticamente smorzato)**: Il sistema si assesta nel modo più veloce possibile senza oscillazioni.
- **$\zeta > 1$ (sovra-smorzato)**: Il sistema si assesta lentamente senza oscillazioni.

##### $s$
La variabile di Laplace. Rappresenta l'operatore di derivazione nel dominio del tempo, trasformato nel dominio della frequenza complessa.