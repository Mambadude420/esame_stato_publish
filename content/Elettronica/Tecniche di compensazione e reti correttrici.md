---
lastSync: Sat May 24 2025 21:36:32 GMT+0200 (Ora legale dell’Europa centrale)
---
Possibile intervenire su retroazione per stabilizzare $G_{s}$ (o aumentare i margini di stabilità).

$\downarrow \downarrow$ Guadagno Statico $\rightarrow$ $\downarrow \downarrow$ Precisione

Una via alternativa è quella di bilanciare la reazione, intervenendo sui poli)
```mermaid
graph LR
	Ingresso>"R(s)"] --> controllo((" "))
	controllo --> C["C(s)"]
	C --> G["Gol(s)"]
	G --> punto((" "))
	punto --> Uscita>"Ur(s)"]
	punto --> controllo
```
