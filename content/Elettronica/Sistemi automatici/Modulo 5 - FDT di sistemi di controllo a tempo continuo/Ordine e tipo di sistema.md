---
lastSync: Wed Jun 18 2025 23:46:50 GMT+0200 (Ora legale dell’Europa centrale)
---
### Ordine del Sistema
L'**ordine di un sistema** lineare e stazionario è definito come il **grado del polinomio al denominatore della sua Funzione di Trasferimento (FDT)**, una volta che numeratore e denominatore sono stati semplificati (cioè, non ci sono cancellazioni polo-zero).

In modo equivalente, l'ordine di un sistema è il **numero di poli** della sua FDT. È anche il grado dell'equazione differenziale che descrive la dinamica del sistema.

**Perché è importante?** L'ordine ci dice quanti "elementi di accumulo di energia" (come masse, molle, condensatori, induttori) ci sono nel sistema e, di conseguenza, ci dà un'idea della sua complessità dinamica.

- Un **sistema del primo ordine** (che abbiamo già visto) ha un solo polo e una risposta esponenziale.
- Un **sistema del secondo ordine** (che abbiamo anche visto) ha due poli (reali o complessi coniugati) e può mostrare comportamenti oscillatori.
- Sistemi di ordine superiore avranno più poli e risposte più complesse, ma spesso possono essere approssimati con sistemi di ordine inferiore per l'analisi.

---
### Tipo di Sistema
Il **tipo di un sistema** si riferisce al numero di **poli della Funzione di Trasferimento ad Anello Aperto L(s) che si trovano nell'origine** del piano complesso (s=0). In altre parole, è il numero di termini s al denominatore di L(s) se s non è moltiplicato da altre costanti o addizionato a esse.

Il tipo di sistema è cruciale perché determina la capacità del sistema a retroazione chiusa di inseguire diversi tipi di segnali di riferimento (gradino, rampa, parabola) con un **errore a regime nullo**. Questo è un concetto che approfondiremo moltissimo quando parleremo dell'errore a regime.

- **Sistema di Tipo 0:** Non ha poli nell'origine. La L(s) non ha termini s al denominatore.
    - Esempio: $L(s)=\frac{K}{(s+1)(s+2)}$. Questo sistema avrà in genere un errore a regime _costante e non nullo_ in risposta a un ingresso a gradino.
- **Sistema di Tipo 1:** Ha un polo nell'origine. La L(s) ha un termine s al denominatore.
    - Esempio: $L(s)=\frac{K}{s(s+1)}$. Questo sistema avrà un errore a regime _nullo_ in risposta a un ingresso a gradino, ma un errore _costante e non nullo_ in risposta a un ingresso a rampa.
- **Sistema di Tipo 2:** Ha due poli nell'origine. La L(s) ha un termine $s^2$ al denominatore.
    - Esempio: $L(s)=\frac{K}{s^2(s+1)}$. Questo sistema avrà un errore a regime _nullo_ in risposta a un ingresso a gradino e a rampa, ma un errore _costante e non nullo_ in risposta a un ingresso a parabola.

E così via per tipi superiori. Ogni polo nell'origine aggiunge un'integrazione nel loop, che migliora la capacità del sistema di eliminare gli errori a regime per determinati tipi di ingresso.