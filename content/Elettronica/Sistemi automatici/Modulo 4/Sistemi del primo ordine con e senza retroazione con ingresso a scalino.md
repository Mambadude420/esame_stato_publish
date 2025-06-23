---
lastSync: Sun Jun 15 2025 15:35:54 GMT+0200 (Ora legale dell’Europa centrale)
---
I sistemi del primo ordine sono i "mattoni" più semplici e fondamentali per capire il comportamento dinamico di molti processi fisici. Anche se semplici, modellano un'ampia varietà di fenomeni, dal riscaldamento di un oggetto alla carica di un condensatore.

Un **sistema del primo ordine** è un sistema la cui dinamica è descritta da un'equazione differenziale del primo ordine. Nel dominio di Laplace, la sua Funzione di Trasferimento (FDT) ha la forma generale:
$$
G(s)=\frac{K}{τs + 1}​
$$
Dove:

- $K$ è il **[guadagno statico](Guadagno%20statico.md)** del sistema. Ci dice qual è il valore finale che l'uscita raggiunge a regime, una volta che il transitorio è terminato, in risposta a un ingresso costante.
- $\tau$ (tau) è la **[costante di tempo](Costante%20di%20tempo.md)** del sistema. È un parametro cruciale che ci indica quanto "velocemente" il sistema risponde a un cambiamento nel suo ingresso. Un τ piccolo significa una risposta rapida, un τ grande significa una risposta lenta.

---
#### Sistemi del Primo Ordine Con Retroazione
Ora, cosa succede se inseriamo questo sistema del primo ordine in un **anello di retroazione negativa** (supponiamo per semplicità una retroazione unitaria, $H(s)=1$)?

La funzione di trasferimento ad anello chiuso GCL​(s) sarà:
$$
G_{CL​}(s)=1+\frac{G(s)}{H(s)G(s)}​= \frac{{\frac{K}{\tau s + 1}}}{1 + \frac{K}{\tau s + 1} \cdot 1}​
$$
Semplificando l'espressione:
$$
G_{CL}​(s) = \frac{{K}}{\tau s + 1 + K} = \frac{K}{(\tau)s + (1 + K)}
$$
Per renderla nella forma standard di un sistema del primo ordine $(K′/(τ′s+1))$, dividiamo numeratore e denominatore per $(1+K)$:
$$
G_{CL}​(s)=\frac{\frac{K}{(1+K)}}{{\frac{\tau}{1 + K}s} + 1}​
$$

Analizzando questa nuova FDT ad anello chiuso, possiamo identificare il **nuovo guadagno statico** $K′$ e la **nuova costante di tempo** $τ′$:

- **Nuovo guadagno statico:** $K′=\frac{K}{1+K}$
- **Nuova costante di tempo:** $τ′= \frac{\tau}{1 + K}​$

**Cosa impariamo da questo?**
1. **Il guadagno statico si riduce:** Se K è positivo, K′ sarà sempre minore di K. Questo significa che la retroazione "attenua" l'effetto finale dell'ingresso sull'uscita. Potrebbe sembrare uno svantaggio, ma è un compromesso necessario per la stabilità e la riduzione dei disturbi.
2. **La costante di tempo si riduce:** τ′ è sempre minore di τ (se K è positivo). Questo è un enorme vantaggio! **La retroazione rende il sistema più veloce!** Il tempo di risposta diminuisce, il che significa che il sistema raggiunge il suo valore di regime più rapidamente.

La retroazione ha quindi un doppio effetto su un sistema del primo ordine: ne riduce il guadagno, ma ne aumenta significativamente la velocità di risposta, rendendolo più reattivo e meno suscettibile ai disturbi.