# Progetto SeedShare
- [Progetto SeedShare](#progetto-seedshare)
    - [User Stories](#user-stories)
    - [Analisi Funzionale](#analisi-funzionale)
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
### Funzionalità di ricerca di globale
#### Descrizione
La funzionalità di ricerca permette di ricercare all'interno del social dei tag specifici, degli utenti o dei semi.
#### Interazione con altre funzionalità
Può essere fatta la ricerca anche da utenti non loggati.
#### Workflof della funzionalità
per accedere a questa funzionalità è sempre disponibile sulla barra superiore del sito un campo doi testo che permette l'immissione del testo da ricercare.
una volta inserito il testo e premuto invio si viene reindirizzati su un altra pagina in cu queste informazioni sono suddivise su dei tab (utenti, semi, tag).
- nel tab dei tag vengono mostrati tutti i tag correlati al testo inserito nella barra di ricerca.
- nel tab persone vengono mostrati tutte le persone correlate al testo inserito nella barra di ricerca.
- nel tab semi vengono mostrate le varietà e le specie di semi corrispondenti al testo inserito nella barra di ricerca.
### Funzionalità di gestione della banca dei semi (TODO)
#### Descrizione
#### Interazione con altre funzionalità
#### Workflof della funzionalità
#Andrea
### Funzionalità di aggiunta di un post
#### Descrizione
La funzionalità di aggiunta di un post permette all'utente, solo se loggato, di aggiungere sul sito un post riguardante uno o più argomenti, specificati dai tag che andranno obbligatoriamente inseriti nel post.
#### Interazione con altre funzionalità
L'aggiunta di un post potrà essere effettuata esclusivamente da utenti loggati. 
L'inserimento di un post andrà ad interagire con la funzionalità di ricerca globale e con la ricerca post tramite filtri tag.
Quando un post verrà inserito infatti, potrà essere visto da tutti sia attraverso la ricerca globale, sia attraverso la ricerca tramite filtri tag, purchè nel post sia inerito un tag selezionato nella ricerca.
#### Workflof della funzionalità
Per accedere a questa funzionalità sarà necessario andare sulla pagina "Home" del sito e cliccare sulla barra al centro della pagina con scritto "Nuovo post".
Una volta cliccato sulla barra, si aprirà una scheda che ci permetterà di scrivere il post che vogliamo aggiungere.
Una volta scritto il testo e inserito uno o più tag, basterà premere il tasto invio per pubblicare il post. Da questo momento il nostro post sarà visibile a tutti. 
### Funzionalità di ricerca post tramite filtri tag
#### Descrizione
Questa funzionalità permette agli utenti di visualizzare tutti i post inerenti degli specifici tag; questi tag saranno selezionati dall'utente che sta facendo la ricerca.
#### Interazione con altre funzionalità
La ricerca può essere effettuata anche da utenti non loggati.
Questa funzionalità interagisce con l'inserimento di nuovi post: quando un nuovo post viene pubblicato sul sito infatti, questo verrà aggiunto alla lista dei post visualizzabili con quello o quei specifici tag.
#### Workflof della funzionalità
Per accedere a questa funzionalità bisogna andare nella parte superiore della schermata Home e selezionare i tag che ci interessano. Per farlo potremo sia cliccare sopra le nuvolette contenenti i tag a cui siamo interessati che vediamo a schermo, sia cliccare sulla barra di ricerca dove possiamo ricerca uno specifico tag.
Una volta selezionati i tag interessati, questi si sposteranno sul riquadro dove si trova la barra di ricerca, in modo da poter vedere quali sono i tag che stiamo filtrando in quel momento.
A questo punto nella parte inferiore della schermata Home potremo vedere tutti i post in ordine cronologico, dal più recente al più vecchio, contenenti i tag selezionati.
### Funzionalità di aggiunta, aggiornameto e rimozione foto profilo
#### Descrizione
Questa funzionalità consente all'utente registrato sul sito di inserire una foto sul proprio profilo e successivamente di modificarla o rimuoverla.
#### Interazione con altre funzionalità
Per inserire una foto profilo è necessario essere loggati.
L'aggiunta di una foto profilo interagisce con lo scambio di messaggi tra utenti, poichè, se inserita, sarà visualizzabile affianco al nome dell'utente durante lo scambio di messaggi.
#### Workflof della funzionalità
Per utilizzare questa funzionalità sarà necessario che l'utente, dopo essersi loggato, vada sulla pagina del suo profilo. Lì potrà cliccare sul riquadro in alto a sinistra della pagina con scritto "Carica una foto profilo". Cliccando si aprirà una finestra che gli chiederà di selezionare, all'interno delle cartelle del PC, una foto da inserire.
Se l'utente ha inserito una foto profilo, passando con il cursore sopra di essa, vedrà apparire in alto a destra della foto due piccoli simboli, raffiguranti una matita e una X. 
Andando, sempre con il cursore, sopra la matita, apparirà la scritta "Modifica foto profilo". Cliccando sulla matita, si aprirà nuovamente la finestra di inserimento foto e sarà possibile selezionare una nuova foto.
Andando invece sopra la X, apparirà la scritta "Cancella foto profilo". Cliccando sulla X la foto sarà rimossa e vedremo nuovamente il riquadro vuoto con scritto "Carica una foto profilo".
### Funzionalità di inserimento e modifica dei dati personali
#### Descrizione
Questa funzionalità permette all'utente loggato sul sito di inserire e modificare nel proprio profilo una serie di dati personali quali nome, cognome, data di nascita, luogo di nascita e di residenza.
#### Interazione con altre funzionalità
Per inserire i dati personali e modificarli l'utente deve essere registrato.
La ricerca globale interagisce con questa funzionalità; quando un utente cerca una persona infatti, se quest'ultima avrà inserito dei dati personali allora questi ultimi saranno visibili sul suo profilo. 
#### Workflof della funzionalità
Per inserire dei dati personali l'utente dovrà essere loggato e trovarsi sulla pagina del proprio profilo. Nell'area in alto al centro della pagina troverà: una barra dove gli sarà possibile inserire il proprio nome, una barra dove inserire il proprio cognome, una barra dove inserire la propria data di nascita, una barra dove inserire il proprio luogo di nascita, una barra dove inserire il proprio luogo di residenza e una barra dove poter inserire qualsiasi informazione aggiuntiva.
Per modificare i dati sarà necessario semplicemente tornare sulla barra del dato che si desidera ed effettuare le modifiche.
#Salvatore
### Contattare un utente
#### Descrizione
#### Interazione con altre funzionalità
#### Workflof della funzionalità
### Funzionalità di seguire un utente (cuoricino sulla pagina profilo e/o cuoricino appena scrivo utente)
#### Descrizione
#### Interazione con altre funzionalità
#### Workflof della funzionalità
### Vedere chi seguiamo e da chi siamo seguiti
#### Descrizione
#### Interazione con altre funzionalità
#### Workflof della funzionalità
#Gianluigi
### Vedere la cronologia di transazioni e scambi
#### Descrizione
#### Interazione con altre funzionalità
#### Workflof della funzionalità
### Lettura dei feed
#### Descrizione
#### Interazione con altre funzionalità
#### Workflof della funzionalità
### Poter messaggiare
#### Descrizione
#### Interazione con altre funzionalità
#### Workflof della funzionalità
#Nicolo
### Visualizzare la specie
#### Descrizione
Questa funzionalità permette a qualsiasi utente di vedere i dati di una specie di semi presenti sul sito.
#### Interazione con altre funzionalità
Sia gli utenti registrati che quelli non registrati possono usufruire di questa funzionalità.
La visualizzazione di una specie è legata all'utilizzo della funzione di ricerca globale, da cui si cerca la specie interessata.
#### Workflof della funzionalità
Per visualizzare una specie di semi è necessario cliccare sulla barra di ricerca globale, accessibile da qualsiasi pagina del sito sia dall'utente loggato sia da quello sloggato.
Sulla barra bisogna scrivere il nome della specie che ci interessa. A quel punto cliccheremo sul tab dei semi, in modo da vedere solo i risultati della ricerca inerenti le specie e le varietà. Ora scorreremo tra i risultati finchè non troveremo la specie interessata, su cui cliccheremo. Questo ci porterà sulla pagina di quella specie, che si presenterà con una foto raffigurante quella specie in alto a sinistra con affianco la sua descrizione e tutte le informazioni necessarie. Più in basso sarà invece possibile osservare dei riquadri con tutte le varietà presenti sul sito di quella specie.
### Visualizzare la varietà
#### Descrizione
#### Interazione con altre funzionalità
#### Workflof della funzionalità
### Richiedere una varietà
#### Descrizione
#### Interazione con altre funzionalità
#### Workflof della funzionalità
