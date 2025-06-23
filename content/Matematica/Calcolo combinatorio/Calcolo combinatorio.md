---
lastSync: Fri May 30 2025 14:44:25 GMT+0200 (Ora legale dell’Europa centrale)
---
Il calcolo combinatorio è un ramo della matematica che si occupa di contare quanti raggruppamenti diversi si possono formare a partire da un certo numero di elementi, seguendo determinate regole.
Esempi:
- Scelta di cosa indossare: quante combinazioni di vestiti puoi creare con quello che hai nell'armadio?
- Decidere i posti a tavola: quante diverse disposizioni sono possibili?

##### Concetti principali nel calcolo combinatorio:
- **Permutazioni**: Le [permutazioni](Permutazioni.md) si usano quando l'ordine degli elementi è importante e si usano tutti gli elementi a disposizione.
- **Disposizioni**: Le [disposizioni](Disposizioni.md)] si usano quando l'ordine degli elementi è importante, ma si seleziona solo un sottoinsieme degli elementi disponibili.
- **Combinazioni**: Le [combinazioni](Combinazioni.md) si usano quando l'ordine degli elementi NON è importante e si seleziona un sottoinsieme degli elementi disponibili.

##### Come distinguerli?
La chiave per distinguere tra i tre è farsi due domande fondamentali:
1. L'rodine è importante?
2. Si usano tutti gli elementi a disposizione?


| Tipo di raggruppamento | Ordine importante? |  Si usano tutti gli elementi?   |                                                   Esempio chiave                                                    |
| :--------------------: | :----------------: | :-----------------------------: | :-----------------------------------------------------------------------------------------------------------------: |
|      Permutazioni      |         Si         |               Si                |                                           Disporre libri su uno scaffale                                            |
|      Disposizioni      |         Si         | No (si sceglie un sottoinsieme) |        Assegnare medaglie (oro, argento, bronzo); eleggere cariche specifiche (presidente, vicepresidente).         |
|      Combinazioni      |         No         | No (si sceglie un sottoinsieme) | Scegliere ingredienti per una macedonia; estrarre numeri per una lotteria (senza importare l'ordine di estrazione). |

#### Esempi pratici
Immaginiamo di avere 3 amici ( immagina, almeno quello puoi :') ): Anna (A), Beatrice (B), Carlo (C).
- **Scenario 1: Permutazioni**
    - Vogliamo sapere in quanti modi diversi possono sedersi in fila su 3 sedie.
    - L'ordine è importante (ABC è diverso da ACB).
    - Usiamo tutti gli amici disponibili.
    - Risposta: $3!=6$ modi (ABC, ACB, BAC, BCA, CAB, CBA).
- **Scenario 2: Disposizioni**
    - Dobbiamo scegliere un caposquadra e un vice-caposquadra tra i 3 amici.
    - L'ordine è importante (se Anna è caposquadra e Beatrice vice, è diverso da Beatrice caposquadra e Anna vice).
    - Non usiamo tutti gli amici (ne scegliamo solo 2 su 3).
    - Risposta: $D_{3,2} ​= \frac{3!}{(3−2)}! ​= \frac{3!}{1!} ​= 3 \times 2 = 6$ modi (AB, AC, BA, BC, CA, CB).
- **Scenario 3: Combinazioni**
    - Dobbiamo scegliere 2 amici per andare a comprare le pizze.
    - L'ordine NON è importante (se scegli Anna e Beatrice, è lo stesso che scegliere Beatrice e Anna).
    - Non usiamo tutti gli amici (ne scegliamo solo 2 su 3).
    - Risposta: $C_{3, 2} = \frac{3!}{2!(3 - 2)!} = \frac{3!}{2! 1!} = \frac{6}{2 \times 1} = 3$ modi (AB, AC, BC).