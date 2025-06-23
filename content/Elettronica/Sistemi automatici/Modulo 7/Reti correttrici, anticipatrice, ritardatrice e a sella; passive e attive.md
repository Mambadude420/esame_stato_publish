---
lastSync: Tue Jun 17 2025 20:28:52 GMT+0200 (Ora legale dell’Europa centrale)
---
### Reti Correttrici: Anticipatrice, Ritardatrice e a Sella; Passive e Attive
Oltre ai controllori PID, esistono altre tipologie di compensatori o "reti correttrici" che vengono usate per modellare e migliorare la risposta in frequenza di un sistema di controllo. Queste reti sono fondamentalmente filtri che alterano il guadagno e la fase della funzione di trasferimento ad anello aperto L(s) in specifiche bande di frequenza per raggiungere gli obiettivi di progetto (stabilità, velocità, precisione).

Le reti correttrici possono essere implementate in due modi principali:
1. **Passive:** Realizzate con componenti passivi (resistenze, condensatori, induttori). Non richiedono alimentazione esterna. Sono semplici, robuste ed economiche, ma possono introdurre un'attenuazione (riduzione di guadagno) e non possono fornire guadagno.
2. **Attive:** Realizzate con componenti attivi (amplificatori operazionali) oltre ai passivi. Richiedono alimentazione esterna. Possono fornire guadagno e maggiore flessibilità di progetto, ma sono più complesse e potenzialmente sensibili al rumore e alla non linearità dell'amplificatore.

Le tipologie principali di reti correttrici sono:
#### 1. Rete Correttrice Anticipatrice (Lead Compensator)
- **Scopo:** Migliorare la **risposta transitoria** e la **stabilità** (aumentare il margine di fase).
- **Funzionamento:** Una rete anticipatrice introduce uno **zero e un polo** nella funzione di trasferimento L(s), dove lo zero si trova a una frequenza inferiore rispetto al polo. In questo modo, la rete fornisce un **anticipo di fase** (contributo positivo alla fase) a determinate frequenze, tipicamente attorno alla frequenza di taglio del guadagno del sistema non compensato.
- **Impatto sui Diagrammi di Bode:**
    - **Modulo:** Aumenta leggermente il guadagno alle alte frequenze.
    - **Fase:** Introduce un picco positivo di fase (anticipo) a una certa frequenza, spostando la fase di L(s) verso valori più alti, aumentando il margine di fase.
- **Quando si usa:** Quando il sistema è instabile o marginalmente stabile e ha bisogno di un aumento del margine di fase, o quando si vuole migliorare la velocità di risposta e ridurre la sovraelongazione. È efficace nel compensare i ritardi di fase introdotti da altri componenti del sistema.

#### 2. Rete Correttrice Ritardatrice (Lag Compensator)
- **Scopo:** Migliorare l'**accuratezza a regime** (ridurre l'errore a regime) e, in minor misura, la stabilità.
- **Funzionamento:** Una rete ritardatrice introduce uno **zero e un polo**, dove lo zero si trova a una frequenza superiore rispetto al polo, e entrambi sono molto vicini all'origine. In questo modo, la rete fornisce un **ritardo di fase** (contributo negativo alla fase) ma un **guadagno elevato** a basse frequenze.
- **Impatto sui Diagrammi di Bode:**
    - **Modulo:** Fornisce un guadagno elevato alle basse frequenze (per ridurre l'errore a regime) e poi si attenua.
    - **Fase:** Introduce un ritardo di fase, ma questo ritardo viene posizionato a frequenze molto basse, ben al di sotto della frequenza di taglio del guadagno, in modo da minimizzare il suo impatto negativo sul margine di fase.
- **Quando si usa:** Quando il sistema ha un errore a regime inaccettabile (come un PID con solo P o PD) ma ha già margini di stabilità sufficienti. È come aggiungere un'azione integrale, ma con più controllo sulla sua influenza sulla fase.

#### 3. Rete Correttrice a Sella (Lead-Lag Compensator)
- **Scopo:** Ottenere contemporaneamente i benefici delle reti anticipatrici e ritardatrici.
- **Funzionamento:** Una rete a sella combina le caratteristiche di una rete anticipatrice e di una ritardatrice, introducendo **due zeri e due poli**. Tipicamente, il polo e lo zero del ritardo sono a basse frequenze (vicini all'origine), mentre il polo e lo zero dell'anticipo sono a frequenze più alte.
- **Impatto sui Diagrammi di Bode:** Il suo diagramma di Bode è una combinazione delle due reti precedenti. Avrà un aumento del guadagno alle basse frequenze e un anticipo di fase alle frequenze intermedie.
- **Quando si usa:** Quando si vogliono migliorare sia le prestazioni a regime (riduzione dell'errore) che quelle transitorie (velocità e smorzamento), e il sistema originale non permette di raggiungere entrambi gli obiettivi con una singola rete o un PID semplice.