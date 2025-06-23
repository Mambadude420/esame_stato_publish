---
lastSync: Sat Jun 14 2025 17:55:24 GMT+0200 (Ora legale dell’Europa centrale)
---
### Diagrammi di Nyquist: Proprietà e Tracciamento Qualitativo

I Diagrammi di Nyquist sono uno strumento grafico potentissimo nell'analisi dei sistemi di controllo. Sono come una mappa che ci permette di "vedere" la **stabilità** di un sistema in catena chiusa semplicemente analizzando la sua funzione di trasferimento ad anello aperto.

L'idea alla base è che, invece di guardare solo i poli della funzione di trasferimento ad anello chiuso (che a volte sono difficili da trovare), possiamo analizzare il comportamento della **funzione di trasferimento ad anello aperto L(s) nel dominio della frequenza**.

Un **Diagramma di Nyquist** è, in pratica, la rappresentazione grafica del luogo dei punti L(jω) nel piano complesso, al variare della frequenza ω da 0 a ∞. Metti un attimo da parte la s e pensa a jω. Stiamo sostituendo s con jω nella funzione di trasferimento L(s). Questo perché jω rappresenta le frequenze pure, e ci permette di vedere come il sistema risponde ai segnali sinusoidali.

#### Proprietà Fondamentali

Le proprietà principali che rendono i diagrammi di Nyquist così utili sono:

1. **Stabilità del sistema a ciclo chiuso (Criterio di Nyquist):** Questa è la ragione principale per cui li usiamo! Il Criterio di Nyquist ci permette di determinare la stabilità di un sistema a catena chiusa basandosi sul numero di avvolgimenti che il percorso di Nyquist di L(s) compie attorno al punto critico **(-1, j0)** del piano complesso. Se il sistema ad anello aperto è stabile, e il punto (-1, j0) non viene racchiuso dalla curva, allora il sistema a catena chiusa è stabile. Se ci sono poli instabili ad anello aperto, il criterio diventa un po' più sofisticato, ma l'idea è la stessa. È come se il punto (-1, j0) fosse una "buccia di banana" e il sistema è stabile se la curva riesce a evitarla o ad aggirarla in un certo modo.
2. **Informazioni su guadagno e fase:** Ogni punto sul diagramma rappresenta il modulo (o guadagno) e la fase di L(jω) per una specifica frequenza ω.
	- La **distanza dall'origine** al punto sul diagramma è il **guadagno** di L(jω) a quella frequenza.
	- L'**angolo** che il vettore dall'origine al punto forma con l'asse reale positivo è lo **sfasamento** (fase) di L(jω) a quella frequenza.
3. **Misure di robustezza (Margini di fase e di guadagno):** Dal diagramma di Nyquist possiamo facilmente ricavare i **margini di fase e di guadagno**, che sono indicatori di quanto un sistema sia "robusto" alla variazione dei suoi parametri prima di diventare instabile. Sono come delle "distanze di sicurezza" dal punto critico (-1, j0).