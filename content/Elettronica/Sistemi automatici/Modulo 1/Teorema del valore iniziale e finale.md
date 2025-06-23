---
lastSync: Sat Jun 14 2025 16:58:21 GMT+0200 (Ora legale dell’Europa centrale)
---
## Teorema del Valore Iniziale
Questo teorema ci dice il valore di una funzione f(t) nel momento iniziale ($t \rightarrow 0^+$), utilizzando la sua trasformata di Laplace $F(s)$.
$$
\lim_{ t \to 0^+ } f(t) = \lim_{ t \to \infty } sF(s)
$$
##### **Cosa significa?**
 Se vuoi sapere da che valore parte un segnale appena "acceso" (t appena dopo lo zero), ti basta prendere la sua trasformata F(s), moltiplicarla per s, e poi vedere a cosa tende l'espressione quando s diventa molto, molto grande (∞).
 
##### **Condizioni d'uso:**
È importante che il limite di $sF(s)$ esista. Se ci sono poli di $sF(s)$ sull'asse immaginario o nel semipiano destro del piano complesso, il teorema potrebbe non essere applicabile.

##### **Esempio:**
Immagina di accendere una luce. Il teorema del valore iniziale ti direbbe qual è la luminosità esatta nel momento in cui la accendi (o appena dopo), anche se hai solo la formula che descrive come la luminosità cambia nel tempo nel dominio di s.

## Teorema del Valore Finale
Questo teorema, al contrario, ci dice il **valore di una funzione f(t) dopo un tempo infinitamente lungo (t→∞)**, sempre utilizzando la sua Trasformata di Laplace F(s). È particolarmente utile per capire il **comportamento a regime** di un sistema, cioè come si stabilizza dopo un lungo periodo.
$$
\lim_{ t \to \infty } f(t) = \lim_{ t \to 0 } sF(s)
$$
##### **Cosa significa?**
Se vuoi sapere a che valore si stabilizza un segnale dopo tanto tempo, prendi la sua trasformata F(s), moltiplicala per s, e poi vedi a cosa tende l'espressione quando s si avvicina a zero.

##### **Condizioni d'uso:**
Questa è la parte cruciale per la stabilità! Affinché questo teorema sia valido, tutti i poli di sF(s) devono avere parte reale negativa (cioè devono trovarsi nel semipiano sinistro del piano complesso), ad eccezione di un polo semplice in s=0. Se ci sono poli sull'asse immaginario (eccetto s=0) o nel semipiano destro, il sistema non si stabilizza o oscilla indefinitamente, e il teorema non può essere applicato per trovare un valore finale finito. Questo è un concetto che approfondiremo quando parleremo di stabilità!

##### **Esempio:**
Tornando alla luce, il teorema del valore finale ti direbbe a che livello di luminosità si stabilizza la luce dopo un bel po' di tempo che è accesa.