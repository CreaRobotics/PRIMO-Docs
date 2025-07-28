# Componenti principali di PRIMO

PRIMO è un braccio robotico articolato progettato per introdurre alla robotica industriale in modo pratico e accessibile. Ogni componente che lo costituisce ha un ruolo funzionale ben preciso, pensato per simulare il comportamento di veri robot industriali.

## Struttura generale

Il robot è composto da sei assi rotazionali, ognuno dei quali permette un movimento controllato. Questi assi sono realizzati attraverso una combinazione di:

- **Motori passo-passo**
- **Giunti meccanici**
- **Supporti e snodi**
- **Elementi strutturali stampati in 3D**

Ogni asse introduce un grado di libertà (DoF), permettendo movimenti indipendenti che, combinati, danno vita a una cinematica articolata.

---

## Motori passo-passo

I motori utilizzati sono chiamati **NEMA 17**. Sono motori in grado di ruotare di piccoli passi precisi (es. 1.8° per passo), rendendoli ideali per la robotica educativa. Non utilizzano sensori di posizione (open-loop), ma possono essere controllati con alta precisione tramite appositi driver.

### Come contribuiscono

Ogni motore è responsabile della rotazione di un segmento del braccio robotico. La combinazione di più rotazioni consente al braccio di orientarsi nello spazio.

---

## Giunti rotazionali

I giunti permettono il movimento relativo tra due parti del braccio. Sono il cuore della struttura articolata e simulano le articolazioni di un braccio umano (es. spalla, gomito, polso).

### Come contribuiscono

Senza i giunti, le rotazioni dei motori non avrebbero alcun effetto: è grazie ai giunti che i segmenti del braccio possono muoversi in modo coordinato.

---

## Supporti e snodi

Gli snodi sono elementi meccanici che collegano tra loro motori, giunti e bracci. Possono contenere cuscinetti per rendere fluido il movimento e garantire stabilità.

---

## Controller e driver

Il controllo dei motori avviene tramite una scheda centrale, a cui i motori sono collegati. In PRIMO, i driver sono in **open-loop**, ovvero senza retroazione: il sistema invia comandi ai motori ma non verifica se il movimento è stato realmente eseguito.

### Che cosa permette questa configurazione?

- Riduzione dei costi
- Maggiore semplicità didattica
- Possibilità di esplorare limiti e potenzialità del controllo senza feedback

---

## In sintesi

Ogni componente di PRIMO è stato progettato per simulare i concetti fondamentali della robotica industriale:

| Componente        | Funzione                                  |
|-------------------|--------------------------------------------|
| Motore passo-passo| Genera il movimento rotazionale            |
| Giunto            | Trasmette e permette la rotazione          |
| Supporto/snodo    | Collega e guida i movimenti                |
| Controller        | Invia comandi ai motori (open-loop)        |

> Lo scopo non è solo vedere PRIMO muoversi, ma capire **come e perché** ogni parte contribuisce al movimento complessivo del robot.
