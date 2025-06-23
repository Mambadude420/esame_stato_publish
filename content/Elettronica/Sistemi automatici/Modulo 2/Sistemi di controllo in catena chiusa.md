---
lastSync: Sun Jun 15 2025 16:45:11 GMT+0200 (Ora legale dell’Europa centrale)
---
### Sistemi di Controllo in Catena Chiusa: Definizioni e Caratterizzazione Statica e Dinamica

Mentre nei sistemi in catena aperta il controllo avveniva "alla cieca", i sistemi in catena chiusa introducono un concetto fondamentale: il **feedback** (o retroazione).

Immagina di voler mantenere la temperatura della tua stanza a 20°C. Con un sistema in catena aperta, accenderesti il riscaldamento per un certo tempo basandoti solo sulla tua esperienza. Con un sistema in **catena chiusa**, invece, hai un **sensore** (un termometro) che misura continuamente la temperatura attuale della stanza. Questa misura viene confrontata con la temperatura desiderata (i tuoi 20°C). Se c'è una differenza (un "errore"), il sistema agisce per correggerla, ad esempio accendendo o spegnendo la caldaia.

#### Definizioni Fondamentali
Un **sistema di controllo in catena chiusa** (o a **retroazione**) è un sistema in cui l'uscita desiderata viene continuamente confrontata con l'uscita attuale, e la differenza (l'errore) viene utilizzata per generare un'azione di controllo che riduca tale errore.

Ecco gli elementi chiave di un sistema a catena chiusa:
- **Valore di riferimento (o setpoint) $(R(s))$:** È il valore desiderato per la variabile di uscita (es. 20°C).
- **Variabile di uscita (o controllata) $(Y(s))$:** È il valore attuale misurato del processo (es. la temperatura attuale della stanza).
- **Sensore:** Un dispositivo che misura la variabile di uscita e la converte in un segnale che può essere utilizzato dal controllore.
- **Errore $(E(s))$:** La differenza tra il valore di riferimento e la variabile di uscita misurata $(E(s)=R(s)−Y(s)$ in retroazione unitaria negativa, o $E(s)=R(s)−H(s)Y(s)$ in generale). È il segnale che il controllore cerca di minimizzare.
- **Controllore $(C(s))$:** La "mente" del sistema. Riceve il segnale di errore e genera un segnale di comando per l'attuatore.
- **Attuatore:** Il dispositivo che agisce sul processo (es. una valvola che regola il flusso di gas alla caldaia).
- **Processo (o impianto) $(P(s))$:** L'oggetto fisico che stiamo controllando (es. la caldaia e la stanza).
- **Feedback (o retroazione):** Il percorso che riporta l'uscita misurata all'ingresso del controllore per il confronto.

Il grande vantaggio della retroazione è la sua capacità di **compensare i disturbi** e le incertezze del processo. Se una finestra si apre e la temperatura scende (un disturbo), il sistema rileva l'errore e accende il riscaldamento per compensare, cosa che un sistema in catena aperta non potrebbe fare.

#### Caratterizzazione Statica e Dinamica

Quando analizziamo un sistema di controllo in catena chiusa, ci interessano due aspetti principali del suo comportamento:

1. **Caratterizzazione Statica (o a Regime):** Riguarda il comportamento del sistema quando ha raggiunto uno stato di equilibrio, cioè dopo che tutte le fasi transitorie sono terminate e i segnali si sono stabilizzati. La domanda chiave qui è: "A quale valore si stabilizza l'uscita? C'è un errore a regime?"
   L'**errore a regime** è la differenza tra il valore di riferimento desiderato e il valore effettivo dell'uscita dopo che il sistema si è stabilizzato. Idealmente, vorremmo un errore a regime nullo, ma in pratica non è sempre così. Dipende molto dalla struttura del controllore e del processo.
2. **Caratterizzazione Dinamica (o Transitoria):** Riguarda il comportamento del sistema mentre si muove da uno stato iniziale a uno stato finale. La domanda qui è: "Come raggiunge il sistema il valore desiderato? Quanto velocemente? Oscilla? Va oltre il valore desiderato e poi torna indietro?"
   Questa analisi studia la **[[Risposta transitoria.md|risposta transitoria]]** del sistema, ovvero come l'uscita evolve nel tempo in risposta a un cambiamento dell'ingresso o a un disturbo. Parametri importanti che useremo per descrivere la risposta dinamica includono:
    - **Tempo di salita:** Quanto tempo impiega l'uscita per raggiungere una certa percentuale (spesso 90%) del suo valore finale.
    - **Sovra-elongazione:** Se l'uscita supera il valore desiderato prima di stabilizzarsi (un po' come un'auto che frena troppo tardi e oltrepassa il semaforo).
    - **Tempo di assestamento:** Il tempo necessario affinché l'uscita rimanga entro una piccola percentuale del suo valore finale. ^c9f103

Un buon sistema di controllo deve bilanciare sia la performance statica (errore a regime minimo) che quella dinamica (risposta rapida e ben smorzata, senza eccessive oscillazioni). È come un atleta che non solo deve arrivare al traguardo (stato statico), ma deve farlo nel modo più veloce e controllato possibile (stato dinamico).