# Programmazione Base del Robot PRIMO

---

## Cos'è il G-code

Il **G-code** è un linguaggio di programmazione standard utilizzato per controllare macchine CNC, stampanti 3D e robot industriali. Consiste in una serie di comandi testuali che indicano movimenti, velocità, posizioni e altre azioni da eseguire. Ogni comando in G-code specifica istruzioni precise come spostare un asse, cambiare velocità o attivare/disattivare un utensile.

Utilizzando il G-code è possibile definire traiettorie e sequenze di movimento per il robot in modo semplice e flessibile.

---

## Come si controlla manualmente PRIMO

Il controllo manuale di PRIMO permette di spostare singolarmente gli assi del robot per operazioni di prova, calibrazione o posizionamento preciso. Questo controllo diretto viene effettuato inviando comandi che indicano lo spostamento di un singolo asse di una certa quantità o angolo.

Attraverso un'interfaccia di controllo, è possibile scegliere quale asse muovere e definire il numero di passi o la distanza da percorrere, controllando così manualmente la posizione del robot.

---

## Come si possono dare comandi da una console o interfaccia web

Il robot PRIMO può ricevere comandi da una console di controllo o da un’interfaccia web dedicata. Questi strumenti consentono di inviare comandi testuali (come quelli in G-code) direttamente al sistema di controllo, visualizzare lo stato del robot e monitorare l'esecuzione dei movimenti.

La console e l’interfaccia web permettono anche di eseguire macro, caricare file di programma e inviare istruzioni di movimento in tempo reale, facilitando così l’interazione con il robot.

---

## Esempi di G-code semplici per muovere gli assi

Ecco alcuni esempi base di comandi per muovere gli assi del robot:

- **Spostamento rotativo su un asse (esempio: asse B):**

G1 B10 F1000

Questo comando sposta l'asse B a 10 gradi con una velocità di 1000 gradi/minuto.

- **Spostamento contemporaneo di più assi (esempio: X e Y):**

G1 X20 Y15 F800

Sposta gli assi X e Y rispettivamente a 20 e 15 gradi con velocità 800.

- **Ritorno alla posizione zero (home):**

G28

Comando per riportare tutti gli assi alla posizione di origine.

- **Spostamento relativo (rispetto alla posizione corrente):**

G91
G1 X5 Y-3 F500
G90

Qui il robot si sposta di +5 sull'asse X e -3 sull'asse Y rispetto alla posizione attuale. `G91` abilita il modo di spostamento relativo, mentre `G90` lo disabilita tornando al modo assoluto.

---

*Questa guida fa parte della documentazione tecnica del braccio robotico educativo PRIMO.*
