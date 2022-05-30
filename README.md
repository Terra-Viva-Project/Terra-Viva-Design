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
- voglio poter valutare il servizio
- che ha conservato dei semi in banca vorrei poterli ritirare
- vorrei poter richiedere dei semi da una banca
- vorrei poter allegare ai semi delle informazioni legate ai semi che sto spedendo
- vorrei poter proporre un scambio di semi

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