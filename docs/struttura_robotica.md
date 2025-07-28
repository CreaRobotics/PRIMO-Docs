# Struttura Robotica

## Cosa sono gli assi e i gradi di libertà

Un **robot** si muove nello spazio grazie a una serie di **assi**, cioè snodi o giunti che gli permettono di ruotare o traslare. Ogni asse aggiunge un **grado di libertà (DoF, Degree of Freedom)**, cioè una direzione possibile di movimento.

Un corpo nello spazio può avere fino a **6 gradi di libertà**:

- 3 di **traslazione**: avanti/indietro, sinistra/destra, su/giù.
- 3 di **rotazione**: rollio, beccheggio, imbardata.

Un robot con **6 assi** può quindi raggiungere qualsiasi posizione e orientamento nello spazio tridimensionale, proprio come il braccio di un essere umano.

---

## Cinematica diretta e cinematica inversa

La **cinematica** studia il movimento dei corpi, senza preoccuparsi delle forze.

- **Cinematica diretta**: si conoscono gli angoli dei giunti → si calcola dove si trova l’estremità del braccio (end-effector).
- **Cinematica inversa**: si conosce la posizione desiderata dell’estremità → si calcolano gli angoli da dare ai giunti.

La cinematica inversa è particolarmente importante: ci permette di dire al robot *"Vai lì"* e il robot calcola come muoversi.

---

## Che struttura ha PRIMO

PRIMO è un **braccio robotico a 6 assi**, ovvero un **manipolatore articolato** che ricorda il braccio umano. È composto da:

1. **Base** – ruota il braccio orizzontalmente
2. **Spalla** – alza e abbassa il braccio
3. **Gomito** – estende o ritrae il braccio
4. **Polso 1** – piega verso l'alto o il basso
5. **Polso 2** – ruota lateralmente
6. **Polso 3** – ruota sull'asse dell'end-effector

Questa struttura è molto diffusa nell'industria, perché permette di raggiungere molti punti nello spazio con grande flessibilità.

---

## Cinematica a catena aperta (visiva)

PRIMO ha una **struttura a catena aperta**: ogni giunto è collegato al successivo in sequenza, come i segmenti di un braccio umano.

