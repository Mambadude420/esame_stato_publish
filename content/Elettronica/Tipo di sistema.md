---
lastSync: Sat May 24 2025 18:23:23 GMT+0200 (Ora legale dell’Europa centrale)
---
Il "tipo" di sistema di controllo ad anello chiuso è determinato dal numero di [integratori](Integratore.md) ($1 / s$ termini) presenti nella funzione di trasferimento ad anello aperto $G(s) H(s)$. Il tipo di sistema ha un impatto diretto sulla precisione nel seguire diversi tipi di ingressi ([gradino](Ingresso%20a%20gradino%20(Step%20input).md), [rampa](Ingresso%20a%20rampa%20(Ramp%20input).md), [parabola](Ingresso%20a%20parabola%20(Parabolic%20input).md)).

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


---
### Precedente
[Precisione di un sistema](Precisione%20di%20un%20sistema.md)

### Successivo


### Riferimenti
[Errore a regime costante e non nullo](Errore%20a%20regime%20costante%20e%20non%20nullo.md)
[Ingresso a gradino (Step input)](Ingresso%20a%20gradino%20(Step%20input).md)
[Ingresso a rampa (Ramp input)](Ingresso%20a%20rampa%20(Ramp%20input).md)
[Ingresso a parabola (Parabolic input)](Ingresso%20a%20parabola%20(Parabolic%20input).md)