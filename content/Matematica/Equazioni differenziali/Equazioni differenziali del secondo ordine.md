---
lastSync: Sun May 11 2025 18:55:43 GMT+0200 (Ora legale dell’Europa centrale)
---
Un' equazione differenziale di secondo ordine è un'equazione che coinvolge una funzione incognita $y(x)$, la sua derivata prima $y'$, la sua derivata seconda $y''$, e possibilmente la variabile indipendente $x$.

##### Perché sono importanti?
Le equazione differenziali di secondo ordine compaiono in moltissimi campi della scienze e dell'ingnegneria per descrivere fenomeni che dipendono non solo dallo stato attuale di un sistema, ma anche dalla velocità con cui tale stato sta cambiando.
Ad esempio:
- In **fisica**: il moto di un oggetto soggetto a una forza ( come un pendolo o una massa attaccata a una molla) è spesso descritto da equazioni differenziali di secondo ordine (la famosa legge di Newton, $F = ma$, dove l'accelerazione $a$ è la derivata seconda della posizione).
- **L'ingegneria**: L'analisi di circuiti elettrici ( con induttori e condensatori), la vibrazione di strutture (come ponti e edifici), e il trasferimento di calore spesso portano a equazioni di questo tipo.
- **La biologia**: Modelli di crescita di popolazioni o la diffusione di malattie possono essere descritti da sistema di equazioni differenziali, alcune delle quali possono essere di secondo ordine.

##### Cosa rende le equazioni di secondo ordine "di secondo ordine"?
Semplicemente, la presenza della **derivata seconda** come la derivata di ordine più alta nell'equazione. Se ci fosse solo la derivata prima, sarebbe un'equazione differenziale del primo ordine.

###### Come si svolge un equazione differenziale lineare omogenea del secondo ordine a coefficienti costanti?
Un'equazione della forma:
$$
ay'' - by' + cy = 0
$$
dove $a$, $b$, $c$, sono costanti reali ($a \neq 0$), dipende dalla radici dell'equazione caratteristica associata:
$$
ar^2 + br + c = 0
$$
Il discriminante ($\Delta$, delta) di questa equazione quadratico, $\Delta = b^2 - 4ac$, determina la natura delle radici $r$ e, di conseguenza, la forma della soluzione generale dell'equazoine differenziale.

### Caso 1: $\Delta > 0$ (Delta maggiore di 0)
1. Radici dell'equazione caratteristica: Ci sono due radici reali e distinte, $r_{1}$ e $r_{2}$.
$$
x = \frac{ -b \pm \sqrt{ b^2 - 4ac } }{ 2a } = \frac {- b \pm \\\\sqrt{ \Delta } } { 2a}
$$
2. Soluzioni fondamentali: Le due soluzioni linearmente indipendenti dell'equazione differenziale sono $y_1(t) = e^{r_{1}t}$ e $y_2(t) = e^{r_{2}t}$ .
3. Soluzione generale: La soluzione generale è una combinazione lineare delle soluzioni fondamentali:
$$
y(t) = C_{1}e^{r_{1}t} + C_{2}e^{r_{2}t}
$$
dove $C_1$ e $C_2$ sono costanti arbitrarie, determinate da eventuale condizioni iniziali o al contorno.

### Caso 2: $\Delta = 0$ (Delta uguale a 0)
1. Radici dell'equazione caratteristica: C'è una sola radice reale (o due radici reali coincidenti), $r$.
$$
r = \frac {b} {2a}
$$
2. Soluzione fondamentali: Una soluzione è $y_{1}(t) = e^{rt}$. La seconda soluzione linearmente indipendente si ottiene moltiplicando la prima per t, quindi $y_{2}(t) = xe^{rt}$.
3. Soluzione generale: La soluzione generale è una combinazione lineare di queste due:
$$
y(t) = C_{1}e^{rt} + tC_{2}e^{rt}
$$
che può anche essere scritta come:
$$
y(t) = (C_{1} + tC_{2})e^{rt}
$$
Anche qui $C_{1}$ e $C_2$ sono costanti arbitrarie.

### Caso 3: $\Delta < 0$ (Delta minore di 0)
1. Radici dell'equazione caratteristica: Ci sono due radici complesse coniugate, $r_{1,2} = a \pm i\beta$.
$$
r_{1,2} = \frac{ -b \pm \sqrt{ b^2 - 4ac } }{ 2a } = \frac{ -b \pm \sqrt{ -(b^2 - 4ac) } }{ 2a } = \frac{ -b \pm \sqrt{ | \Delta | } }{ 2a }
$$
Qui, $\alpha = -\frac {b} {2a}$ è la parte reale e $\beta = \frac {\sqrt{ |\Delta| }} {2a}$ è la parte immaginaria (si prende $\beta > 0$).
2. Soluzioni fondamentali: Usando la formula di Eulero ( $e^{i\theta} = \cos(\theta) + i \sin(\theta)$), si possono derivare due soluzioni reali e linearmente indipendenti: $y_{1}(t) = e^{\alpha t} \cos(\beta t)$ e $y_{2}(t) = e^{\alpha t} \sin(\beta t)$.
3. La soluzione generale: La soluzione generale è una combinazione lineare di queste:
$$
y(t) = e^{\alpha x}(C_{1} \cos (\beta t) + C_{2} \sin (\beta t))
$$
$C_1$ e $C_2$ sono costanti arbitrarie reali.


### Precedente
[[Introduzione equazioni differenziali.md]]