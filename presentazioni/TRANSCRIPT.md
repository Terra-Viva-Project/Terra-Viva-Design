# Slide 1 Presentazione
- Saluti 
- presentazione nome del progetto 
- nomi del team
# Slide 2 Cos'è
Terra Viva è un progetto che mira alla creazione di un social network rivolto principalmente ai seed saver.\
I seed saver sono delle persone che conservano e scambiano sementi di varietà antiche nell'ottica di preservare la biodiversità.\
Data l'importanza dell'attività svolta dai seed saver e sperando di dare il nostro contributo, abbiamo orientato il nostro lavoro 
alla creazione di un hub digitale di incontro per queste persone.
# Slide 3 Agile e Scrum
Il team ha lavorato con metodologie agile e in particolare ha implementato SCRUM.\
Scrum è un framework di sviluppo agile che permette di lavorare in maniera incrementale e iterativa.\
Una delle cerimonie centrali del nostro workflow è stato lo stand up meeting che ci ha permesso:
- di creare una relazione più forte tra i membri del team
- di conoscere lo stato di avanzamento del lavoro degli altri membri del team
- di risolvere piccoli problemi inerenti al lavoro del giorno precedente
# Slide 4 Trello
Uno degli strumenti di implementazione della metodologia Agile e del framework Scrum che abbiamo deciso di utilizzare è stato Trello.\
Questa è una foto della nostra bacheca, in cui si può vedere come le task sono assegnate e a che punto del loro svolgimento si trovano.
# Slide 5 GitHub
Per permetterci di lavorare in remoto sulla stessa codebase abbiamo utilizzato git e github.\
In particolare abbiamo implementato un flusso di lavoro chiamato github flow, tramite il quale abbiamo potuto lavorare separatamente sul codice 
per poi unire le modifiche effettuate sul branch master. 
Per assicurarci di introdurre il minor numero di bug nel ramo di rilascio, abbiamo sottoposto il merge delle modifiche alla review di almeno un altro membro del team.
Questo è un estratto del nostro github in cui si possono notare i merge delle varie pull request.
# Slide 6 Analisi Funzionale
Prima di stendere il codice abbiamo proceduto con una fase di progettazzione che ha portato alla scrittura delle user stories e allo sviluppo di ognuna di esse un una analisi funzionale
Pqui vediamo degli esempi di user stories a sinistra e analisi funzionale a destra.
Le parti costituenti dell'analisi funzionale sono:
- la descrizione della funzionalità presa in esame
- l'interazione che la funzionalità ha con eventuali altre funzionalità
- il workflow ovvero il processo attraverso il quale l'utenter fruisce la funzionalità o la risorsa
# Slide 7 wireframe
Sempre in fase di progettazione abbiamo creato un set di wireframe che rappresenti un bozza rudimentale dell'interfaccia con cui l'utente finale si trovera a interaggire.
Questo ci ha permesso di comprendere meglio quali fossero le necessità dell'utente finale.
# Slide 8 Stack tecnologico
Durante il corso in develhope abbiamo sviluppato il software backend per questo progetto.
Nella fase implementativa abbiamo utilizzato diverse tecnologie. In particolare le basi dell'ambiente di sviluppo sono state il linguaggio Java e il framework Spring.
Abbiamo deciso di utilizzare un database relazionale nello specifico MariaDB in quanto i valori con i quali viene sviluppato sono molto simili a i valori che supportano terra viva: partecipazione e cooperazione.
# Slide 9 Diagramma E/R
Prima di approcciarci alla scrittura del codice particolare attenzione è stata data alla modellazione del diagramma entità relazioni.
Qui possiamo vedere la struttura finale del diagramma E/R dalla quale siamo partiti per scrivere le entità e successivamente tutti gli strati che portano a rendere fruibili i nostri endpoint.
Abbiamo cercato di fare in modo che questo modello fosse il più aderente possibile alla realta rappresentata in modo che le modifiche successive al modello siano le minori possibili.
# ???????
# Slide 10
Oltre alla funzionalità core di spring (IOC contatiner, dependency injection)
abbiamo utilizzato altri moduli:
- Web
- DataJpa
- Validation

SpringSecurity è stato usato inizialmente per implementare le funzionalità di autenticatione e autorizzazione.
Successivamente abbiamo deciso di scrivere una nostra libreria per fare questo.
# Slide 11
Buds security è una libreria opensource che permette di intagrare in un progetto le funzionalità di autenticazione e autorizzazione.
La libreria è disponibile sui principali maven repository e abbiamo settato un piccola pipeline per il deploy automatico.
# Slide 12
Lo sviluppo dell'applicazione a seguito le specifiche endpoint che abbiuamo definito in fase di progettazione.
queste sono state poi implementate con swagger. è disponibile online una swagger ui che permette di interaggire con il sistema in modo da semplificare lo sviluppo frontend e da testare i singoli endpoint.

# Postman

