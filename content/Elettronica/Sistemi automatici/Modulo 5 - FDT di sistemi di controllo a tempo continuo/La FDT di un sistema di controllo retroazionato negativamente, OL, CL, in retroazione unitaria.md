---
lastSync: Wed Jun 18 2025 23:15:32 GMT+0200 (Ora legale dell’Europa centrale)
---
Nel contesto dei sistemi di controllo a **retroazione negativa**, ci sono tre FDT principali che dobbiamo conoscere a fondo, poiché ciascuna ci fornisce informazioni diverse e cruciali sul comportamento del sistema.

#### 1. Funzione di Trasferimento ad Anello Aperto (L(s))

La **Funzione di Trasferimento ad Anello Aperto**, spesso indicata con L(s), rappresenta il guadagno complessivo che si ottiene percorrendo l'intero anello di retroazione, dal punto di errore fino all'uscita del blocco di feedback, **immaginando di "aprire" l'anello**.

In un sistema di controllo generico con retroazione negativa, che include un **controllore** C(s), un **processo (o impianto)** P(s) e un **blocco di feedback** H(s) (che modella il sensore o qualsiasi condizionamento del segnale di retroazione), la FDT ad anello aperto è semplicemente il prodotto di tutte le FDT lungo il percorso:
$$
L(s)=C(s)P(s)H(s)
$$
**Perché è importante?** Questa funzione è la chiave per analizzare la **stabilità** del sistema ad anello chiuso usando strumenti come i diagrammi di Nyquist e Bode (che vedremo nel Modulo 6). Se L(s) non rispetta certe condizioni, il tuo sistema ad anello chiuso potrebbe oscillare senza controllo o diventare instabile.

#### 2. Funzione di Trasferimento ad Anello Chiuso $G_{CL}(s) \ \text{o} \ T(s)$

La **Funzione di Trasferimento ad Anello Chiuso**, indicata con GCL​(s) o talvolta T(s) (dall'inglese _transfer function_ o _overall transfer function_), descrive la relazione tra l'**ingresso di riferimento** (R(s)) e l'**uscita del sistema** (Y(s)), considerando l'intero loop di retroazione attivo.

Per un sistema a retroazione negativa, la sua derivazione porta alla formula fondamentale:
$$
G_{CL}​(s)=\frac{Y(s)​}{R(s)}=\frac{C(s)P(s)}{1+C(s)P(s)H(s)}​
$$
A volte, si usa la notazione G(s)=C(s)P(s) per indicare la funzione di trasferimento del "ramo diretto" (controllore + processo). In quel caso la formula diventa:
$$
G_{CL}​(s)=\frac{G(s)}{1+G(s)H(s)}​
$$
**Perché è importante?** Questa FDT ci dice come l'intero sistema di controllo risponde ai comandi che gli vengono dati. È ciò che useremmo per analizzare la **risposta transitoria** (ricordi, come si comporta con un ingresso a scalino?) e l'**errore a regime** del sistema finale. Se GCL​(s) ha poli nel semipiano destro, il sistema è instabile.

#### 3. Retroazione Unitaria

Un caso speciale e molto comune è quello della **retroazione unitaria**. Si verifica quando il blocco di feedback H(s) è semplicemente 1. Questo significa che il segnale misurato dall'uscita viene confrontato direttamente con il segnale di riferimento, senza alcuna modifica o guadagno/filtro aggiuntivo nel percorso di feedback.

In questo scenario, le formule si semplificano:

- **FDT ad Anello Aperto (con retroazione unitaria):
$$
L(s)=C(s)P(s)
$$
- **FDT ad Anello Chiuso (con retroazione unitaria):**
$$
G_{CL}​(s)=\frac{C(s)P(s)}{1+C(s)P(s)}
$$​
- o, usando G(s)=C(s)P(s):
$$
G_{CL}​(s)=\frac{G(s)}{1+G(s)}​
$$
**Perché è importante?** Molti sistemi reali possono essere approssimati a un modello a retroazione unitaria per semplificare l'analisi e il progetto. Inoltre, le proprietà di stabilità e prestazione sono spesso discusse in riferimento a questo caso semplificato.