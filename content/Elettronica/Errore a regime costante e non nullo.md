---
lastSync: Thu May 15 2025 12:52:07 GMT+0200 (Ora legale dell’Europa centrale)
---
Quando un sistema viene sottoposto a un ingresso di riferimento (ad esempio, un [gradino](Ingresso%20a%20gradino%20(Step%20input).md) per raggiungere una nuova posizione o velocità costante), idealmente vorremmo che l'uscita del sistema raggiungesse esattamente il valore desiderato e vi rimanesse, con un errore di zero.

Tuttavia, in molto sistemi reali, dopo che la fase transitoria si è esaurita, potrebbe rimanere una differenza costante tra il segnale di riferimento e l'uscita effettiva del sistema.
Questa differenza costante è ciò che chiamiamo **errore a regime costante nullo**.

### Significato dei termini:
- **Errore a regime**: si riferisce all'errore (la differenza tra il riferimento e uscita) quando il tempo tende all'infinito, cioè quando il sistema ha raggiunto il suo stato stazionario. ^76f787
- **Costante**: significa che il valore dell'erorre non cambia nel tempo una volta raggiunto il regime permanente. Non oscilla e non tende a zero o all'infinito.
- **Non nullo**: indica che il valore di questo errore costante è diverso da 0. C'è una discrepanza persistente tra ciò che vogliamo e ciò che otteniamo.

### Motivi della verifica di un errore a regime constante e non nullo
- **Guadagno finito del sistema**: Sistemi di Tipo 0 tendono ad avere un errore a regime costante per [ingressi a gradino](Ingresso%20a%20gradino%20(Step%20input).md) proprio a causa del loro guadagno statico finito.
- **Disturbi costanti**: Se c'è un disturbo costante che agisce sul sistema, il sistema potrebbe stabilizzarsi con un errore per compensare questo disturbo.
- **Non idealità dei componenti**: Componenti reali come motori e attuatori potrebbero avere delle non linearità o delle offset che contribuiscono a un errore a regime.