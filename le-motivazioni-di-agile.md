# Le motivazioni di Agile

Lo sviluppo Agile è prima di tutto un impegno a essere un professionista e a promuovere un comportamento professionale. Per adottare bene Agile occorre lavorare in coppie, scrivere dei test, rifattorizzare e produrre progetti "semplici". Occorre lavorare in cicli brevi e comunicare con l'azienda su base regolare e continua.

### Ragionevoli aspettative

Quello che segue è un elenco di aspettative che i manager, gli utenti e i clienti hanno nei nostri confronti. I principi e le pratiche Agile si rivolgono quasi direttamente alla maggior parte delle aspettative di questo elenco.

#### Non consegneremo mai "schifezze"!

È fastidioso dover menzionare questa aspettativa nel nostro settore, ma tutti noi ci siamo trovati a scrivere del codice che, per qualsiasi ragione o causa, era proprio una "schifezza". È perfettamente ragionevole che i nostri manager, clienti e utenti si aspettano da noi che forniamo dei sistemi di alta qualità e perfettamente funzionanti. L'enfasi di Agile su _Testing, Refactoring, Simple Design_ e _feedback continuo_ è il rimedio per evitare di consegnare software di cattiva qualità.

#### Prontezza tecnica continua

Un elemento che spesso caratterizza i progetti software sono i ritardi artificiali. La causa di questi ritardi è spesso dovuta al tentativo di realizzare tutte le funzionalità simultaneamente invece di fornire prima al cliente le funzionalità più importanti. Spesso vengono forniti software quasi pronti o semi-collaudati. Un'altra fonte di ritardi è data dalla fase di QA. Il team si riserva un tempo abbastanza lungo per poter testare il software prima di raccomandare la fase di deploy. L'approccio Agile risolve questi problemi con la regola che il sistema software deve essere _tecnicamente pronto al deploy_ alla fine di ogni iterazione. Questo significa che alla fine di ogni iterazione il codice è pulito, tutti i test vengono passati e il sistema è tecnicamente solido per passare alla fase di deploy.&#x20;

Se il sistema alla fine di ogni iterazione è tecnicamente pronto al deploy, allora _il deployment è una decisione puramente commerciale, non tecnica_. __ L'azienda può decidere che non vi sono sufficienti funzionalità e per questo deve attendere nuove iterazioni. Per raggiungere ogni settimana questa _prontezza tecnica continua_, il team dovrà selezionare un numero di storie sufficientemente piccolo da permetterne il completamento nel giro di un'iterazione. Questa "prontezza tecnica" è necessaria, perché quando l'azienda vede che una funzionalità funziona, si aspetta che essa sia completata del tutto.

#### Produttività stabile

All'inizio di ogni progetto, il team di programmazione procede spedito nell'implementazione delle funzionalità. Questo avviene perché il codice, inizialmente, è ben organizzato e pulito e di conseguenza, non avendo ancora un enorme base di codice, i rallentamenti sono quasi del tutto nulli. Sfortunatamente, mentre il tempo passa, i problemi nel codice possono accumularsi se non viene tenuto pulito e ordinato. Questi problemi inizieranno a creare pressione all'interno del team che inizierà a rallentare sempre di più. Col passare del tempo, ci si ritroverà con una base di codice non mantenibile, dove per implementare una nuova funzionalità occorrono svariate settimane con l'aggravante che questo può portare all'introduzione di nuovi bug all'interno del sistema. In questi casi la soluzione che spesso si adotta (erroneamente) è la riscrittura dell'intero progetto. Questo però porta a due complicazioni: la prima è quella che adesso il team deve sia ri-sviluppare il nuovo progetto e sia mantenere quello vecchio. La seconda è data dal fatto che, pur ri-sviluppando da zero, il nuovo progetto presenterà, presto o tardi, le stesse cattive pratiche del vecchio. La vera soluzione per evitare tutto questo e mantenere stabile la produttività è quella di avere un codice _sempre_ ordinato e pulito. Le pratiche Agile di _Testing, Pair Programming, Refactoring_ e _Simple Design_ aiutano a rispettare questa aspettativa.

#### Adattabilità economica

Gli sviluppatori spesso si lamentano del cambiamento dei requisiti, perché questo può portare a sovvertire l'intero sistema software. Se questo avviene, il vero problema non sta nel cambiamento dei requisiti, ma nell'architettura del progetto. Il software nasce per essere un prodotto facile da modificare, pertanto il costo delle modifiche deve essere limitato e proporzionale. Le pratiche Agile di _TDD, Refactoring_ e _Simple Design_ aiutano a rispettare questa aspettativa.

#### Miglioramento continuo

L'atteggiamento sbagliato che spesso adottiamo come sviluppatori è quello di pensare al sistema software come un qualcosa che col tempo andrà a peggiorare. Un prodotto software, come un qualsiasi altro prodotto realizzato dall'uomo, dovrebbe migliorare nel corso del tempo. Le pratiche Agile di _Pair Programming, TDD, Refactoring_ e _Simple Design_ aiutano a raggiungere questa aspettativa.

#### Competenza senza paura

Il motivo principale per cui i sistemi software non migliorano con il tempo è data dalla nostra paura a modificare e migliorare il codice. Sappiamo che il codice va sistemato, ma abbiamo paura che una nostra modifica possa rompere parti del sistema funzionanti. Questa paura non fa altro che peggiorare la qualità del codice e, man mano che passa il tempo, aggiungere nuovi problemi con tutto quello che ne consegue. L'unico alleato che ci consente di non avere più paura nel modificare il software è: _la suite di test_. Grazie ai test è possibile applicare modifiche al codice ed essere sicuri che, a ogni modifica applicata, non abbiamo introdotto dei nuovi bug. Le pratiche Agile di _TDD, Refactoring, Pair Programming_ e _Simple Design_ ci aiutano a raggiungere questa aspettativa.

#### La QA non dovrebbe trovare nulla

Se il codice è coperto da test, la QA si troverà a testare un sistema "sempre" perfettamente funzionante. Come vedremo, infatti, esiste un posto migliore per collocare la QA. Le pratiche Agile di _Test di accettazione, TDD_ e _Integrazione continua_ supportano questa aspettativa.

#### Automazione dei test

Spesso per testare un software ci si affida a un team QA che esegue manualmente i test a ogni release. Tuttavia, eseguire questi test risulta essere costoso e inefficiente in quanto ci si deve affidare all'attenzione degli esseri umani. Pertanto, ogni test che può essere automatizzato deve essere automatizzato. Le pratiche Agile _TDD, Integrazione continua_ e _Test di accettazione_ supportano questa aspettativa.

#### Ci "copriamo" l'un l'altro

Come in qualsiasi squadra, ci si aspetta che i membri del team si coprano l'un l'altro. Ogni singolo membro di un team software si deve assicurare che ci sia qualcuno che possa coprire la sua mansione qualora si dovesse assentare. All'interno del team la conoscenza deve essere _condivisa_. La semplice assenza di un membro non può portare il progetto ad arenarsi. Le pratiche Agile di _Pair Programming, Intero team_ e _Proprietà collettiva_ supportano questa aspettativa.

#### Stime oneste

Ammettiamolo, fare stime è una delle attività che più detestiamo. Ci viene difficile fare una stima onesta, soprattutto quando non conosciamo bene il progetto o il linguaggio/framework da utilizzare. Tuttavia, possiamo rimediare utilizzando delle stime relative o probabilistiche. Per esempio, non sappiamo quanto tempo ci vorrà per fare la pagina di "Login", ma sappiamo che per la pagina "Cambio password" ci vorrà circa la metà del tempo rispetto a quella di "Login" oppure possiamo dire che la pagina di "Login" richiederà dai 5 ai 15 giorni. Queste stime, anche se non sono del tutto precise, danno un'informazione utile e onesta ai manager. Le pratiche Agile _Planning game_ e _Intero team_ supportano questa aspettativa.

#### Occorre anche dire "No"

Oltre che per le nostre capacità di programmazione, siamo stati assunti anche per dare pareri oggettivi sulle soluzioni ai problemi. Se per un problema non esiste una soluzione pratica, occorre anche saper dire "no, non è possibile risolvere questo problema". La pratica Agile _Intero team_ supporta questa aspettativa.

#### Apprendimento continuo

Il nostro settore cambia rapidamente. Pertanto, dobbiamo essere in grado di cambiare insieme a esso. Come programmatori abbiamo il dovere di tenerci sempre aggiornati per restare a passo con le nuove tecnologie. La pratica Agile _Intero team_ supporta questa aspettativa.

#### Condividere le conoscenze

Come in ogni buon team bisogna condividere le conoscenze. Insegnare agli altri è sia il modo migliore per condividere quello che si sa, ma anche il modo migliore per imparare bene qualcosa. La pratica Agile _Intero team_ supporta questa aspettativa.

### La Carta dei diritti

Durante il meeting di Snowbird, Kent Beck disse che l'obiettivo di Agile era quello di sanare la divisione fra azienda e sviluppatori. A tal riguardo, venne redatta la seguente carta dei diritti. Leggendo i seguenti punti noterete che i diritti del cliente e quelli dello sviluppatore sono complementari. Vanno di pari passo e formano un tutt'uno.

#### Carta dei diritti del cliente

La parola "cliente" in questo contesto include i veri clienti, i manager, i dirigenti e tutti coloro che hanno una responsabilità di tempi e budget.

La carta dei diritti del cliente include quanto segue:

> I clienti hanno il diritto a un piano generale e a sapere che cosa può essere ottenuto, quando e a che prezzo

Ora è innegabile che un cliente debba avere questo diritto, ma è altrettanto innegabile che non è possibile per uno sviluppatore fornire risultati esatti a date certe. O i risultati o la data devono essere flessibili. Pertanto, uno sviluppatore deve dare delle stime probabilistiche. Per esempio, è possibile stimare che ci sia un 80% di probabilità di portare a termine le prime dieci storie entro una certa data. I clienti hanno il diritto a questo tipo di piano probabilistico.

> I clienti hanno il diritto a trarre il massimo valore possibile da ogni iterazione

A ogni iterazione, il cliente ha il diritto di scegliere quali storie forniscono loro il ritorno più elevato per l'investimento e che sono in linea con le stime dei tempi dello sviluppatore.

> I clienti hanno il diritto di vedere i progressi in un sistema funzionante, il cui funzionamento sia dimostrabile tramite il passaggio di test ripetibili specificati dal cliente stesso

Il cliente deve avere la possibilità di vedere rapidamente e ripetutamente che il sistema funzioni secondo i criteri di accettazione da lui definiti

> I clienti hanno il diritto di cambiare idea, funzionalità e priorità senza andare incontro a costi esorbitanti

L'idea stessa del software è quella di cambiare con facilità il comportamento, pertanto deve adattarsi facilmente ai nuovi requisiti del cliente

> I clienti hanno il diritto di essere informati dei cambi di tempi e stime, così da organizzare contromisure in grado di rispettare comunque una determinata data. I clienti possono ritirarsi in qualsiasi momento avendo tra le mani un sistema funzionante che rifletta l'investimento fatto finora

Il cliente ha il diritto di sapere che il calendario dei lavori è a rischio, in modo da poter reagire tempestivamente

#### La carta dei diritti dello sviluppatore

La parola "sviluppatore" in questo contesto include i programmatori, la QA, i tester e gli analisti.

La carta dei diritti dello sviluppatore include quanto segue:

> Gli sviluppatori hanno il diritto di sapere che cosa è richiesto, con precise dichiarazioni delle priorità

Gli sviluppatori devono conoscere con precisione i requisiti e la loro importanza. Anche per i requisiti vale lo stesso discorso fatto per le stime. Non sempre è possibile essere precisi sui requisiti. Il cliente, come già detto, ha il diritto di cambiare idea. Pertanto, questo diritto vale solo nel contesto di un'iterazione. All'intero di un'iterazione gli sviluppatori hanno il diritto di considerare le storie selezionate come immutabili

> Gli sviluppatori hanno il diritto di produrre software di qualità

Gli sviluppatori hanno il diritto di svolgere un buon lavoro. L'azienda non ha il diritto di chiedere agli sviluppatori di lasciar perdere certe cose o di svolgere un lavoro di scarsa qualità

> Gli sviluppatori hanno il diritto di chiedere e ricevere aiuta dai colleghi, dai manager e dai clienti

Gli sviluppatori possono chiedere ai colleghi di dargli una mano a risolvere un determinato problema o possono chiedere ai clienti di spiegare meglio i requisiti

> Gli sviluppatori hanno il diritto di predisporre e aggiornare le loro stime

Le stime sono ipotesi, non sono degli impegni. Gli sviluppatori hanno il diritto di aggiornare le loro stime se entrano in gioco dei nuovi fattori

> Gli sviluppatori hanno il diritto di accettare le proprie responsabilità e non semplicemente di vedersele assegnare

Uno sviluppatore professionista ha ogni diritto di dire "no" a un determinato compito. Magari perché non si sente sicuro di poterlo portare a termine o magari perché crede sia più adatto a qualcun altro. Chi accetta diviene responsabile della qualità e dell'esecuzione del compito.

### Conclusioni

Agile è un framework di discipline che supporta lo sviluppo software professionale. Agile non è solamente un insieme di regole. Agile è un insieme di diritti, aspettative e discipline che formano la base di una professione etica.
