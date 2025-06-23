---
lastSync: Fri May 30 2025 16:36:13 GMT+0200 (Ora legale dell’Europa centrale)
aliases:
  - regola empirica
---
Questa regola è un modo rapido per capire la dispersione dei dati in una distribuzione normale senza dover fare calcoli complessi con la formula ella densità di probabilità. È una conseguenza diretta della forma a campana ella Gaussiana e della sua simmetria.

Consideriamo una distribuzione normale con una media ($\micro$) e una deviazione standard ($\sigma$).

La regola afferma che:
1. Entro **1 Deviazione Standard (68%)** di tutti i dati si trova all'interno di una deviazione standard dalla media.
	- Questo significa che, se prendiamo la media e ci spostiamo di una deviazione standard a sinistra ($\micro - \sigma$) e di una deviazione standard a destra ($\micro + \sigma$), l'intervallo \[$\micro - \sigma$, $\micro + \sigma$] conterrà circa il 68% delle osservazioni.
	- *Esempio*: Se l'alteza media di una popolazione è 170 cm ($\micro$) e la deviazione standard è 5 cm ($\sigma$), allora il 68% delle persone avrà un altezza tra 165 cm (170 - 5) e 175 cm (170 + 5).
2.  Entro **2 Deviazione Standard (95%**) di tutti i dati si trova all'interno due due deviazioni standard alla media.
	- L'intervallo è \[$\micro - 2\sigma, \micro + 2\sigma$]
	- *Esempio*: Usando l'esempio delle altezze, il 95% delle persone avrà un'altezza tra 160 cm (170 - 2_5) e 180 cm (170 + 2_5). Si noti che al di fuori di questo intervallo c'è solo il 5% delle persone, che si divide tra le persone molto basse e quelle molto alte.
3. Entro **3 Deviazioni Standard (99.7%)** di tutti i dati si trova all'interno di tre deviazioni standard dalla media.
	- L'intervallo è \[$\micro - 3\sigma , \micro + 3\sigma$]
	- - _Esempio:_ Nell'esempio precedente il 99.7% delle persone avrà un'altezza tra 155 cm (170 - 35) e 185 cm (170 + 35). Questo significa che è estremamente raro trovare persone al di fuori di questo intervallo, perché solo lo 0.3% della popolazione si trova lì.

#### Perché è così utile?

- **Identificazione di valori anomali:** Questa regola ci aiuta a capire quando un valore è "normale" o "insolito". Se un dato cade al di fuori di 2 o 3 deviazioni standard dalla media, è considerato un valore anomalo o estremo, il che potrebbe indicare un errore di misurazione o un evento raro.
- **Stima rapida:** Permette di fare stime rapide sulla diffusione dei dati se conosciamo solo la media e la deviazione standard.
- **Base per i test di ipotesi:** È alla base di molti test statistici e del concetto di intervalli di confidenza, che userai per fare inferenza.