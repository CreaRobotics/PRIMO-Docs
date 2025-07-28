# Programmazione Avanzata del Robot PRIMO

---

## Cos’è RoboDK

**RoboDK** è un software di simulazione e programmazione offline per robot industriali. Permette di creare, simulare e ottimizzare percorsi di movimento in un ambiente virtuale prima di eseguirli sul robot reale. RoboDK supporta un'ampia varietà di robot e consente di generare codici di controllo personalizzati tramite post-processor, facilitando l’integrazione con sistemi hardware diversi.

---

## Come si importa un modello PRIMO

Per lavorare con PRIMO in RoboDK, è necessario importare il modello 3D del braccio robotico. Questo modello include la struttura meccanica e i riferimenti cinematici degli assi.

L’importazione avviene tipicamente attraverso un file CAD o un file di definizione robot compatibile con RoboDK (ad esempio file `.stp`, `.igs` o un modello RoboDK `.rdk`). Il modello viene caricato nell’ambiente di simulazione, permettendo di visualizzare e manipolare il robot in 3D.

---

## Come si simula un movimento e si esporta il codice

Una volta importato il modello PRIMO, si possono definire traiettorie e movimenti per il robot all’interno di RoboDK. Attraverso l’interfaccia grafica o utilizzando script, è possibile:

- Creare percorsi con punti intermedi
- Definire velocità e accelerazioni
- Simulare l’esecuzione della traiettoria per verificarne la correttezza e assenza di collisioni

Terminata la simulazione, RoboDK consente di esportare il codice di controllo specifico per PRIMO, adattato al suo firmware e hardware tramite un post-processor personalizzato. Questo codice è pronto per essere caricato e eseguito sul robot reale.

---

## Come funziona il post-processor personalizzato per PRIMO

Il **post-processor** è un componente software che traduce i movimenti e le istruzioni generati in RoboDK in un linguaggio di controllo comprensibile dal robot PRIMO.

Nel caso di PRIMO, il post-processor personalizzato converte le traiettorie in comandi compatibili con il controllo open-loop basato su motori passo-passo e invia istruzioni in forma di comandi passo-passo o G-code adattati al firmware usato.

Questo permette di garantire che il codice esportato sia ottimizzato per il funzionamento di PRIMO, rispettando i limiti meccanici, i parametri dei motori e la modalità di controllo open-loop.

---

*Questo documento fa parte della documentazione tecnica avanzata del braccio robotico educativo PRIMO.*
