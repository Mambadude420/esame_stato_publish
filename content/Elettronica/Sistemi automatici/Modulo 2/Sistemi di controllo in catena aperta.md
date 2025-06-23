---
lastSync: Sat Jun 14 2025 17:16:06 GMT+0200 (Ora legale dell’Europa centrale)
---
# Sistemi di controllo in catena aperta, on/off, feed-forward, a microprocessore
#### Sistemi di Controllo in Catena Aperta (Open-Loop Control)

Immagina di cuocere una torta usando una ricetta: segui le istruzioni (ingredienti, tempi di cottura, temperatura del forno) senza assaggiare il composto o controllare se la torta è effettivamente cotta. Questo è un sistema in **catena aperta**.

In un sistema di controllo in catena aperta, l'**uscita del sistema non viene misurata e non viene utilizzata per influenzare l'ingresso**. L'azione di controllo dipende solo dal segnale di ingresso e da una calibrazione predefinita.

**Esempi:**

- **Tostapane:** Imposti il tempo e il tostapane scalda per quel periodo, indipendentemente dal fatto che il pane sia troppo o troppo poco tostato.
- **Lavatrice (ciclo fisso):** Selezioni un programma e la lavatrice esegue una sequenza di operazioni predefinite (riempimento, lavaggio, risciacquo, centrifuga) senza "sapere" quanto sono sporchi i vestiti.

**Vantaggi:** Sono semplici da progettare e costruire, e solitamente meno costosi.
**Svantaggi:** Sono poco precisi perché non compensano i disturbi esterni (come una variazione di tensione nel tostapane) o le variazioni nelle caratteristiche del processo. Se il pane è congelato, il tostapane non se ne accorge!

#### Sistemi di Controllo On/Off (Bang-Bang Control)

Questo è un tipo di controllo semplice ma molto comune. Pensa a un termostato domestico molto basilare: quando la temperatura scende sotto un certo valore, accende la caldaia. Quando sale oltre un altro valore, la spegne. **Il controllore ha solo due stati possibili: acceso o spento.**

**Esempi:**

- **Termostato domestico:** Accende o spegne il riscaldamento.
- **Frigorifero:** Accende o spegne il compressore per mantenere la temperatura.

**Vantaggi:** Molto semplici ed economici da implementare.
**Svantaggi:** L'uscita del processo tende a oscillare intorno al valore desiderato (questo fenomeno è chiamato "overshoot" e "undershoot" o isteresi), e il componente di controllo (ad esempio la caldaia) viene stressato da continue accensioni e spegnimenti.

#### Sistemi di Controllo Feed-Forward

Questo tipo di controllo cerca di agire prima che il problema si manifesti. Invece di aspettare che un disturbo influenzi l'uscita per correggerlo, il controllo **feed-forward misura il disturbo stesso e agisce sull'ingresso per compensarlo preventivamente**. È come un allenatore di calcio che studia le tattiche dell'avversario prima della partita per impostare la propria strategia, invece di aspettare che l'avversario segni un gol per reagire.

**Esempio:**

- **Sistema di riscaldamento con feed-forward:** Oltre a un termostato normale, potresti avere un sensore che misura la temperatura esterna. Se la temperatura esterna cala bruscamente, il sistema feed-forward potrebbe aumentare preventivamente l'emissione di calore, prima ancora che la temperatura interna della casa scenda significativamente.

**Vantaggi:** Può migliorare le prestazioni del sistema riducendo l'impatto dei disturbi prima che influenzino l'uscita.
**Svantaggi:** Richiede una buona conoscenza del processo e del disturbo, e la misurazione del disturbo deve essere precisa. Non può correggere disturbi imprevisti o errori di modellazione.

#### Sistemi di Controllo a Microprocessore

Questi sono i sistemi di controllo moderni e più flessibili. In questi sistemi, un **microprocessore o un microcontrollore** (spesso un piccolo computer embedded) esegue il software di controllo. Il microprocessore può implementare logiche di controllo molto complesse, elaborare dati da sensori e pilotare attuatori.

**Esempi:**

- **Cruise control dell'auto:** Un microprocessore legge la velocità e l'accelerazione, e regola l'apertura della farfalla del motore per mantenere la velocità impostata.
- **Sistemi di automazione industriale:** Quasi tutti i controlli complessi nelle fabbriche (robot, linee di produzione) sono gestiti da microprocessori/microcontrollori (spesso tramite PLC - Controllori Logici Programmabili).

**Vantaggi:** Grande flessibilità (si cambia il software, non l'hardware), alta precisione, possibilità di implementare algoritmi di controllo complessi e funzionalità avanzate (diagnostica, comunicazione).
**Svantaggi:** Richiede competenze di programmazione e hardware, e può essere più costoso e complesso per applicazioni molto semplici.


## Riferimenti e collegamenti
### Precedente


### Successivo
[[Sistemi di controllo in catena chiusa.md]]

### Riferimenti
