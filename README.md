# Progetto SeedShare
- [Progetto SeedShare](#progetto-seedshare)
    - [User Stories](#user-stories)
    - [Analisi Funzionale](#analisi-funzionale)
    - [Analisi Tecnica](#analisi-tecnica)
## User Stories
Io come **utente**:
- voglio potermi registrare
    * Criteri di accettazione:
        + Scenario: L'utente vuole effettuare la registrazione
        + Precondizioni: L'utente non loggato si trova su una qualsiasi pagina del sito
        + quando: l'utente clicca sul pulsante in alto a destra "Sign in/signup"
        + Allora: viene reindirizzato nella pagina di login e registrazione qui trova un pulsante con scritto "Registrati". Cliccato quel pulsante viene reindirizzato sulla pagina di registrazione. <br> riempiti tutti i campi puo premere su registrati. il sistema inviera un'e-mail di conferma all'utente. cliccando sul link di quella mail l'utente verrà reindirizzato sul sito e si troverà gia loggato.
- voglio potermi registrare grazie al mio account google
    * Criteri di accettazione:
        + Scenario: L'utente vuole effettuare la registrazione
        + Precondizioni: L'utente non loggato si trova su una qualsiasi pagina del sito
        + quando: l'utente clicca sul pulsante in alto a destra "Sign in/signup"
        + Allora: viene reindirizzato nella pagina di login e registrazione qui trova un pulsante che gli permette di registrarsi tramite google
- voglio poter effetuare il login
    * Criteri di accettazione:
        + Scenario: L'utente vuole effettuare il login
        + Precondizioni: L'utente non loggato si trova su una qualsiasi pagina del sito
        + quando: l'utente clicca sul pulsante in alto a destra "Sign in/signup"
        + Allora: viene reindirizzato nella pagina di login e registrazione dove trova dei campi da riempire con le proprie credenziali e un pulsante "login". Una volta cliccato su login se le credenziali sono giuste viene reindirizzato sulla sua pagina profilo, altrimenti gli vengono richieste di nuovo le credenziali.
- voglio poter navigare alcune parti del sito senza la necessita di registrarmi
    * Criteri di accettazione:
        + Scenario: l'utente vuole navigare sul sito senza essere registrato
        + Precondizioni: L'utente non loggato si trova su una qualsiasi pagina del sito
        + Qando: L'utente cerca di interagire con delle parti del sito che richiedono registrazione
        + Allora: Viene reindirizzato sulla pagina di "SignIn/SignOut" una volta loggato viene riportato sulla pagina che stava visitando.
-------------------
### Nicolò
- voglio poter recuperare le mie credenziali se le ho dimenticate.
- da ogni pagina del sito voglio poter accedere alla pagina di login e/o di registrazione.<br>
- se sono già loggato, dallo stesso posto, voglio poter accedere alla mia pagina profilo.
- voglio poter aggiungere un foto profilo
- voglio poter aggiungere informazioni al mio profilo
- voglio poter cancellare il mio account
### Andrea
- voglio poter mettere a disposizione semi in mio possesso
- voglio poter inserire informazioni riguardo ai semi che ho inserito
- voglio poter chiedere la giacenza dei miei semi ad una banca
- voglio poter visualizzare la storia delle transazioni
- voglio vedere il numero dei semi scambiati sul social
- voglio poter tracciare i semi che mi sono stati inviati
### Salvatore
- voglio poter contattare in una chat privata un altro utente
    * Criteri di accettazione:
        + Scenario: l'utente vuole contattare in privato un altro utente per chiedere informazioni
        + Precondizioni: l'utente deve essere registrato e loggarsi per poter utilizzare la chat
        + Quando: l'utente non è loggato e vuole aprire la chat, gli apparirà la finestra per il login
        + Allora: l'utente potrà accedere al profilo e successivamente mandare il messaggio, una volta inviato il messaggio al destinatario, a quest'ultimo apparirà una notifica
- voglio poter valutare il servizio
    * Criteri di accettazione:
        + Scenario: l'utente vuole valutare il servizio ricevuto con una valutazione che va da 1 a 5 stelle con l'aggiunta di una descrizione
        + Precondizioni: l'utente deve aver effettuato uno scambio,acquisto e/o cessione
        + Quando: la transizione sarà ufficialmente chiusa allora l'utente potrà esprimere un giudizio sul servizio ottenuto
        + Allora: il giudizio inficerà sulla graduatoria di gradimento dell'altro utente facente parte della transizione che è visibile a tutti nel suo profilo
- che ha conservato dei semi in banca vorrei poterli ritirare
    * Criteri di accettazione:
        + Scenario: l'utente vuole ritirare dei semi dalla banca
        + Precondizioni: l'utente deve aver già depositato dei semi in banca per poterli ritirare successivamente
        + Quando: l'utente andrà a ritirare dei semi dalla banca, ad esso verranno chieste tutte le credenziali di sicurezza e dei certificati di proprietà
        + Allora: una volta accertato che l'utente sia il vero possessore dei semi richiesti, ad esso verrà rilasciata la quantità richiesta dei semi richiesti
- vorrei poter richiedere dei semi da una banca
    * Criteri di accettazione
        + Scenario: l'utente ha bisogno di semi che non possiede
        + Precondizioni: l'utente che chiede dei semi ad una banca deve essere già registrato e deve poter fare un colloquio con dei dirigenti della banca che verificheranno se l'utente può o sarà in grado di pagare i semi richiesti
        + Quando: le condizioni saranno soddisfatte e accertate
        + Allora: verranno rilasciati all'utente i semi richiesti
- vorrei poter allegare ai semi delle informazioni legate ai semi che sto spedendo
    * Criteri di accettazione:
        + Scenario: l'utente deve spedire i semi richiesti da un altro utente per completare la transizione
        + Precondizioni: i due utenti devono mettersi d'accordo su quantità,pagamento e spedizione dei semi
        + Quando: l'accordo verrà raggiunto e l'utente che deve spedire i semi preparerà il pacco
        + Allora: esso potrà allegare ai semi delle informazioni utili alla coltivazione e al loro utilizzo migliore
- vorrei poter proporre un scambio di semi
    * Criteri di accettazione:
        + Scenario: un utente possiede già dei semi e vorrebbe averne altri che al momento non ha oppure ne ha scarsa disponibilità
        + Precondizioni: l'utente deve essere già registrato e loggato cosi da poter contattare un altro utente che potrebbe soddisfare la sua richiesta
        + Quando: l'utente che vuole effettuare lo scambio ne trova un altro che ne accetta i termini e le condizioni
        + Allora: entrambi possono mettersi d'accordo sulla modalità di scambio

io come **utente banca dei semi** voglio:
- voglio poter accettare dei semi e custodirli per un utente
- voglio poter richiedere un pagamento per la custodia dei semi
- voglio poter mettere un ranking ai semi

------------

## Analisi Funzionale
descrizione della funzionalità
descrizione dell'interazione di questa funzionalità con altre funzionalità
workflow della funzionalità (flussi di lavoro)

## Analisi Tecnica