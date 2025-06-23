---
lastSync: Mon Jun 16 2025 12:37:45 GMT+0200 (Ora legale dell’Europa centrale)
---
I **margini di fase (PM)** e di **guadagno (GM)** sono due delle metriche più importanti per valutare la **stabilità relativa** e la **robustezza** di un sistema di controllo a retroazione. Non ci dicono solo _se_ un sistema è stabile, ma _quanto_ lo è. Ci indicano quanto guadagno o fase possiamo aggiungere al loop ad anello aperto prima che il sistema a catena chiusa diventi instabile.

Questi margini vengono determinati direttamente dai **Diagrammi di Bode** della funzione di trasferimento ad anello aperto L(jω), quelli che abbiamo visto essere composti dal diagramma dei moduli e dal diagramma delle fasi.

#### 1. Margine di Fase (PM - Phase Margin)

Il **Margine di Fase** è la quantità di fase (in gradi) che può essere aggiunta alla frequenza di taglio del guadagno (ωc​) prima che il sistema diventi instabile.
- **Dove si legge:** Si legge sul **diagramma delle fasi** alla frequenza in cui il **modulo** è 0 dB (ωc​).
    
- **Calcolo:** PM=180∘+∠L(jωc​) Dove ∠L(jωc​) è la fase di L(jω) alla frequenza ωc​.
    
- **Interpretazione:**
    
    - Un PM>0∘ indica un sistema **stabile**.
    - Un PM=0∘ indica un sistema al limite della stabilità (oscillazioni continue).
    - Un PM<0∘ indica un sistema **instabile**.
    
    Tipicamente, un buon sistema di controllo dovrebbe avere un margine di fase tra 30∘ e 60∘. Un PM troppo piccolo significa che il sistema è vicino all'instabilità e potrebbe presentare sovraelongazioni elevate e oscillazioni smorzate lentamente. Un PM troppo grande può indicare un sistema pigro o troppo smorzato.
    

**Analogia:** Immagina di guidare una macchina. La fase è la direzione del tuo volante. Se il margine di fase è piccolo, significa che ti basta girare di poco il volante per perdere il controllo. Se è grande, hai un buon "gioco" prima che le cose si mettano male.

---

#### 2. Margine di Guadagno (GM - Gain Margin)

Il **Margine di Guadagno** è la quantità di guadagno (in dB) che può essere aggiunta alla frequenza di taglio della fase (ωp​) prima che il sistema diventi instabile.

- **Dove si legge:** Si legge sul **diagramma dei moduli** alla frequenza in cui la **fase** è −180∘ (ωp​).
    
- **Calcolo:** GM=−20log10​∣L(jωp​)∣ dB Dove ∣L(jωp​)∣ è il modulo di L(jω) alla frequenza ωp​. Nota il segno meno: se il modulo a ωp​ è ad esempio 0.5 (che è -6 dB), il GM sarà +6 dB.
    
- **Interpretazione:**
    
    - Un GM>0 dB indica un sistema **stabile**.
    - Un GM=0 dB indica un sistema al limite della stabilità.
    - Un GM<0 dB indica un sistema **instabile**.
    
    Un GM tipico desiderabile è tra 6 dB e 12 dB. Un GM troppo piccolo significa che piccole variazioni nel guadagno del loop possono rendere il sistema instabile.
    

**Analogia:** Se il margine di guadagno è piccolo, è come se la tua auto avesse un acceleratore troppo sensibile: una piccola pressione in più ti porterebbe subito fuori strada. Se è grande, hai un buon controllo sull'accelerazione.

---

#### Dimensionamenti (Cosa significano per il Progetto)

Nel progetto di un sistema di controllo, i margini di fase e di guadagno non sono solo indicatori di stabilità, ma anche di **prestazioni desiderate**.

- Un **PM più elevato** tende a tradursi in una **risposta transitoria meno oscillatoria** (meno sovraelongazione) e un migliore smorzamento, ma potrebbe rendere il sistema più lento.
- Un **GM più elevato** indica una maggiore **robustezza alle variazioni di guadagno** nel loop.

Il compito dell'ingegnere è spesso quello di progettare il controllore C(s) in modo da raggiungere i requisiti di prestazione (come tempo di salita, sovraelongazione, errore a regime) pur garantendo margini di fase e di guadagno adeguati per la robustezza.

In pratica, i margini di fase e di guadagno ci danno un'idea immediata e grafica di quanto il nostro sistema sia ben "tarato" e quanto "resista" a incertezze o disturbi prima di impazzire.