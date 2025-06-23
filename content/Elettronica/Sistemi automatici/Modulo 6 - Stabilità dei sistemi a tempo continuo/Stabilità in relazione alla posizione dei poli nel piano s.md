---
lastSync: Sun Jun 15 2025 19:04:40 GMT+0200 (Ora legale dell’Europa centrale)
---
I **poli** di una FDT sono i valori di s che rendono il denominatore della FDT uguale a zero. Sono le "radici" del polinomio al denominatore.

La posizione di questi poli nel **piano complesso s** (che ha un asse reale e un asse immaginario) è il **criterio più diretto e fondamentale per determinare la stabilità di un sistema lineare e stazionario (LTI)**.

Immagina il piano s diviso a metà dall'asse immaginario (jω). Abbiamo:
- Il **semipiano sinistro** (parte reale negativa).
- Il **semipiano destro** (parte reale positiva).
- L'**asse immaginario** (parte reale nulla).

Il legame tra la posizione dei poli e la stabilità è il seguente:
1. **Poli nel Semipiano Sinistro (Parte Reale Negativa): STABILITÀ**
    - Se **tutti i poli** della Funzione di Trasferimento **ad anello chiuso** del sistema (cioè i poli di $G_{CL}​(s)$) hanno parte reale negativa, allora il sistema è **asintoticamente stabile**.
    - Questo significa che, se il sistema viene perturbato o se riceve un ingresso finito, la sua risposta transitoria si smorzerà nel tempo e l'uscita si stabilizzerà a un valore finito. Le oscillazioni (se presenti, come nei sistemi sottosmorzati) si estingueranno.
    - Più la parte reale dei poli è negativa, più velocemente la risposta transitoria si smorza (ricordi la costante di tempo $τ=1/∣Re(polo)∣$ ?).
2. **Poli nel Semipiano Destro (Parte Reale Positiva): INSTABILITÀ**
    - Se **almeno un polo** della FDT ad anello chiuso ha parte reale positiva, allora il sistema è **instabile**.
    - Questo significa che, anche per una piccola perturbazione o un ingresso limitato, la risposta del sistema crescerà esponenzialmente nel tempo, allontanandosi indefinitamente dal punto di equilibrio. Le oscillazioni, se presenti, avranno ampiezza crescente.
    - Un sistema instabile è inutilizzabile e potenzialmente pericoloso.
3. **Poli sull'Asse Immaginario (Parte Reale Nulla): STABILITÀ MARGINALE**
    - Se non ci sono poli nel semipiano destro, ma ci sono **poli semplici** (non ripetuti) sull'asse immaginario (es. in $s=±jω0$​), allora il sistema è **marginalmente stabile**.
    - Questo significa che, se il sistema viene perturbato, la sua risposta transitoria non si smorzerà, ma non crescerà nemmeno. Si verificheranno oscillazioni continue a una frequenza fissa (quella data da $ω_{0}$​).
    - Un esempio è un pendolo ideale senza attrito: se lo spingi, oscilla all'infinito. Dal punto di vista del controllo, la stabilità marginale è spesso indesiderabile, a meno che l'oscillazione sia il comportamento desiderato (es. un generatore di onde).
4. **Poli Ripetuti Sull'Asse Immaginario: INSTABILITÀ**
    - Se ci sono **poli ripetuti** (di molteplicità maggiore di 1) sull'asse immaginario (es. in $s=0$,0 o $s=±jω0​,±jω0$​), allora il sistema è **instabile**. Anche se la parte reale è zero, la ripetizione fa sì che la risposta cresca nel tempo (linearmente o come potenza del tempo).