---
lastSync: Sat Jun 14 2025 17:05:37 GMT+0200 (Ora legale dell’Europa centrale)
---
Se la Trasformata di Laplace è il nostro "traduttore" che porta un segnale dal dominio del tempo al dominio di $s$, l'**Anti-trasformata di Laplace** è il processo inverso. È il "traduttore al contrario" che ci riporta dal dominio di $s$ al dominio del tempo.

##### **Perché è così importante?**
Ricordi l'ingegnere che risolveva le equazioni differenziali nel dominio di s? Una volta trovata la soluzione F(s) in quel dominio più semplice, ha bisogno di sapere come si comporta il circuito **nel tempo reale**. Ed è qui che interviene l'Antitrasformata di Laplace. Essa prende quella soluzione "tradotta" e la riporta nella sua forma originale nel tempo, f(t), che è ciò che l'ingegnere può misurare e osservare nel mondo fisico.

### Come si calcola l'Anti-trasformata?
Ci sono diversi modi, ma i più comuni e pratici per la maggior parte delle applicazioni in sistemi di controllo sono:

1. **Consultazione delle tabelle delle Trasformate Notevoli:** Per fortuna, non dobbiamo fare ogni volta l'integrale della Trasformata di Laplace per l'antitrasformata! Esistono delle tabelle che associano funzioni comuni nel tempo alle loro trasformate di Laplace. Spesso, per anti-trasformare un'espressione F(s), si cerca di ricondurla a una di queste forme note.
    
2. **Decomposizione in Frazioni Parziali:** Questa tecnica è fondamentale. Spesso, l'espressione F(s) che otteniamo risolvendo un problema è una frazione razionale (un rapporto di polinomi in $s$). Per anti-trasformarla, la si scompone in una somma di frazioni più semplici, ognuna delle quali ha una forma riconoscibile nelle tabelle.
    
    Ad esempio, se abbiamo una F(s) come questa:
$$
F(s) = \frac{K}{(s + a)(s + b)}
$$
	La decomponiamo in:
$$
F(s) = \frac{A}{s + a} + \frac{B}{s + b}
$$
	Dive $A$ e $B$ sono costanti che calcoliamo. Ognuna di queste frazioni più semplici è facilmente anti-trasformabile usando le tabelle.