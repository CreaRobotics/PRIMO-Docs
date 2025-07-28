# Controllo del Robot PRIMO

## Differenza tra controllo Open-Loop e Closed-Loop

Il **controllo open-loop** è un metodo in cui il sistema esegue comandi senza ricevere alcun feedback sulla posizione o lo stato reale degli attuatori. Il controllo si basa esclusivamente sull’invio di istruzioni, presupponendo che l’azione venga eseguita correttamente. Questo tipo di controllo è semplice e meno costoso, ma può essere soggetto a errori non rilevati come perdite di passi o scostamenti di posizione.

Il **controllo closed-loop** utilizza un sistema di retroazione che misura continuamente la posizione o lo stato effettivo dell’attuatore tramite sensori. Il sistema confronta il valore misurato con il valore desiderato e apporta correzioni per minimizzare gli errori, garantendo una maggiore precisione e affidabilità del movimento.

---

## Perché PRIMO è Open-Loop

PRIMO utilizza un controllo open-loop perché impiega motori passo-passo senza sensori di retroazione. Questa scelta permette di mantenere il progetto semplice, economico e facilmente accessibile a chi si avvicina alla robotica educativa. La semplicità hardware e software facilita l’apprendimento dei principi base del controllo dei robot senza la complessità aggiuntiva del feedback.

Inoltre, per applicazioni didattiche con carichi leggeri e velocità moderate, il controllo open-loop è sufficiente per ottenere movimenti precisi e affidabili.

---

## Come Avviene il Movimento dei Motori Passo-Passo

I motori passo-passo sono motori elettrici che si muovono a scatti discreti chiamati “passi”. Ogni impulso elettrico ricevuto fa ruotare l’albero del motore di un angolo fisso. La posizione è quindi controllata contando il numero di impulsi inviati al motore.

Il movimento complessivo del motore è ottenuto sommando questi passi, permettendo un controllo accurato della posizione senza necessità di sensori esterni.

---

## Come PRIMO Riceve ed Esegue i Comandi di Movimento

Il sistema di controllo interpreta le istruzioni di movimento e le traduce in impulsi elettrici inviati ai motori passo-passo. Questi impulsi indicano quanti passi ciascun motore deve compiere e con quale velocità.

L’esecuzione avviene in open-loop: si presume che il motore compia esattamente il numero di passi comandati senza una verifica attiva della posizione raggiunta. Questo metodo è efficace in condizioni controllate e permette una programmazione semplice e diretta del movimento del robot.

---

*Questo documento fa parte della documentazione tecnica del braccio robotico educativo PRIMO.*
