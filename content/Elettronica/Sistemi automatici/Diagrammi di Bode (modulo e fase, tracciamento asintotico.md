---
lastSync: Sat Jun 14 2025 19:09:31 GMT+0200 (Ora legale dell’Europa centrale)
---
### Diagrammi di Bode: Modulo e Fase, Tracciamento Asintotico

Mentre il Diagramma di Nyquist ci offre una visione completa della risposta in frequenza in un unico grafico nel piano complesso, i **Diagrammi di Bode** la dividono in due grafici separati, il che li rende spesso più intuitivi da disegnare (soprattutto a mano) e da interpretare per capire l'impatto dei singoli componenti del sistema.

I Diagrammi di Bode sono un modo per rappresentare il **guadagno (o modulo)** e lo **sfasamento (o fase)** di una funzione di trasferimento L(jω) (che, ti ricordo, è la nostra funzione di trasferimento ad anello aperto) in funzione della frequenza ω. Entrambi gli assi della frequenza sono rappresentati su scala logaritmica.

Sono composti da due grafici:
1. **Diagramma dei Moduli (o del Guadagno):** Rappresenta il **modulo** di L(jω) espresso in **decibel (dB)** in funzione della frequenza ω (in scala logaritmica). Il modulo in dB si calcola come: $M_{dB}​=20log_{10}​∣L(jω)∣$. Usare i decibel è comodo perché le moltiplicazioni delle funzioni di trasferimento (che corrispondono a blocchi in serie) si trasformano in semplici somme sui diagrammi di Bode.
2. **Diagramma delle Fasi:** Rappresenta la **fase** di L(jω) in gradi (o radianti) in funzione della frequenza ω (in scala logaritmica).