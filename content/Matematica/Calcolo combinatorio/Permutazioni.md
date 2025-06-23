---
lastSync: Fri May 30 2025 14:23:14 GMT+0200 (Ora legale dell’Europa centrale)
aliases:
  - permutazioni
---
Si immagini di avere un gruppo di oggetti distinti e di volerli disporre in un certo ordine. Le permutazioni ci dicono quanti modi diversi ci sono per ordinare tutti questi oggetti. La parola chiave qui è "ordine": se l'ordine cambia, otteniamo una permutazione diversa.

Se hai tre libri diversi (A, B , C) su uno scaffale, quanto modi diversi ci sono per disporli?
- ABC
- ACB
- BAC
- BCA
- CAB
- CBA
Ci sono 6 modi diversi.

La formula per calcolare il numero di permutazioni di $n$ oggetti oggetti distinti è $P_{n} = n!$ (n fattoriale). Il fattoriale di un numero $n$ è il prodotto di tutti gli interi positivi minori o uguali a $n$.

**Esempio:**
- 3!=3×2×1=6 (come nell'esempio dei libri)
- 4!=4×3×2×1=24
- 1!=1
- 0!=1 (questa è una definizione un po' speciale, ma utile per la matematica!)