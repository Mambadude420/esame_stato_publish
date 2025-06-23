---
lastSync: Thu May 29 2025 21:37:03 GMT+0200 (Ora legale dell’Europa centrale)
---
# Mappa Concettuale degli Argomenti

1.  **Protezione degli Impianti Elettrici**
    * **Cortocircuito**
        * **Definizione e cause:** Si verifica quando l'impedenza complessiva di un circuito diminuisce drasticamente, portando a un aumento anomalo e pericoloso delle correnti circolanti. Questo può essere causato da un contatto diretto tra conduttori di fase, o tra fase e neutro/terra, spesso a causa di un isolamento difettoso o un guasto meccanico. Il caso più critico per il calcolo è il cortocircuito franco simmetrico trifase.
        * **Mezzi di protezione:**
            * **Interruttori automatici:** Dispositivi in grado di interrompere la corrente in caso di guasto. Il loro costo è direttamente proporzionale alla massima corrente di guasto che possono interrompere (potere di rottura).
            * **Valvole fusibili:** Componenti più economici che interrompono il circuito fondendo un elemento conduttivo quando la corrente supera un certo valore per un tempo definito. Richiedono la sostituzione dopo ogni intervento.
        * **Calcolo della corrente di cortocircuito:** Essenziale per dimensionare correttamente i dispositivi di protezione, viene effettuato nei punti strategici dell'impianto dove sono collocati gli interruttori.
    * **Sovraccarico**
        * **Definizione e effetti (temperatures):** Si verifica quando una corrente, pur non essendo un cortocircuito, supera il valore nominale per un periodo prolungato, causando un innalzamento della temperatura nei cavi e nei componenti.
        * **Temperature di riferimento:**
            * **T di cortocircuito:** La temperatura si innalza così rapidamente da richiedere un'interruzione entro pochi secondi (180-250°C).
            * **T di sovraccarico:** Temperatura che determina un rapido deterioramento dell'isolante se mantenuta per tempi dell'ordine delle ore (110-150°C).
            * **T di regime permanente:** La temperatura massima che il conduttore può sopportare indefinitamente senza danni (70-90°C).
    * **Interruttori**
        * **Tipi:**
            * **Termici:** Basati su regoli bimetallici che si deformano con il riscaldamento dovuto a correnti superiori alla nominale, provocando lo sgancio. Proteggono dai sovraccarichi.
            * **Magnetici:** Utilizzano bobine che, in presenza di correnti elevate (tipiche dei cortocircuiti), generano un campo magnetico sufficiente a sganciare l'interruttore. Il loro campo di intervento può essere fisso o regolabile.
            * **Magnetotermici:** Integrano entrambe le protezioni (termica per sovraccarichi e magnetica per cortocircuiti) in un unico dispositivo, offrendo una protezione completa per cavi e macchine.
        * **Caratteristiche principali:**
            * **Tensione nominale:** La tensione per cui l'interruttore è progettato.
            * **Corrente nominale (In):** Il valore di corrente che i contatti possono sopportare indefinitamente.
            * **Potere di rottura (Icn):** Il massimo valore di corrente di guasto che l'interruttore è in grado di interrompere in sicurezza. Questo valore è cruciale per garantire che l'interruttore non si danneggi irrimediabilmente e possa proteggere l'impianto anche in condizioni estreme.
            * **Tempo totale di apertura:** Il tempo che intercorre tra l'inizio del guasto e l'interruzione completa della corrente.
        * **Caratteristiche d'intervento (curve):** Descrivono il comportamento dell'interruttore in funzione della corrente e del tempo (In, Inf, If, Im1, Im2).
        * **Scelta dell'interruttore (regole e criteri):**
            * Installazione a meno di 3 metri dalla conduttura protetta.
            * Corrente nominale (In) non inferiore alla massima corrente di funzionamento (IB).
            * Potere di rottura (Icn) maggiore della corrente presunta di cortocircuito (Icc).
            * L'interruttore deve garantire l'intervento per qualsiasi guasto nella linea protetta.
    * **Coordinamento delle Protezioni**
        * **Protezione in cascata:** Gli interruttori sono disposti in serie, e quello più a monte (A) interviene prima, garantendo una selettività minima e una continuità di funzionamento ridotta.
        * **Protezione selettiva:** Garantisce la massima continuità di funzionamento, minimizzando l'interruzione del servizio solo alla sezione interessata dal guasto. Solo l'interruttore più vicino al punto di guasto interviene (es. sequenza D, C, B, A). Richiede curve di intervento senza punti in comune e una capacità di rottura di ogni interruttore superiore alla Icc a valle. Si limita a massimo 3 o 4 interruttori per evitare tempi di intervento eccessivi.

2.  **Pericolosità della Corrente Elettrica e Protezioni per le Persone**
    * **Effetti dell'Elettrocuzione:** I danni dipendono dal valore e dalla durata della corrente che attraversa il corpo umano.
        * **Tetanizzazione:** Contrazione muscolare involontaria che impedisce al soggetto di staccarsi dalla parte in tensione.
        * **Arresto respiratorio:** Per correnti più elevate, i muscoli respiratori possono bloccarsi.
        * **Fibrillazione ventricolare:** Alterazione del ritmo cardiaco che può portare all'arresto del cuore, essendo il cuore stesso stimolato elettricamente.
        * **Ustioni:** Il passaggio di corrente elettrica, per effetto Joule, riscalda i tessuti attraversati.
    * **Resistenza del Corpo Umano:** Il valore della corrente dipende anche dalla resistenza che il corpo oppone.
        * **Fattori che la influenzano:** Diminuisce con pelle umida o ferite, aumentando con la pressione e la superficie di contatto. Aumenta in presenza di zone callose.
        * **Tensione di soglia (50 Volt):** Limite di tensione per non avere un passaggio di corrente eccessiva, basato su una resistenza media del corpo umano. Questo valore è un riferimento fondamentale per la progettazione sicura degli impianti e la classificazione degli ambienti.
    * **Zone di Pericolosità (Curva Corrente-Tempo):** Studi di elettrofisiologia definiscono confini probabilistici tra le zone di pericolosità.
        * **Zona 1 (sotto 0.5 mA):** Corrente non percepita.
        * **Zona 2:** Corrente percepita senza effetti dannosi.
        * **Zona 3:** Possibili tetanizzazione, disturbi reversibili al cuore, aumento pressione sanguigna, difficoltà respiratoria.
        * **Zona 4:** Fibrillazione ventricolare e ustioni. Il valore asintotico di corrente sopportabile (circa 30 mA) è raggiunto con tempi di esposizione di 5 secondi. La curva è valida per il percorso "mano-piedi".
    * **Contatti Elettrici:**
        * **Contatto diretto:** Tocco di una parte dell'impianto normalmente in tensione (es. conduttore di un cavo, attacco di una lampadina).
        * **Contatto indiretto:** Tocco di una massa metallica che è andata in tensione a causa di un cedimento dell'isolamento principale (es. scocca di un elettrodomestico).
    * **Sistemi di Protezione:**
        * **Interruttore Differenziale:** Rileva la differenza tra la corrente di fase e quella di neutro. Se le correnti non sono uguali, significa che una parte sta disperdendo (es. attraverso il corpo umano o verso terra), attivando la protezione. È essenziale per la protezione dai contatti diretti e indiretti. I suoi componenti includono un trasformatore toroidale che rileva lo squilibrio.
        * **Impianto di Terra:** Insieme di dispersori e conduttori che collegano le masse metalliche degli impianti e degli utilizzatori al terreno. Ha lo scopo fondamentale di proteggere le persone dai contatti indiretti, garantendo che in caso di guasto a terra, la corrente di dispersione venga convogliata verso terra, facendo intervenire l'interruttore differenziale.

3.  **Sicurezza sul Lavoro e Gestione Rifiuti (DL 81/2008 & RAEE)**
    * **DL 81/2008 (Testo Unico sulla Sicurezza sul Lavoro):** Decreto legislativo che disciplina in Italia i presidi e le prescrizioni per la salute e sicurezza in ogni tipologia di attività lavorativa. Il suo approccio è volto a far percepire il concetto di rischio al lavoratore, definito empiricamente come $R = P \ \times D$ (Rischio = Probabilità di un evento dannoso x Entità del danno).
    * **Normativa CEI 64-8:** Redatta dal Comitato Elettrotecnico Italiano, è una normativa fondamentale per gli impianti elettrici in bassa e media tensione. Disciplina concetti tecnici come la tensione di contatto massima ammissibile (50 V), i contatti diretti e indiretti, e fornisce linee guida per il dimensionamento di un impianto elettrico (rilievo potenze, determinazione potenze assorbite, stima potenza richiesta, scelta distribuzione, dimensionamento cavi).
    * **Forniture Elettriche:**
        * **BT (Bassa Tensione):** 220V/380V, per potenze inferiori a 150KW.
        * **MT (Media Tensione):** 3KV fino a 20KV, per potenze superiori a 150KW fino a MW.
        * **AT (Alta Tensione):** 60KV, 120KV e oltre, per potenze molto elevate (>>MW), con normative specifiche di settore industriale.
    * **RAEE (Rifiuti di Apparecchiature Elettriche ed Elettroniche):**
        * **Problematica:** I RAEE rappresentano un problema ambientale significativo e in continua crescita, a causa della presenza di sostanze inquinanti (es. diossina, metalli pesanti che possono contaminare le falde acquifere) e per l'impatto energetico legato al loro smaltimento in discarica. Si stima una produzione di circa 15 kg/anno per abitante.
        * **Normative e gestione:** Lo standard europeo ha introdotto normative specifiche per produttori e rivenditori. In Italia, la gestione è stata sistematizzata dal 2011 tramite una logistica capillare di raccolta, il recupero dei materiali riutilizzabili (soprattutto metalli preziosi) e la neutralizzazione delle sostanze tossiche. Il trattamento include messa in sicurezza, bonifica, smontaggio e separazione preliminare dei materiali.
        * **Soggetti obbligati:** Produttori che fabbricano/vendono con proprio marchio, rivendono con proprio marchio apparecchiature altrui, o importano/immettono per primi nel mercato nazionale.
        * **Classificazione:** Grandi e piccoli elettrodomestici, apparecchiature informatiche e di telecomunicazione, illuminazione, strumentazione elettrica/elettronica, giocattoli, distributori automatici. Non sono RAEE: auto/moto, installazioni fisse, impiantistica elettrica.
        * **Marcatura e Direttiva RoHS:** I prodotti introdotti nel mercato italiano devono avere la marcatura RAEE. Dal 2006, la direttiva RoHS (Restriction of Hazardous Substances) è obbligatoria per i prodotti in UE, regolamentando l'impiego di 5 materiali primari critici: Piombo, Mercurio, Cadmio, Cromo esavalente, Bifenili polibromurati.

4.  **Grado di Protezione IP**
    * **Codice IP:** È un sistema di classificazione standardizzato (CEI 70-1) che indica il livello di protezione fornito da un involucro di un'apparecchiatura elettrica. Descrive la protezione contro l'accesso a parti pericolose, la penetrazione di corpi estranei solidi e l'ingresso di acqua.
    * **Componenti:** Il codice è composto da due cifre numeriche e una lettera addizionale opzionale.
    * **1ª Cifra (Protezione Solidi/Persone):** Indica il grado di protezione dell'apparecchiatura contro la penetrazione di corpi solidi estranei e la protezione delle persone contro l'accesso a parti pericolose. La scala va da 0 (non protetto) a 6 (totalmente protetto contro la polvere e l'accesso con un filo).
        * **Esempi di protezione:**
            * IP1x: Protetto contro corpi solidi > 50 mm (es. dorso della mano). Tipico per involucri che proteggono da contatti accidentali di grandi oggetti.
            * IP2x: Protetto contro corpi solidi > 12 mm (es. un dito).
            * IP3x: Protetto contro corpi solidi > 2.5 mm (es. un attrezzo).
            * IP4x: Protetto contro corpi solidi > 1 mm (es. un filo).
            * IP5x: Protetto contro la polvere e l'accesso con un filo.
            * IP6x: Totalmente protetto contro la polvere e l'accesso con un filo.
    * **2ª Cifra (Protezione Liquidi):** Indica il grado di protezione dell'apparecchiatura contro la penetrazione di acqua con effetti dannosi. La scala va da 0 (non protetto) a 8 (protetto contro gli effetti della sommersione continua).
        * **Esempi di protezione:**
            * IPx1: Protetto contro la caduta verticale di gocce d'acqua.
            * IPx3: Protetto contro la pioggia (spruzzi d'acqua fino a 60° dalla verticale).
            * IPx5: Protetto contro i getti d'acqua.
            * IPx7: Protetto contro gli effetti dell'immersione temporanea (es. 30 minuti a 1 metro di profondità).
            * IPx8: Protetto contro gli effetti della sommersione continua (condizioni specificate dal produttore).
    * **Lettera Addizionale (Opzionale):** Utilizzata se la protezione effettiva contro l'accesso a parti pericolose è superiore a quella indicata dalla prima cifra, o se è indicata solo la protezione contro l'accesso a parti pericolose (in questo caso la prima cifra è sostituita da una X). Le lettere (A, B, C, D) specificano ulteriormente il tipo di protezione delle persone (es. A per dorso della mano, D per filo).
    * **Esempio:** IP55 significa protetto contro le polveri, contro l'accesso con un filo, e contro i getti d'acqua. Per apparecchiature all'aperto senza tettoia, è prescritto un minimo IPX3.

5.  **Trasduttori, Sistemi di Controllo e Microcontrollori**
    * **Trasduttori:** Dispositivi che convertono una grandezza fisica (non elettrica) in un segnale elettrico proporzionale, o viceversa. Sono il primo anello di una catena di acquisizione dati.
        * **Temperatura:**
            * **Pt100/NTC:** Trasduttori resistivi (la resistenza varia con la temperatura), richiedono una conversione Resistenza/Tensione (R/V).
            * **AD590:** Trasduttore che genera una corrente proporzionale alla temperatura (conversione I/V).
            * **LM35:** Trasduttore che genera una tensione proporzionale alla temperatura (amplificazione V).
            * **Termocoppie:** Basate sull'effetto Seebeck (generano una piccola tensione in base alla differenza di temperatura tra due giunzioni), richiedono amplificazione della tensione.
        * **Posizione:**
            * **Potenziometro lineare/rotativo:** Trasduttori resistivi che convertono uno spostamento lineare o angolare in una variazione di tensione (richiedono amplificazione V).
        * **Forza:**
            * **Estensimetri:** Sensori che cambiano la loro resistenza quando deformati (conversione R/V).
            * **Piezoelettrico:** Genera una tensione quando sottoposto a una forza (amplificazione AV).
        * **Velocità angolare:**
            * **Dinamo tachimetrica:** Genera una tensione proporzionale alla velocità angolare (amplificazione V).
        * **Luminosità:**
            * **Fotoresistenza:** La resistenza varia con l'intensità luminosa (conversione R/V).
            * **Fotodiodo:** Genera una corrente proporzionale alla luce (conversione I/V).
            * **Fototransistor:** Combina fotodiodo e transistor, usato come rivelatore di passaggio (es. in encoder) o in fotoaccoppiatori (optoisolatori) per isolamento galvanico (sicurezza).
        * **Encoder:** Trasduttori digitali calettati su un albero di trasmissione per rilevare posizione o velocità angolare.
            * **Incrementale:** Genera impulsi per ogni "passo" di rotazione, utile per la velocità angolare.
            * **Assoluto:** Genera un codice binario unico per ogni posizione angolare, fornendo la posizione assoluta dell'albero (spesso con codifica Gray).
    * **Sistemi di Controllo:** Sequenze di blocchi funzionali per l'elaborazione e la gestione dei segnali.
        * **Catena di Acquisizione:** Il percorso del segnale dal trasduttore al microprocessore. Include: Trasduttore (TSD), Preamplificatore (PREAMP) e Filtro (per condizionare il segnale e rimuovere rumore), Multiplexer (MUX) per selezionare tra più canali, Amplificatore (AMPLI), Sample & Hold (S/H) per campionare e mantenere il valore del segnale, Convertitore Analogico-Digitale (ADC) per digitalizzare il segnale, e infine il Microprocessore (µP) per l'elaborazione.
        * **Catena di Distribuzione:** Il percorso del segnale dal microprocessore all'attuatore. Include: Microprocessore (µP), Convertitore Digitale-Analogico (DAC) per convertire il segnale digitale in analogico, Demultiplexer (DEMUX) per distribuire il segnale a più canali, Sample & Hold (S/H), Filtro, Amplificatore (AMPLI) e infine l'Attuatore. È possibile usare un DAC per ogni canale per maggiore complessità e costo. Attuatori a ingresso digitale (es. motore passo-passo) non richiedono DAC, ma possono necessitare di driver di potenza.
    * **Microcontrollori (µC):** Sistemi integrati che contengono una CPU, memoria e periferiche di I/O su un singolo chip, ideali per sistemi embedded.
        * **Componenti generali:**
            * **ALU (Arithmetic Logic Unit):** Esegue operazioni aritmetiche e logiche.
            * **Registri generali:** Memorie veloci per l'elaborazione dei dati.
            * **Decoder istruzioni:** Interpreta le istruzioni del programma.
            * **Controllore di interrupt:** Gestisce le richieste di interruzione dalle periferiche.
            * **RAM dati:** Memoria volatile per i dati.
            * **ROM codice:** Memoria non volatile per il programma.
            * **Porte I/O standard (TTL e analog):** Per la comunicazione con l'esterno.
            * **Porte seriali (UART/USART, SPI):** Per la comunicazione seriale con altri dispositivi.
            * **Connettività (CAN-BUS, USB, Ethernet):** Per reti e comunicazioni avanzate.
            * **Timer/counter:** Per la temporizzazione e il conteggio degli eventi.
            * **Comparatori:** Per confrontare segnali analogici.
            * **DAC/ADC multicanale:** Per conversioni analogico-digitale e digitale-analogico.
            * **Uscita PWM (Pulse Width Modulation):** Per generare segnali a larghezza di impulso variabile, utile per il controllo di motori o luminosità.
        * **Tecniche di comunicazione CPU-Periferica:**
            * **Polling:** La CPU scandisce ciclicamente tutte le periferiche per verificarne la disponibilità alla comunicazione. Semplice ma inefficiente per molte periferiche.
            * **Interrupt:** La periferica che necessita di comunicare invia una richiesta di interruzione alla CPU, che sospende il compito corrente per gestire la richiesta, migliorando l'efficienza.
        * **Arduino:** Un esempio di µC ampiamente usato per la prototipazione grazie alla sua facilità di programmazione.
    * **Prestazioni PIC (es. 16F84A, 16F688, 16F88):** I microcontrollori PIC (Peripheral Interface Controller) sono noti per la loro architettura e le loro caratteristiche.
        * **Confronto tra modelli:** Il 16F688 offre più linee I/O, più timer (due a 8 bit, uno a 16 bit), comparatori analogici, ADC multicanale (7 canali a 10 bit) e uscita PWM, rispetto al 16F84A.
        * **Caratteristiche specifiche del 16F88:** Include EEPROM per il mantenimento dei dati per oltre 40 anni, un ampio range operativo (2.0V-5.0V), un modulo CCP (Capture, Compare, PWM), porte seriali sincrone (SSP) e universali sincrone/asincrone (AUSART/SCI), compatibilità con CAN-BUS, USB, Ethernet, e un Watchdog timer per il ripristino del µC in caso di blocco del programma (copre intervalli da 1ms a 268s). Ha un set di 33 istruzioni base, con la maggior parte che richiede 4 cicli di clock.

6.  **Attuatori e Motori Elettrici**
    * **Attuatori:** Componenti che, pilotati da segnali di controllo (analogici o digitali), realizzano le variazioni desiderate di una grandezza controllata. Convertire l'energia elettrica in ingresso in altre forme di energia (meccanica, termica, idraulica, acustica).
        * **Esempi on/off:** Relè (interruttore elettromeccanico), elettrovalvola (controlla il flusso di fluidi), transistor BJT (usato come switch).
    * **Dispositivi di Potenza:** Circuiti o componenti che prelevano un segnale di controllo e lo rendono compatibile con il pilotaggio di carichi di potenza, come i motori.
        * **Amplificatori di potenza lineari (driver):** Strutture a T (mezzo ponte, es. L165) o ad H (ponte, es. L298). La struttura ad H è più complessa ma offre maggiore controllo e assenza di distorsione.
        * **Tiristori:** Dispositivi di potenza (es. SCR, TRIAC, relè a stato solido o optoisolatore) che, tramite impulsi di corrente di innesco, permettono il trasferimento di elevate potenze al carico.
    * **Motori a Corrente Continua (MCC):**
        * **Con spazzole:** Composto da uno statore con magnete permanente e un rotore con avvolgimenti eccitati tramite un complesso collettore/spazzole. È una macchina reversibile (può funzionare anche come generatore, dinamo). Presenta problemi di usura delle spazzole e innesco di archi elettrici/scintille. La sua funzione di trasferimento equivalente è del 2° ordine (filtro passa-basso). La velocità può essere controllata in catena aperta (on/off, lineare, PWM) o in catena chiusa (con retroazione, tipicamente usando una dinamo tachimetrica come trasduttore). Per il controllo del verso di rotazione, sono necessari ponti a T o H.
        * **Brushless (senza spazzole):** Impiega le stesse parti di un MCC ma con disposizione invertita (rotore a magnete permanente, statore con avvolgimenti). Il complesso collettore-spazzole è sostituito da un circuito elettronico e un trasduttore angolare (encoder, resolver, sensori Hall). Offre vantaggi come maggiore affidabilità, minore manutenzione, versatilità nell'alimentazione (AC o DC) e un controllo di velocità preciso tramite PWM. Ideale per posizionamenti di precisione, CNC e robotica.
    * **Motore Passo-Passo (Step Motor):** Un motore elettrico che converte impulsi elettrici in movimenti angolari discreti (passi). Il rotore (magnete permanente o acciaio dolce nei motori a riluttanza variabile) insegue il campo magnetico generato sullo statore per minimizzare la riluttanza. Gli spostamenti angolari sono precisi e discreti. Il pilotaggio può essere a passo intero, mezzo passo o quarto di passo, offrendo diversi livelli di precisione e fluidità di movimento.
    * **Servomotore Elettrico:** Tipicamente un complesso costituito da un MCC a magnete permanente e un dispositivo di feedback (dinamo tachimetrica o encoder) calettato direttamente sull'albero. Spesso accoppiato con un motoriduttore per ottenere rapide accelerazioni e alte coppie di spunto. Il segnale pilota consente di realizzare servomeccanismi (controllo di posizione) o servosistemi (controllo di velocità) ad alta precisione.
    * **Motori in Corrente Alternata:**
        * **Principio di funzionamento:** Gli avvolgimenti dello statore alimentati in corrente alternata generano un campo magnetico rotante. Questo campo induce forze elettromotrici (fem) negli avvolgimenti del rotore, che per reazione si oppongono alla causa che le genera, mettendo in rotazione il rotore. Le correnti sul rotore sono generate per induzione, da cui il nome "motore a induzione".
        * **Sincroni:** Il rotore "aggancia" il campo magnetico rotante e ruota in sincronismo con esso alla velocità $n_{\\circ} = (60 \\times f) / p$, dove $f$ è la frequenza della tensione di alimentazione e $p$ è il numero di coppie polari sullo statore.
        * **Asincroni:** La velocità del rotore ($n$) è leggermente inferiore alla velocità di sincronismo ($n_{\\circ}$) a causa di uno "scorrimento" ($s$). La relazione è $n = n_{\\circ} \\times (1-s)$. Sono i motori più diffusi nell'industria per la loro robustezza e semplicità costruttiva.