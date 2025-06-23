---
lastSync: Sun Jun 15 2025 16:09:50 GMT+0200 (Ora legale dell’Europa centrale)
aliases:
  - smorzamento
  - fattore di smorzamento
---
ζ (zeta) è il **fattore di smorzamento**. Questo è un parametro cruciale che determina la **forma della risposta transitoria** del sistema. Ci dice quanto "smorzate" (o meno) saranno le oscillazioni.

#### Importanza del Fattore di Smorzamento (ζ)

Il fattore di smorzamento ζ è il vero "direttore d'orchestra" per la risposta di un sistema del secondo ordine. In base al suo valore, distinguiamo diversi tipi di risposta all'ingresso a scalino:

1. **Sistemi Sovrasmorzati (ζ>1):**    
    - La risposta è **lenta** e **non presenta oscillazioni**. Sembra una risposta del primo ordine, ma più lenta.
    - I poli del sistema sono reali e distinti, e si trovano sull'asse reale negativo.
    - È come cercare di far affondare un oggetto molto denso nella melassa: scende lentamente senza oscillare.
2. **Sistemi Criticamente Smorzati (ζ=1):**
    - La risposta è la **più veloce possibile senza generare oscillazioni**. È il punto di equilibrio ideale tra velocità e assenza di oscillazioni.
    - I poli sono reali e coincidenti, e si trovano sull'asse reale negativo.
    - È come calare un oggetto in un liquido esattamente con la densità giusta per fermarsi subito senza galleggiare né sprofondare troppo velocemente.
3. **Sistemi Sottosmorzati (0<ζ<1):**
    - La risposta è **oscillatoria** e presenta una **sovraelongazione** ([[overshoot.md|overshoot]]), cioè l'uscita supera il valore finale desiderato prima di stabilizzarsi.
    - I poli sono complessi coniugati e si trovano nel semipiano sinistro del piano complesso.
    - Più ζ si avvicina a 0, maggiori saranno le oscillazioni e la sovraelongazione.
    - È come un pendolo che oscilla per un po' prima di fermarsi.
4. **Sistemi Non Smorzati (ζ=0):**
    - La risposta è una **oscillazione continua** e non si stabilizza mai.
    - I poli sono immaginari puri e si trovano sull'asse immaginario.
    - È un pendolo ideale che oscilla all'infinito senza attrito.
5. **Sistemi Instabili (ζ<0):**
    - La risposta cresce esponenzialmente e oscilla con ampiezza crescente. Il sistema è instabile.
    - I poli si trovano nel semipiano destro del piano complesso.
    - Immagina di spingere un pendolo e, invece di rallentare, ogni spinta lo fa oscillare sempre di più.