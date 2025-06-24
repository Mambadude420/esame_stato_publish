---
lastSync: Sat May 24 2025 18:23:23 GMT+0200 (Ora legale dell’Europa centrale)
---
Il "tipo" di sistema di controllo ad anello chiuso è determinato dal numero di [[Integratore.md|integratori]] ($1 / s$ termini) presenti nella funzione di trasferimento ad anello aperto $G(s) H(s)$. Il tipo di sistema ha un impatto diretto sulla precisione nel seguire diversi tipi di ingressi ([[Ingresso a gradino (Step input|gradino]].md), [[Ingresso a rampa (Ramp input|rampa]].md), [[Ingresso a parabola (Parabolic input|parabola]].md)).

- Sistema di Tipo 0: non ha integratori ($s$ al denominatore)
	- Errore a regime costante e non nullo per un ingresso a gradino
	- Errore a regime tendente all'infinito per un ingresso a rampo o parabola
- Sistema di Tipo 1: ha un integratore ($\frac{1}{s}$) nella funzione di trasferimento ad anello aperto
	- Errore a regime nullo per un ingresso a gradino
	- Errore a regime costante e non nullo per un ingresso a rampa
	- Errore a regime tendente all'infinito per un ingresso a parabola
- Sistema di Tipo 2: ha due integratori ($\frac{1}{s^2}$) nella funzione di trasferimento ad anello aperto
	- Errore a regime nullo per un ingresso a gradino o a rampa
	- Errore a regime costante e non nullo per un ingresso a parabola


# Riferimenti e collegamenti
### Precedente
[[Precisione di un sistema.md]]

### Successivo


### Riferimenti
[[Errore a regime costante e non nullo]]  
[[Step input)](Ingresso a gradino (Step input|Ingresso a gradino (Step input)]]  
[[Ramp input)](Ingresso a rampa (Ramp input|Ingresso a rampa (Ramp input)]]  
[[Parabolic input)](Ingresso a parabola (Parabolic input|Ingresso a parabola (Parabolic input)]]