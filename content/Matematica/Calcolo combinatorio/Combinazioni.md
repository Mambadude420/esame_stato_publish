---
lastSync: Fri May 30 2025 14:27:30 GMT+0200 (Ora legale dell’Europa centrale)
aliases:
  - combinazioni
---
Nelle combinazioni, a differenza delle permutazioni e delle disposizioni, **l'ordine degli elementi NON è importante**. Ci interessa solo quali elementi vengono scelti, non in che sequenza.

Si consideri quando si prepara una macedonia di frutta: se metti mele, pere e banane, il risultato è lo stesso sia che vengano aggiunte nell'ordine "mele, pere, banane" sia che vengano messe nell'ordine "banane, mele, pere". L'insieme finale degli ingredienti è lo stesso.

Un altro esempio classico è la scelta dei numeri per una lotteria (tipo il Superenalotto, ma in piccolo): se scegli i numeri 1, 5, 10, non importa se li segni sulla schedina come "1, 5, 10" o "10, 1, 5". L'importante è averli scelti.

La formula per calcolare il numero di combinazioni di $k$ elementi scelti da un insieme di $n$ elementi distinti (senza ripetizione) è:
$$
C_{n, k} = \binom {n}{k} = \frac{n!}{k! (n - k)!}
$$
Il simbolo $\binom {n}{k}$ si legge "n su k" ed è chiamato coefficiente binomiale. Da notare che è molto simile alla formula delle disposizioni, ma con un k! al denominatore. Questo k! serve proprio a "togliere" l'importanza dell'ordine, dividendo per il numero di permutazioni possibili degli k elementi scelti.

Tornando all'esempio della macedonia: se hai 5 tipi di frutta e vuoi sceglierne 3 per la tua macedonia:
$n=5$ (tipi di frutta) e $k=3$ (frutta da scegliere).
$$
C_{5, 3} = \frac{5!}{3!(5 - 3)!} = \frac{5!}{3! 2!} = \frac{{5 \times 4 \times 3 \times 2 \times 1}}{(3 \times 2 \times 1) (2 \times 1)} = \frac{120}{6 \times 2} = \frac{120}{12} = 10
$$
Ci sono 10 modi diversi per scegliere 3 tipi di frutta da 5.

**Esercizio:**
In un'urna ci sono 12 palline numerate da 1 a 12. Si estraggono contemporaneamente 3 palline.
Quante diverse combinazioni di 3 palline si possono ottenere?

Soluzione: $n = 12$ (palline totali) e $k = 3$ (estrazione).
$$
C_{12,3} = \binom{12}{3} = \frac{12!}{3!(12-3)!} = \frac{12!}{3!9!} = \frac{12 \times 11 \times 10 \times 9!}{ (3 \times 2 \times 1) \times 9!}
$$
Ci sono 220 diverse combinazioni di 3 palline che si possono ottenere.