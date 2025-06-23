---
lastSync: Tue Jun 17 2025 19:53:31 GMT+0200 (Ora legale dell’Europa centrale)
---
Il controllore PID è un algoritmo che calcola il segnale di controllo da applicare a un processo basandosi sull'erorre tra il valore desiderato (riferimento) e il valore misurato (uscita). L'azione di controllo u(t) è la somma di tre termini: proporzionale, integrale e derivativo.

#### 1. Azione Proporzionale (P)
- **Come funziona:** L'azione di controllo è **direttamente proporzionale all'errore attuale**. Se l'errore è grande, l'azione correttiva è grande; se l'errore è piccolo, la correzione è piccola. È come quando acceleri un'auto: più sei lontano dalla velocità desiderata, più premi sull'acceleratore.
- **Impatto sul Transitorio:**
    - **Velocità:** Aumentare $Kp$​ rende il sistema più **veloce** e reattivo. Risponde più rapidamente ai cambiamenti.
    - **Stabilità:** Aumentare troppo $Kp$​ può portare a **oscillazioni** e, se eccessivo, può rendere il sistema **instabile**. È come premere troppo sull'acceleratore, l'auto sbanda.
    - **Sovraelongazione:** Spesso aumenta la **sovraelongazione** ([[overshoot.md|overshoot]]).
- **Impatto a Regime:**
    - **Errore a regime:** L'azione P, da sola, genera quasi sempre un **errore a regime costante e non nullo** (un "offset"). Questo significa che l'uscita non raggiungerà mai _esattamente_ il valore desiderato, ma si stabilizzerà con una piccola differenza. È come provare a centrare perfettamente un bersaglio: ti avvicini molto, ma non sei mai esattamente al centro.

#### 2. Azione Integrale (I)
- **Come funziona:** L'azione di controllo è proporzionale all'**integrale dell'errore nel tempo**. Ciò significa che "accumula" l'errore passato. Se c'è un errore persistente, anche se piccolo, l'azione integrale continuerà a crescere fino a quando l'errore non si annulla. È come tenere il piede sull'acceleratore finché non raggiungi la velocità esatta.
- **Impatto sul Transitorio:**
    - **Velocità:** Tende a rendere il sistema più **lento** nel rispondere.
    - **Stabilità:** Può **ridurre la stabilità** e aumentare le oscillazioni, perché introduce un ritardo e un "momentum" (accumulo) nell'azione di controllo.
    - **Sovraelongazione:** Spesso aumenta la **sovraelongazione**.
- **Impatto a Regime:**
    - **Errore a regime:** Il suo vantaggio principale è che **elimina l'errore a regime** per ingressi a gradino. Finché c'è un errore, anche minimo, l'integratore continua a lavorare per annullarlo. Questo è il suo superpotere!

#### 3. Azione Derivativa (D)
- **Come funziona:** L'azione di controllo è proporzionale alla **velocità di variazione dell'errore** (la sua derivata). Agisce in modo predittivo: se l'errore sta cambiando rapidamente (ad esempio, sta aumentando o diminuendo velocemente), l'azione derivativa applica una correzione maggiore per contrastare o anticipare il cambiamento. È come frenare in anticipo se vedi un ostacolo avvicinarsi velocemente.
- **Impatto sul Transitorio:**
    - **Velocità:** Aumenta la **velocità di risposta** del sistema.
    - **Stabilità:** Migliora la **stabilità** e lo smorzamento del sistema, riducendo le oscillazioni.
    - **Sovraelongazione:** Rende la risposta più "liscia" e **riduce la sovraelongazione**.
    - **Problemi con il rumore:** È molto sensibile al **rumore di misura** (derivando un segnale rumoroso si ottengono picchi molto grandi) e per questo è spesso usato con un filtro.
- **Impatto a Regime:**
    - **Errore a regime:** Non ha alcun impatto sull'errore a regime per ingressi costanti, poiché la derivata di un errore costante è zero. Il suo effetto si manifesta solo durante la fase di transitorio.