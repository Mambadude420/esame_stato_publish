---
lastSync: Thu May 15 2025 02:16:33 GMT+0200 (Ora legale dell’Europa centrale)
---
In un sistema di controllo ad anello chiuso, l'uscita del sistema viene misurata da un sensore e confrontata con il segnale di riferimento (il valore desiderato). La differenza tra il riferimento e l'uscita misurata è l'errore. Questo segnale di errore viene quindi utilizzato dal [controllore](Controllore%20(G(s)).md) per generare un segnale di controllo che agisce sull'[attuatore](Attuatore.md), il quale a sua volta influenza l'impianto (il sistema che vogliamo controllare) per ridurre l'errore. Questo processo forma un "anello" chiuso di azione e reazioni.

#### Vantaggi del controllo a retroazione
- **Riduzione dell'errore a regime**: La retroazione può ridurre o eliminare l'errore tra l'uscita desiderata e quella effettiva in condizioni stazionarie.
- **Miglioramento della risposta dinamica**: La retroazione può influenzare la velocità di risposta, l'[overshoot](Overshoot.md) e altre caratteristiche della risposta transitoria del sistema.
- **Riduzione della sensibilità alle variazioni dei parametri dell'impianto**: Un sistema ad anello chiuso può essere meno influenzato da cambiamenti nei parametri dell'impianto o da disturbi esterni rispetto a un sistema ad anello aperto.
- **Stabilizzazione di sistemi instabili**: La retroazione può essere utilizzata per rendere stabili sistemi che altrimenti sarebbero instabili.