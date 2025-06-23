---
lastSync: Fri May 30 2025 14:23:09 GMT+0200 (Ora legale dell’Europa centrale)
aliases:
  - disposizioni
---
Mentre le permutazioni riguardano l'ordinamento di _tutti_ gli elementi disponibili, le disposizioni entrano in gioco quando scegliamo un _sottoinsieme_ di elementi da un gruppo più grande e l'ordine in cui li scegliamo è importante.

Considerando una gara di corsa con 10 partecipanti, quanto modi ci sono per assegnare la medagli d'oro, d'argento e di bronzo? Qui l'ordine è cruciale: arrivare primo, secondo o terzo sono posizioni diverse e la stessa persona al primo posto e poi al secondo posto sono due scenari completamente diversi. Inoltre, non stiamo considerando tutti i 10 partecipanti, ma solo i primi 3 classificati.

La formula per le disposizioni di $k$ elementi scelti da un insieme di $n$ elementi distinti (senza ripetizione) è:
$$
D_{n, k} = \frac{n!}{(n-k)!}
$$
Dove:
- $n$ è il numero totale di elementi disponibili
- $k$ è il numero di elementi che scegliamo
- $n \geq k$ (non puoi scegliere più elementi di quelli che hai!)

Riprendendo l'esempio della gara: $n = 10$ (i partecipanti) e $k = 3$ (le medaglie).
$$
D_{10, 3} = \frac{10!}{(10 -3)!} = \frac{10!}{7!} = \frac{{10 \times 9 \times 8 \times 7!}}{7!} = 10 \times 9 \times 8 =720
$$
Ci sono 720 modi diversi per assegnare le medagli d'oro, d'argento e di bronzo.

**Esercizio:**
In una classe ci sono 20 studenti. Si deve eleggere un rappresentante di classe, un vice-rappresentante e un segretario. Ogni studente può ricoprire una sola carica.
Quanti modi diversi ci sono per eleggere queste tre figure?

Soluzione: $n = 20$ (studenti) e $k = 3$ (cariche disponibili).
$$
D_{20, 3} = \frac{20!}{(20 -3)!} = \frac{20!}{17!} = \frac{{20 \times 19 \times 18 \times 17!}}{17!} = 20 \times 19 \times 18 = 6840
$$
Ci sono 6840 modi diversi per eleggere queste tre figure.