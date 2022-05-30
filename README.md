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
- voglio poter recuperare le mie credenziali se le ho dimenticate.
    * Criteri di accettazione:
        + scenario: lutente vuole. invio di una mail di recupero (password) o modificare.
        + Precondizioni: L'utente a dimenticato la password.
        + Qando: clica il link per il recupero password e imette la mail con cui siera registrato.
        + Allora: Viene inviata una mail di recupero/ reset password (nuova password)
- da ogni pagina del sito voglio poter accedere alla pagina di login e/o di registrazione.<br>
    * Criteri di accettazione:
        + Scenario: l'utente vuole: poter accedere alla pagina di login e/o di registrazione da ogni pagina del sito.
        + Precondizioni: l'utente non si trova nella pagina di login o registrazione.
        + Qando: clica il link per accedere alla pagina di login/ registrazione.
        + Allora: Viene spostatto sulla pagina di login/ registrazione
- se sono già loggato, dallo stesso posto, voglio poter accedere alla mia pagina profilo.
    * Criteri di accettazione:
      +link al mio profilo da ogni paggina del sito
        + Precondizioni: lutente e gia logato
        + Qando: clica il link per accedere alla pagina profilo.
        + Allora: Viene spostatto sulla pagina profilo.
- voglio poter aggiungere un foto profilo
    * Criteri di accettazione:
        + scenario: lutente vuole. caricare una imagine sul suo profilo.
- voglio poter aggiungere informazioni al mio profilo
    * Criteri di accettazione:
        +
- voglio poter cancellare il mio account
    * Criteri di accettazione:
    + Precondizioni: lutente a gia un account
- voglio poter mettere a disposizione semi in mio possesso
    * Criteri di accettazione:
        + Scenario: l'utente loggato vuole caricare sul sito un seme da condividere
        + Precondizioni: l'utente loggato è sulla propria pagina di profilo del sito
        + Quando: l'utente clicca sul pulsante "Condividi i tuoi semi"
        + Allora: viene reindirizzato su una pagina che gli chiede il tipo di seme che vuole mettere a disposizione. L'utente inserisce il nome del seme, preme invio e verrà portato sulla pagina del seme appena caricato.
- voglio poter inserire informazioni riguardo ai semi che ho inserito
    * Criteri di accettazione:
        + Scenario: l'utente vuole inserire tutte le informazioni aggiuntive riguardanti i semi che ha inserito sul sito
        + Precondizioni: l'utente ha inserito il seme che voleva mettere a disposizione e si trova sulla pagina del seme
        + Quando: l'utente clicca sul pulsante "inserisci informazioni aggiuntive"
        + Allora: viene reindirizzato su una scheda che gli chiede di compilare i seguenti campi: "Quantità di semi", "Temperatura di conservazione", "Grandezza dei semi", "Foto dei semi", "Altre informazioni rilevanti". Compilati i campi che intende riempire, preme il pulsante invio e viene riportato sulla pagina del seme aggiornata.
- voglio poter chiedere la giacenza dei miei semi ad una banca
    * Criteri di accettazione:
        + Scenario: l'utente vuole richiedere a un utente banca di custodire nella sua banca i semi che ha inserito sul sito.
        + Precondizioni: l'utente loggato si trova sulla pagina di un utente banca
        + Quando: l'utente clicca sul pulsante "Richiedi giacenza presso questa banca"
        + Allora: viene reindirizzato su una pagina che gli chiede quali sono i semi che vorrebbe inviare alla banca. Seleziona i semi desiderati, preme invio e riceverà un messaggio a schermo con scritto "La tua richiesta di giacenza è stata inviata".
- voglio poter visualizzare la storia delle transazioni
    * Criteri di accettazione:
        + Scenario: l'utente vuole poter vedere tutte le transazioni avvenute sul sito
        + Precondizioni: l'utente loggato si trova su una qualsiasi pagina di un utente, di un utente banca o di un seme
        + Quando: l'utente clicca il pulsante in alto a sinistra "storico delle transazioni"
        + Allora: viene reindirizzato su una pagina in cui sono visibili tutte le transazioni di quello specifico utente, utente banca o del seme in ordine cronologico. Per le pagine utente, lo storico indicherà tutti i semi inviati e ricevuti (compresi i dati dell'inviante o del ricevente); per gli utenti banca, lo storico indicherà tutti i semi custoditi in passato e tutti i semi attualmente custoditi (compresi i dati degli utenti che li hanno inviati o prelevati); per i semi, lo storico indicherà tutti gli utenti che li hanno tenuti in ordine cronologico.
- voglio vedere il numero dei semi scambiati sul social
    * Criteri di accettazione:
        + Scenario: l'utente vuole vedere il numero dei semi scambiati sul social da ogni utente
        + Precondizioni: l'utente si trova sulla pagina di un qualsiasi altro utente
        + Quando: l'utente clicca sul pulsante ""
        + Allora:
- voglio poter tracciare i semi che mi sono stati inviati
    * Criteri di accettazione:
        + Scenario: l'utente vuole controllare a che punto della spedizione sono i semi che deve ricevere
        + Precondizioni: l'utente loggato si trova sulla pagina del proprio profilo personale
        + Quando: l'utente, nella sezione "Transazioni in corso", clicca sulla transazione interessata
        + Allora: viene reindirizzato su una pagina che indicherà se i semi: sono ancora in attesa di essere inviati, sono in viaggio, sono in procinto di arrivare.
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
