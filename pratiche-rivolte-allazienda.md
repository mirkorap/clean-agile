# Pratiche rivolte all'azienda

Vi è un insieme di pratiche, rivolte verso la società esterna, che gli sviluppatori devono seguire per avere successo.

### Pianificazione

Una delle attività più difficile nella programmazione è la stima dei tempi. Il consiglio che spesso viene dato è quello di suddividere il progetto in elementi più piccoli così da consentire una stima accurata. Ma quanto devono essere piccoli questi elementi? In questo processo dobbiamo tener conto che più piccolo è l'elemento e più facile sarà da stimare, ma, al contempo, maggiore sarà il costo del processo di stima in quanto, suddividere il progetto in piccoli elementi, porterà via parecchio tempo. Una stima, per definizione, è un'ipotesi. Pertanto non può mai essere precisa. L'imprecisione ci consente di ridurre il tempo necessario per creare la stima. Maggiore è l'imprecisione, minore sarà il tempo necessario per calcolarla. Le stime dovrebbero essere il più possibile accurate, ma solo quanto basta a mantenere basso il costo del processo di stima.

### Analisi trivariata (PERT)

Una tecnica che funziona piuttosto bene per attività di grandi dimensioni è la **stima trivariata**. Tali stime sono composte da tre numeri: **caso migliore, caso nominale e caso peggiore**. Il numero del **caso peggiore** rappresenta il tempo entro il quale ci si sente sicuri al 95% che l'attività venga completata. Il **caso nominale** ha solo un 50% di sicurezza e il **caso migliore** solo del 5%. Questo tipo di analisi può essere utile per stimare elementi di grandi dimensioni, per la gestione quotidiana di un progetto abbiamo bisogno di un altro metodo.

### Storie e punti

La tecnica degli **story point** si prende carico della precisione impiegando un ciclo di feedback molto stretto. Inizialmente, l'imprecisione sarà elevata, ma entro alcuni cicli essa si riduce a livelli accettabili. Prima di parlare degli story point, occorre introdurre la definizione di **user story**. Una user story è una descrizione abbreviata di una funzionalità, raccontata dal punto di vista dell'utente:

> Come conducente di un'automobile, se voglio incrementare la velocità, premo di più il pedale dell'acceleratore.

Questa breve descrizione ci deve dare solo un'idea di cosa dovrà fare la funzionalità, i dettagli di come dovrà funzionare verranno discussi e rimandati nel momento in cui verrà scelta questa storia.

#### Storie per uno sportello automatico

Immaginate di essere alla iterazione zero in un team che deve scrivere le storie per uno sportello automatico. Le prime storie che vengono in mente potrebbero essere queste cinque: Login, Logout, Prelievo, Versamento e Bonifico. Nel meeting in cui si è parlato di queste storie saranno venuti fuori molti altri dettagli che possiamo annotare all'interno delle storie, ma, per il momento, non occorre che vengono snocciolati più di tanto. Rimandiamo questa operazione di dettagliare le storie nel momento in cui verranno scelte. È importante resistere all'impulso di dettagliare le storie adesso, in quanto ci ritornerete sicuramente quando verranno scelte e questo vi farà perdere due volte del tempo. Le storie devono partire senza troppo impegno, perché molte di esse verranno modificate, divise, unite o perfino eliminate. Il processo di creazione delle storie non termina mai. Le storie vengono continuamente scritte e modificate nel corso del progetto.

#### Stimare le storie

Una volta definito un gruppo di storie, possiamo procedere alla loro stima. Viene pescata dalla lista una storia (es. _Login_) e viene discussa insieme ai committenti tutti i dettagli relativi a questa storia. Successivamente assegniamo alla storia un numero di punti. La storia _Login_ costerà 3 punti d'impegno di sviluppo. Tre è la media del nostro intervallo di storie, con costi da 1 a 6.

La storia _Login_ diventa così la nostra _Golden Story_, ovvero lo standard rispetto al quale verranno considerate tutte le altre storie. E così, per esempio, _Logout_ sarà molto più semplice di _Login_, pertanto assegniamo un 1. Le storie _Versamento_ e _Prelievo_ sono due volte più difficili rispetto a _Login_, pertanto assegniamo a entrambe un 6. A questo punto sorge la domanda: ma quanto durerà una storia da 3 punti? E quella da 6? Ebbene, **gli story point non sono unità di tempo, ma bensì unità d'impegno**. Una storia da 4 punti richiederà il doppio dell'impegno rispetto a una storia da 2 punti. Questi numeri sono vaghi, imprecisi e non sono in relazione diretta con il tempo vero e proprio. Tuttavia ci danno un'indicazione di quanto ci vorrà per sviluppare una storia.

#### Pianificazione dell'iterazione uno

L'iterazione uno inizia con **l'Iteration Planning Meeting (IPM)**. Questo meeting dovrebbe durare un ventesimo della durata dell'iterazione. L'IPM per un'iterazione di due settimane dovrebbe richiedere circa mezza giornata. Al meeting partecipa l'intero team. I committenti avranno precedentemente letto le stime delle storie e le avranno ordinate in base al loro valore commerciale. Essi dovranno scegliere le storie che verranno implementate dai programmatori durante l'iterazione. Per farlo, devono sapere quanti story point gli sviluppatori pensano di poter completare per l'iterazione. Questo numero è chiamato **velocity**. Il team ipotizza che completerà circa 30 punti per questa iterazione. **Questo numero non è un impegno, ma un'ipotesi e probabilmente, essendo la prima iterazione, sarà anche molto impreciso.**

#### Ritorno sull'investimento

![Gioco dei 4 quadranti](<.gitbook/assets/Gioco dei 4 quadranti.png>)

A questo punto i committenti fanno il **Gioco dei 4 quadranti**. Prendono le storie a uno a uno e, posizionandole in uno dei 4 quadranti, calcolano il **ritorno sull'investimento (ROI)**. Le storie utili ed economiche vengono fatte subito. Quelle utili ma costose verranno rimandate. Quelle poco utili, ma economiche verranno fatte, un giorno. Quelle che non sono utili e anche costose non verranno mai fatte. I committenti così sceglieranno le storie che "rendono di più", che hanno il ROI più elevato. Quando ne trovano abbastanza per raggiungere la **velocity** (es. 30 punti), si fermano.

#### La verifica intermedia

A metà iterazione, viene indetto un meeting di verifica tra il team e i committenti per valutare lo stato di avanzamento delle storie. Durante la valutazione dei progressi, se le storie completate non arrivano nemmeno alla metà della velocity che si era prefissata di raggiungere (es. 30 punti), i committenti dovranno rimuovere alcune storie dal piano, in modo da ridurre i punti rimanenti. Questo evento potrebbe risultare deludente per l'intero team, ma non disperate! Avete comunque generato dei dati fondamentali per le successive iterazioni.

#### Il meteo di ieri

Terminata la prima iterazione, adesso sappiamo quanti punti possiamo completare. Facciamo finta che siano 18. Durante l'IPM della seconda iterazione si prenderà come velocity proprio il dato che abbiamo ottenuto dall'iterazione precedente, ovvero 18. Così all'IPM, i committenti selezionano delle storie che assommano a 18 punti. Ma, questa volta, nella verifica intermedia accade qualcosa di strano. Sono pronti 12 punti. I committenti così aggiungono altri 6 punti al piano, con un totale pianificato pari a 24. Il team ne completerà solo 22, che verranno utilizzati come velocity per la successiva iterazione.

#### La fine del progetto

È in questa maniera che viene portato avanti il progetto. A ogni iterazione, la velocità di completamento viene aggiunta al grafico della velocity, in modo che tutti possano vedere qual è la velocità del team. Man mano che si procede in questo "flusso", nuove storie vengono aggiunte e altre completate. Un bel giorno, all'IPM, i committenti guardano le storie e non trovano più nulla. Il progetto è terminato. Il progetto non termina quando sono state completate tutte le storie, ma quando non vi sono più storie che valga la pena implementare.

### User story

Le user story sono semplici affermazioni che impieghiamo per sintetizzare le funzionalità. Le storie seguono un semplice insieme di linee guida, che vanno sotto l'acronimo **INVEST**.

* **I - Independent:** le user story sono indipendenti fra loro. Questo ci consente d'implementare le storie nell'ordine del loro valore commerciale. Questo è un requisito flessibile, perché vi possono essere storie che sono legate in qualche modo (es. la storia _Recupero Password_ è legata alla storia _Login_).
* **N - Negotiable**: questo è un altro motivo per cui non trascriviamo tutti i dettagli all'interno delle storie. Vogliamo che i dettagli siano negoziabili fra gli sviluppatori e l'azienda. Magari i committenti vogliono per una funzionalità un'interfaccia drag-and-drop complicata da realizzare. Gli sviluppatori potrebbero proporre una soluzione alternativa per rendere lo sviluppo della funzionalità molto più economico.
* **V - Valuable**: la storia deve avere un valore commerciale chiaro e quantificabile per l'azienda. Potete utilizzare una scala di 10 punti o un'etichetta basso/medio/alto, purché sia chiaro il valore della storia. Per questa ragione non devono esistere storie come: _Refactoring_, _Miglioramento Architettura_, _Installazione Pacchetti_...
* **E - Estimable**: una user story deve essere sufficientemente concreta da consentire agli sviluppatori di valutarne una stima.
* **S - Small**: una user story deve essere sufficientemente piccola, tale da consentire a uno o due sviluppatori d'implementarla in un'unica iterazione. Un'iterazione dovrebbe contenere all'incirca lo stesso numero di storie di quanti sono gli sviluppatori del team. Un team da 8, dovrebbe contenere da 6 a 12 storie.
* **T - Testable**: l'azienda deve essere in grado di definire dei test che dimostrino che la storia è stata completata. Questi test, chiamati di accettazione, verranno scritti e dettagliati dalla QA.

#### Stima delle storie

Esistono vari metodi per stimare una storia. I più utilizzati sono i seguenti:&#x20;

#### **Flying Fingers**

Gli sviluppatori siedono su una scrivania estraggono una storia selezionata dai committenti, e buttano un numero con le dita. Se tutti gli sviluppatori hanno buttato lo stesso numero esso si assegna la storia, altrimenti si discute tutti assieme dei motivi del discostamento.

#### Planning Poker

Si crea un mazzo di carte con i seguenti valori: 0, 1, 2, 3, 5, 8, ∞ e ?. I numeri da 1 a 8 vengono utilizzati per stimare le storie secondo la loro complessità. Il valore 0 viene utilizzato per indicare che una storia è troppo semplice e banale per stimarla. Il valore ∞ significa che la storia è troppo grande da stimare e occorre spezzarla in più parti. Infine, il valore ? indica che non sapete come valutare la storia e pertanto avete bisogno di uno **spike**.

#### Divisione, unione e spike

Unire le storie è semplice. Prendete le storie da unire e sommate i loro punti. Ricordatevi però che, se unite tante storie che valgono 0, date a loro un nuovo valore.

La divisione va fatte per quelle storie che risultano essere troppo grandi. Ad esempio, la storia _Login_ può essere divisa in _Login con username e password, Login con Google e Login con Facebook_. Ricordatevi però che, suddividendo le storie, dovete sempre curare i fattori "INVEST".

Uno spike è una meta-storia, ovvero una storia per stimare una storia. Viene utilizzato quando non si dispone della conoscenza necessaria per valutare una user story. Ad esempio, la storia _Stampa PDF_ potrebbe essere troppo difficile da valutare se non si conosce la libreria per la stampa del PDF. In questi casi si crea lo spike _Analisi Stampa PDF_.

### Gestione dell'iterazione

L'obiettivo di ogni iterazione è quello di produrre dei dati per l'esecuzione delle storie successive. È molto meglio aver pronto l'80% delle storie che avere tutte le storie pronte solo all'80%. Concentratevi sul portare a completamento le storie.

#### QA e test di accettazione

Al termine dell'IPM la QA deve iniziare immediatamente a scrivere i test di accettazione. Ci aspettiamo che siano tutti pronti prima della metà dell'iterazione. Senza di essi, una parte degli sviluppatori dovrà smettere di lavorare sulle storie. Dopo la metà dell'iterazione, se tutti i test di accettazione sono pronti, la QA dovrebbe mettersi al lavoro sui test della successiva iterazione. Ancora l'IPM non si è tenuto, ma i committenti possono offrire indicazioni sulle storie che verranno scelte.

Avvicinandosi la fine dell'iterazione, gli sviluppatori dovranno fare in modo che le storie passino i rispettivi test di accettazione. La definizione di "finito" è questa: passa i test di accettazione. Non vogliamo arrivare alla fine con due storie "quasi pronte". Se vi sono storie incomplete, esse verranno riallocate alla successiva iterazione. Questa scelta serve per produrre dati concreti e conoscere realmente qual è la velocity del team.

#### La demo

A fine iterazione verranno mostrare le storie completate ai committenti. Durante questo meeting, della durata di un'ora, gli sviluppatori mostreranno come le storie passano i test di accettazione, sia i nuovi che i precedenti, e i test unitari. È meglio che siano i committenti a operare sul sistema, in modo tale che gli sviluppatori non hanno la tendenza a nascondere le cose che non funzionano.

### Velocità

Al termine dell'iterazione verranno aggiornati i grafici di velocity e di burn-down. Su questi grafici vanno registrati solo i punti delle storie che hanno passato i loro test di accettazione. Dopo alcune iterazioni questi grafici si stabiliranno. Il grafico burn-down predice la data della prossima versione milestone. Il grafico della velocity ci dice quanto è ben gestito il team.

#### Velocità crescente

Se si nota una strana pendenza positiva sul grafico della velocity, non significa che il team sta procedendo bene, ma bensì che il project manager sta mettendo pressione al team, il quale inconsciamente modificherà il valore delle proprie stime, per far sembrare che il lavoro proceda velocemente. I punti delle storie sono come una valuta e il team la sta svalutando a causa di una pressione esterna. Lo scopo della stima durante l'IPM è fare in modo che i committenti sappiano quante storie possono essere terminate, così da pianificare i tempi.

#### Velocità in calo

Al contrario, se il grafico della velocità mostra una pendenza negativa, significa che la qualità del codice è scadente. Il team non ha eseguito un'adeguata rifattorizzazione a causa della mancanza dei test unitari. Questa scarsa qualità del codice porta il team a procedere a rilento, genera pressione  e di conseguenza il team tenderà a nascondere il calo della velocità aumentando la stima dei tempi.

#### La Golden Story

Un buon modo per verificare l'inflazione delle stime è quello di confrontare la stima delle storie con la Golden Story, ovvero la storia presa come riferimento per la misurazione di tutte le altre user story. Se la Golden Story _Login_ misurava 3 e adesso la nuova storia _Correggere gli errori nel menu_ ha una stima pari a 10, vuol dire che è in atto una forza inflattiva.

### Piccole release

La pratica Piccole release suggerisce che il team debba rilasciare il proprio software il più frequentemente possibile. L'idea è quella di rilasciare il codice in produzione al termine di ogni iterazione.

#### Git e i test

Al giorno d'oggi impieghiamo Git. A differenza del passato, con Git non abbiamo tempi di blocco sul codice. Ogni sviluppatore può modificare lo stesso modulo. Se durante l'accettazione della modifica avvengono dei conflitti, essi possono essere risolti rapidamente dagli sviluppatori. La rapida frequenza di accettazione e la possibilità di creare un ampio pacchetto di test automatizzato rende a oggi possibile il **Rilascio continuo**.

#### Agile e le piccole release

Agile tende a portare i team a ridurre sempre di più i cicli di rilascio. Alla fine di ogni iterazione, poiché tutte le storie finora selezionate sono complete al 100%, è possibile effettuare il rilascio di tutte le funzionalità prodotte. A quel punto la decisione di eseguire il deployment sarà esclusivamente commerciale. Se i committenti reputano di avere troppe poche funzionalità per eseguire il deploy, esso potrà essere spostato a una iterazione successiva.

### Test di accettazione

La pratica Test di accettazione è una delle meno usate in ambito Agile. Essa dice che: _**i requisiti devono essere specificati dall'azienda.**_

Ma che cos'è una specifica? _****_ Una specifica è un test. Ad esempio:

> Quando l'utente specifica un nome e una password validi e poi fa clic su "Login", il sistema deve presentare la pagina "Welcome".

Questa specifica dice chiaramente agli sviluppatori come il sistema si dovrà comportare dal punto di vista dell'azienda. Una specifica, essendo anche un test, deve poter essere automatizzata.

#### Strumenti e metodologie

Per facilitare la scrittura dei test di accettazione per i non addetti ai lavori, sono nati tutta una serie di strumenti e di metodologie che tentano di suddividere, attraverso un linguaggio "umano", i lati tecnico e commerciale di un test automatizzato. Ma nonostante questo, molte aziende sono riluttanti nella scrittura dei test di accettazione.

#### Behavior-Driven Development (BDD)

Per avvantaggiare le aziende nella scrittura delle specifiche, Dan North cercò di rimuovere il gergo tecnico dei test attraverso l'utilizzo di un linguaggio "meno complicato e più preciso", in questo caso usando tre avverbi: _Given, When_ e _Then_. I sostenitori del BDD suggeriscono che l'azienda possa specificare le funzionalità che desidera implementare, tramite la definizione di scenari, indipendentemente dal fatto che poi questi requisiti possano essere automatizzati e diventare test.

#### La pratica

I test di accettazione sono un impegno collaborativo fra gli analisi dell'azienda, la QA e gli sviluppatori. Gli analisti specificano i percorsi desiderati. La QA scrive i percorsi indesiderati. Essi sono stati assunti per la loro capacità d'immaginare che cosa potrebbe andare storto nel sistema. Gli sviluppatori collaborano con la QA e gli analisti per garantire che i test abbiano senso da un punto di vista tecnico.

#### QA

Questo fa cambiare il ruolo della QA all'interno di un progetto. Invece di andare a testare gli errori e le omissioni alla fine di tutto il progetto, lavorano fin dall'inizio per definire le specifiche e dare dei feedback tempestivi al team di sviluppo, per aiutarlo a prevenire questi errori.

#### Perdere i test finali

Quando la QA agisce manualmente alla fine del progetto, non facciamo altro che creare un collo di bottiglia, perché essa verrà messa sotto pressione per terminare il lavoro il prima possibile, così da poter rilasciare il software in produzione. Sotto pressione, la QA non controllerà tutto il sistema, ma si limiterà soltanto alle parti più importanti, lasciando da parte intere funzionalità. Invece, facendo intervenire la QA fin dall'inizio e automatizzando il processo dei test, questa pressione finale non si verificherà e il sistema potrà essere rilasciato senza problemi in qualsiasi momento.

#### Il problema della QA

Mettendo la QA alla fine del processo emerge un altro grande problema: la scoperta dei difetti porta a un ulteriore slittamento della data di consegna. Chi si avvantaggia di questi difetti? Sia la QA che gli sviluppatori! La prima perché dimostrerà di aver svolto appieno il proprio lavoro di "scovare i difetti". I secondi perché, come in ogni progetto che si rispetti, a inizio progetto hanno affermato: "Ti consegnerò il progetto alla data prefissata, purché non ti aspetti che tutto il sistema funzioni correttamente". Questo atteggiamento porta a considerare i difetti come una cosa buona e un modo per tutelarsi.

#### Gli sviluppatori sono i tester

Questi problemi vengono curati dalla pratica Test di accettazione. La QA scrive i test per le storie presenti in un'iterazione. Gli sviluppatori producono il codice necessario per far sì che il sistema superi questi test, automatizzando il processo durante la fase di build.

### Intero team

Questa pratica ha lo scopo di ridurre la distanza fra il cliente/azienda e i programmatori, per migliorare la comunicazione e rendere più veloce e accurato lo sviluppo software. La parola _**cliente**_ sta a indicare qualcuno che conosce le esigenze degli utenti. In Scrum, questa figura prende il nome di _**Product Owner**_. Questa è la persona che sceglie le storie, definisce le priorità e fornisce un feedback immediato. L'obiettivo della pratica è quello di minimizzare la distanza fisica tra tutti i membri del team (cliente, manager, tester e sviluppatori) mettendo l'intero team all'interno della stessa stanza.

#### Co-locazione

Il modo migliore per consentire questo tipo di comunicazione rapida ed efficiente è quello di far lavorare l'intero team nella stessa stanza. In questa maniera l'intera azienda trae un forte vantaggio, in quanto la comunicazione resta sempre puntuale e precisa.

#### Lavorare in remoto da casa

Oggi con l'ampia diffusione d'Internet e l'elevata ampiezza di banda, è possibile gestire un intero team stando comodamente seduti in casa. I nuovi strumenti messi a disposizione consentono di organizzare meeting veloci, con la possibilità di condividere schermi, grafici e persino frammenti di codice. Questo genere di team funzionano, e anche piuttosto bene, ma, sicuramente, mettere un intero team all'interno della stessa stanza da risultati ancora più sorprendenti, in quanto si elimina ogni fraintendimento e si evitano perdite di comunicazioni non verbali.

### Conclusioni

Le pratiche rivolte all'azienda hanno lo scopo di sanare la divisione fra cliente e sviluppatori. Seguendo queste pratiche, le aziende e gli sviluppatori possono avere un modo semplice e non ambiguo per comunicare.
