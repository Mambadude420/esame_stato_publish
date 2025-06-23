---
lastSync: Sun Jun 15 2025 15:51:25 GMT+0200 (Ora legale dell’Europa centrale)
---
### Sistemi del Secondo Ordine con e Senza Retroazione con Ingresso a Scalino

Dopo i [[Sistemi del primo ordine con e senza retroazione con ingresso a scalino.md|sistemi del primo ordine]], i **sistemi del secondo ordine** sono i successivi "mattoni" fondamentali nell'analisi dei sistemi di controllo. Sono estremamente importanti perché molti sistemi fisici complessi possono essere approssimati con un modello del secondo ordine, e la loro risposta include comportamenti molto comuni come le oscillazioni.

Un **sistema del secondo ordine** è descritto da un'equazione differenziale del secondo ordine. Nel dominio di Laplace, la sua Funzione di Trasferimento (FDT) ha la forma canonica (standard) seguente:

$$
G(s) = \frac{{K \omega_{n}^2}}{s^{2} + 2 \zeta \omega_{n}s + \omega_{n}^{2}}
$$

Dove:

- $ω_{n}$ (omega n) è la **frequenza naturale non smorzata** (in rad/s). Questo parametro indica la frequenza alla quale il sistema oscillerebbe se non ci fosse smorzamento. Immagina un pendolo perfetto: ωn​ sarebbe la sua frequenza di oscillazione.
- ζ (zeta) è il **[[Smorzamento.md|fattore di smorzamento]]**. Questo è un parametro cruciale che determina la **forma della risposta transitoria** del sistema. Ci dice quanto "smorzate" (o meno) saranno le oscillazioni.