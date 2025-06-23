---
lastSync: Thu May 15 2025 15:14:23 GMT+0200 (Ora legale dell’Europa centrale)
---
Gli integratori nelle funzione di trasferimento ad anello aperto $G(s) H(s)$ sono i termini nella forma $\frac{1}{s}$.

Nel dominio tempo, un'operazione di integrazione è descritta dalla seguente relazione:
$$
y(t) = \int u(r) dr
$$
Applicando la Trasformata di Laplace (con condizioni iniziali nulle), otteniamo:
$$
Y(s) = \frac{1}{s}U(s)
$$
Quindi nel dominio di Laplace, l'operazione di integrazione nel tempo corrisponde a una moltiplicazione per $\frac{1}{s}$. Questo termine $\frac{1}{s}$ nel denominatore della funzione di trasferimento rappresenta un integratore.

#### Effetto degli integratori sul sistema:
Un integratore in un sistema di controllo ha la proprietà di "accumulare" l'errore nel tempo. Questo è il motivo per cui i sistemi con integratori sono in grado di ridurre o eliminare l'errore a regime per ingressi costanti.
- Se c'è un errore costante, l'integratore continuerà ad aumentare il segnale di controllo nel tempo, fino a quando l'errore non viene azzerato.