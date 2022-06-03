# Progetto SeedShare
# Table of contents
- [Progetto SeedShare](#progetto-seedshare)
    - [Analisi Funzionalità core](#analisi-funzionalit-core)
    - [Analisi Funzionalità](#analisi-funzionalit)
# Salvatore
## Analisi Funzionalità core
### Funzionalità di registrazione
#### Descrizione
Questa funzionalità garantisce all'utente la possibilità di registrare un proprio account in modo da poter interagire con il social.
#### Interazione con altre funzionalità
Questa funzionalità ha interazioni con la funzionalità di login
#### Workflof della funzionalità
l'utente non loggato da ogni pagine del sito avrà la possibilità di accedere alla pagina di sign-in sign-up.
un volta reindirizzato su questa pagina l'utente cliccherà sul pulsante registrati e compilerà i form che li si presentano.
una volta completato l'inserimento l'utente cliccherà sul pulsante registrami e riceverà una mail di conferma.
una volta cliccato sul link nella mail l'utente verrà reindirizzato sulla sua pagina profilo.
# Gianluigi
### Funzionalità di log-in
#### Descrizione
Questa funzionalità deve poter consentire all'utente di effettuare l'accesso nel sistema con le proprie credenziali
#### Interazione con altre funzionalità
interagisce con la funzionalità di login in quanto un utente gia loggato non puo rieffettuare il login prima di essersi sloggato
#### Workflof della funzionalità
da utente sloggato viene sempre garantito in ogni pagina del sito l'accesso alla funzionalità di sign-in sign up.\
una volta cliccato sul link l'utente verrà reindirizzato su una pagina che gli consente di effettuare il login o la registrazione\
per effettuare il login dovrà inserire delle credenziali valide negli appositi form e cliccare sul tasto login.
### Funzionalità navigazione nell'albero delle specie
#### Descrizione
questa funzionalità deve poter garantire all'utente la navigazione dell'albero delle specie botaniche presenti nel database.
#### Interazione con altre funzionalità
L'utente può essere loggato o meno per accedere a questa funzionalità.
#### Workflof della funzionalità
A questa funzionalità sarà possibile accedere attraverso un link nel menù laterale.
Essendo questa navigazione legata strettamente alla struttura dei dati vogliomo poter definire meglio questa funzionalità in seguito.
### Funzionalità di aggiunta e modifica di una specie
#### Descrizione
Questa funzionalità deve garantire agli utenti admin di poter inserire o modificare delle specie nel database
#### Interazione con altre funzionalità
l'utente deve essere loggato nel sito e il tipo di utente deve essere admin
#### Workflof della funzionalità
una volta loggato l'utente admin nel menu avrà un link alla pagina di gestione delle specie.
entrato in questa pagina saranno visualizzate tutte le specie.
sulla pagina sara presente un tasto aggiungi che permettera di essere indirizzati alla pagina di aggiunta di una specia
cliccando su una di esse sara possibile accedere alla pagina di modifica della stessa.
### Funzionalità di ricerca di globale
#### Descrizione
La funzionalità di ricerca permette di ricercare all'interno del social dei tag specifici, degli utenti o dei semi.
#### Interazione con altre funzionalità
Può essere fatta la ricerca anche da utenti non loggati.
#### Workflof della funzionalità
per accedere a questa funzionalità è sempre disponibile sulla barra superiore del sito un campo di testo che permette l'immissione del testo da ricercare.
una volta inserito il testo e premuto invio si viene reindirizzati su un altra pagina in cu queste informazioni sono suddivise su dei tab (utenti, semi, tag).
- nel tab dei tag vengono mostrati tutti i tag correlati al testo inserito nella barra di ricerca.
- nel tab persone vengono mostrati tutte le persone correlate al testo inserito nella barra di ricerca.
- nel tab semi vengono mostrate le varietà e le specie di semi corrispondenti al testo inserito nella barra di ricerca.
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
### Contattare un utente
#### Descrizione
La funzionalità di contattare un utente permette a chi è registrato di messaggiare con altri utenti registrati per effettuare delle transizioni.
#### Interazione con altre funzionalità
Questo tipo di funzionalità può essere usata soltanto se la registrazione è stata effettuata e quindi essere in possesso di un proprio profilo. <br> Inoltre per messaggiare con un utente si possono utilizzare anche altre funzionalità come quella della ricerca globale, usata anche per cercare utenti da messaggiare.
#### Workflow della funzionalità
Per inviare un messaggio bisogna prima individuare l'utente con cui farlo, questo è possibile tramite la ricerca globale in cui bisogna inserire del testo che permette di visualizzare il nome degli utenti che più si avvicinano ad esso. <br>
Una volta trovavo l'utente da contattare, si clicca sul nome per aprire la sua pagina profilo in cui si trova il tasto che una volta premuto farà aprire una pagina interamente dedicata alla messaggistica con l'altro utente.
### Lettura dei feed
#### Descrizione
Questa funzionalità permette di leggere i post relativi agli utenti o ai tag seguiti.
#### Interazione con altre funzionalità
Questa funzionalità interagisce con la funzionalità "seguire un tag" e "seguire un seed saver"
#### Workflof della funzionalità
l'utente loggato dal menu laterale attraverso la voce di menù feed accederà ad una pagina che gli permetterà di visualizzare tutti i post relativi ai tag o agli utenti che segue.
### Funzionalità di messaggistica
#### Descrizione
Questa funzionalità permette agli utenti di inviare e ricevere messaggi con gli altri utenti
#### Interazione con altre funzionalità
questa funzionalita interagisce con la funzionalità di login
#### Workflof della funzionalità
sul menu laterale l'utente troverà un lik alla pagina messaggi.\
Una volta reindirizzato sulla pagina dei messaggi l'utente visualizzerà sulla sinistra una lista di tutte le conversazioni gia avviate.\
sulla destra visualizzerà i messaggi relativi alla conversazione avviata. in basso avra un campo di testo dove potra inserire il messagio da inviare e potrà inviarlo cliccando sul pulsante invia.
### Funzionalità di visualizzazione di una varità
#### Descrizione
Questa funzionalità permette a qualsiasi utente di vedere i dati di una specie di semi presenti sul sito.
#### Interazione con altre funzionalità
Sia gli utenti registrati che quelli non registrati possono usufruire di questa funzionalità.
La visualizzazione di una specie è legata all'utilizzo della funzione di ricerca globale, da cui si cerca la specie interessata.
#### Workflof della funzionalità
Per visualizzare una specie di semi è necessario cliccare sulla barra di ricerca globale, accessibile da qualsiasi pagina del sito sia dall'utente loggato sia da quello sloggato.
Sulla barra bisogna scrivere il nome della specie che ci interessa. A quel punto cliccheremo sul tab dei semi, in modo da vedere solo i risultati della ricerca inerenti le specie e le varietà. Ora scorreremo tra i risultati finchè non troveremo la specie interessata, su cui cliccheremo. Questo ci porterà sulla pagina di quella specie, che si presenterà con una foto raffigurante quella specie in alto a sinistra con affianco la sua descrizione e tutte le informazioni necessarie. Più in basso sarà invece possibile osservare dei riquadri con tutte le varietà presenti sul sito di quella specie.
# Nicolò
### Visualizzare la varietà
#### Descrizione
#### Interazione con altre funzionalità
#### Workflof della funzionalità
### Richiedere una varietà
#### Descrizione
Richiedere un seme ad un utente
#### Interazione con altre funzionalità
#### Workflof della funzionalità
### Funzionalità di aggiunta di una varietà
#### Descrizione
#### Interazione con altre funzionalità
#### Workflof della funzionalità
### Visualizzare la specie
#### Descrizione
## Analisi Funzionalità
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
### Funzionalità di seguire un utente (cuoricino sulla pagina profilo e/o cuoricino appena scrivo utente)
#### Descrizione
Questo tipo di funzionalità ci permette di seguire gli utenti a cui siamo più fedeli o semplicemente che ci interessano di più.
#### Interazione con altre funzionalità
Per eseguire questa funzionalità bisogna essere registrati e essere in possesso di un proprio account. <br> Per poter seguire un profilo è possibile utilizzare la ricerca globale per trovare l'account desiderato e successivamente premere il cuore posto accanto al nome utente.
#### Workflow della funzionalità
Per seguire un utente bisogna premere sul cuoricino posto accanto al suo nome profilo, quest'azione può essere effettuata in qualsiasi contesto del sito come ad esempio nella pagina home, nelle ricerche e anche dai messaggi. <br> Questo è possibile perchè il cuore si troverà sempre nella stessa posizione indifferentemente dal modo in cui si visualizza il nome profilo. <br> Quando il cuore viene cliccato, e di conseguenza esso si colora interamente di rosso, vuol dire che stiamo seguendo l'utente e da questo momento in poi è possibile vedere i suoi post nella pagina "seguiti".
### Vedere chi seguiamo e da chi siamo seguiti
#### Descrizione
Questa funzionalità permette all'utente di controllare chi segue e da chi è seguito.
#### Interazione con altre funzionalità
Per poter effettuare questo tipo di operazione bisogna essere registrati e avere un proprio profilo.
#### Workflow della funzionalità
Per controllare i follower e i seguiti bisogna cliccare sulla foto in alto a destra in modo da aprire la pagina dedicata al proprio profilo. <br> Da qui è possibile cliccare sul tasto posto in basso "persone che segui" e comparirà una lista formata da tutte le persone che l'utente segue fino a quel momento. <br> Per quanto riguarda invece la possibilità di controllare chi è che ci segue, bisogna cliccare sul tasto posto in basso "persone che ti seguono" in modo tale da aprire la lista di tutti gli utenti che ci seguono fino a quel momento. <br>
# Andrea
### Vedere la cronologia di transazioni e scambi
#### Descrizione
Questa funzionalità permette all'utente di vedere la storia delle sue transazioni rispetto alla banca dei semi.
#### Interazione con altre funzionalità
Questa funzionalità interagisce con la funzionalità di logi in quanto l'utente deve essere necessariamente loggato.
#### Workflof della funzionalità
una volta effettuato il login l'utente va sulla propria pagina profilo e li trova una lista di tutte le sue transazioni rispetto ai semi.

