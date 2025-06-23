---
lastSync: Mon Jun 16 2025 12:35:31 GMT+0200 (Ora legale dell’Europa centrale)
---
I criteri di stabilità di Bode sono delle regole empiriche (metodi sperimentali) che permettono di **valutare la stabilità relativa di un sistema ad anello chiuso** analizzando i diagrammi di Bode ad anello aperto. Questi criteri sono generalmente applicabili a sistemi a fase minima (sistemi in cui tutti i poli e gli zeri si trovano nel semipiano sinistro del piano $s$).

L'idea fondamentale è che la stabilità di un sistema ad anello chiuso è legata a quanto il guadagno dell'anello si riduce (o si attenua) prima che lo sfasamento totale raggiunga $180^\circ$. Se il guadagno è ancora maggiore di 1 (o 0 dB) quando la fase raggiunge $180^\circ$, c'è il rischio di instabilità o di oscillazioni.

Le due metriche chiave del criterio di Bode sono:
1. **Margine di Guadagno (Gain Margin - GM)**
2. **Margine di Fase (Phase Margin - PM)**

## Margine di Guadagno
Il margine di guadagno indica di quanto il guadagno ad anello aperto può essere aumentato alla frequenza, in cui la fase è $180^\circ$, prima che il sistema ad anello chiuso diventi instabile.
- **Frequenza di attraversamento della fase** ($\omega_{pg}$ - **Phase Crossover Frequency**): È la frequenza alla quale l'angolo di fase della funzione di trasferimento ad anello aperto $G(j \omega) H(j \omega)$ è esattamente $180^\circ$.
$$
\angle G(j \omega_{pg}) H(j \omega_{pg}) = -180^\circ
$$
- **Calcolo del Margine di Guadagno**:
$$
GM = -20 \log_{10} |G(j \omega_{pg}) H(j \omega_{pg})| = dB
$$
- Interpretazione:
	- $GM > 0^\circ \ dB$: Il sistema è stabile, Un GM elevato indica una buona stabilità rispetto a variazioni di guadagno.
	- $GM = 0^\circ \ dB$: Il sistema è al limite della stabilità (oscillatore continuo).
	- $GM < 0^\circ dB$: Il sistema è instabile.
	Un GM tipico desiderabile è tra 6 dB e 12 dB. Un GM troppo piccolo significa che piccole variazioni nel guadagno del loop possono rendere il sistema instabile.

## Margine di Fase (PM)
Il margine di fase indica di quanto l'angolo di fase ad anello aperto alla frequenza, in cui il guadagno è unitario (0 dB), è maggiore di $-180^\circ$.
- **Frequenza di attraversamento del guadagno** ($\omega_{gc}$ - **Gain Crossover Frequency**). È la frequenza alla quale il modulo (guadagno) della funzione di trasferimento ad anello aperto $G(j \omega) H(j \omega)$ è 1 (o 0 dB).
$$
| G(j \omega_{gc}) H(j \omega_{gc}) | = 1 \ \ o \ \ 20\log_{10} | G(j \omega_{gc}) H(j \omega_{gc}) | = 0 \ dB
$$
- **Calcolo del Margine di Fase:**
$$
PM = 180^\circ + \angle G(j \omega_{gc}) H(j \omega_{gc})
$$
- Interpretazione:
	- $PM > 0^\circ$: Il sistema è stabile. Un PM più grande (tipicamente tra $30^\circ$ e $60^\circ$) è desiderabile per una buona stabilità relativa e una risposta transitoria ben smorzata (meno [overshoot](Overshoot.md)).
	- $PM = 0^\circ$: Il sistema è al limite della stabilità (oscillatore continuo).
	- $PM < 0^\circ$: Il sistema è instabile.

#### Perché sono importanti?
- Stabilità relativa: Non ci dicono solo se il sistema è stabile o meno, ma anche "quanto" è stabile. Un sistema con margini di stabilità sufficienti è robusto a piccole variazioni nei parametri e ai disturbi.
- Prestazioni della Risposta Transitoria: C'è una correlazione tra i margini di stabilità e la forma della risposta transitoria. Ad esempio, un PM  basso implica un overshoot elevato e oscillazioni.
- Progettazione dei Controllori: I margini di guadagno e fase sono obiettivi comuni nella progettazione dei controllori, che vengono modificati (ad esempio, con reti anticipatrici o ritardatrici) per ottenere i margini desiderati



## Riferimenti e collegamenti
### Precedente
[Diagrammi di Bode](Diagrammi%20di%20Bode.md)

### Successivo


### Riferimenti
[Tecniche di compensazione e reti correttrici](Tecniche%20di%20compensazione%20e%20reti%20correttrici.md)