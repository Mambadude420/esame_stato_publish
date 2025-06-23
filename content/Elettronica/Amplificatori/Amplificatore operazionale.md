---
lastSync: Tue May 13 2025 16:46:37 GMT+0200 (Ora legale dell’Europa centrale)
---
Un amplificatore operazionale, spesso chiamato "op-amp", è un circuito integrato (un piccolo chip elettronico) che si comporta come un amplificatore di tensione ad alto guadagno. In altre parole, prende un segnale di tensione in ingresso (anche molto piccolo) e lo amplifica, producendo un segnale di tensione in uscita molto più grande.

![Schema Amplificatore Operazionale Non-invertente](Schema%20Amplificatore%20Operazionale%20Non-invertente.png)

### Caratteristiche Ideali di un amplificatore operazionale
Le caratteristiche ideali (che che op-amp non raggiungono perfettamente) sono:
- **Guadagno di tensione ad anello aperto infinito** ($A_{OL} \rightarrow \infty$): Ciò significa che una piccolissima differenza di tensione tra i suoi ingressi produce un'uscita enormemente grande.
- **Resistenza di ingresso infinita** ($R_{in} \rightarrow \infty$): L'op-amp ideale può fornire qualsiasi quantità di corrente all'uscita senza che la sua tensione diminuisca.
- **Resistenza di uscita zero** ($R_{out} \rightarrow \infty$): L'op-amp ideale può fornire qualsiasi quantità di corrente all'uscita senza che la sua tensione diminuisca.
- **Banda passante infinita**: L'op-amp ideale può amplificare segnali di qualsiasi frequenza allo stesso modo.

### I terminali di un amplificatore operazionale
Un op-amp ha tipicamente cinque terminali principali:
1. Ingresso non invertente (+): Un segnale applicato a questo terminale produce un segnale di uscita con la stessa fase.
2. Ingresso invertente (-): Un segnale applicato a questo terminale produce un segnale di uscita con fase invertita di 180 gradi.
3. **Uscita**: Il segnale amplificato è disponibile su questo terminale.
4. **Alimentazione positiva ($V_{CC}$ o $V_+$)**: Fornisce l'energia per il funzionamento dell'op-amp.
5. **Alimentazione negativa ($V_{EE}$ o $V_{-}$ o GND)**: Fornisce l'altro riferimento di tensione per l'alimentazione.

### Utilizzi
Gli op-amp sono blocchi costruttivi versatili utilizzati in moltissimi circuiti elettronici, tra cui:
- **Amplificatori**: Per aumentare l'ampiezza dei segnali
- **Filtri**: Per selezionare o eliminare specifiche gamme di frequenze
- **Comparatori**: Per confrontare due tensioni
- **Oscillatori**: Per generare segnali periodici
- **Circuiti di condizionamento del segnale**: Per modificare segnali in varie forme




---
### Riferimenti
[Amplificatore operazionale non-invertente](Amplificatore%20operazionale%20non-invertente.md)