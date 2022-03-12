# Pratiche rivolte al team

Le pratiche rivolte al team governano le relazioni fra i membri del team e il prodotto che stanno sviluppando. Le pratiche di cui parleremo sono _Metafora, Passo sostenibile, Proprietà collettiva_ e _Integrazione continua._

### Metafora

Per fare in modo che il team comunichi efficacemente, tutti devono impiegare un vocabolario limitato e disciplinato di termini e concetti. Questo vocabolario aiuta il team a comprendersi più facilmente. Esso fa da tramite tra il linguaggio di business utilizzato dai committenti e il team tecnico.

#### Domain-Driven Design

Nel suo libro _Domain-Driven Design: Tackling Complexity in the Heart of Software_, Eric Evans ha coniato il termine _ubiquitous language_, ovvero il linguaggio / vocabolario utilizzato all'interno del progetto e sul quale tutti concordano (programmatori, tester, manager, QA e clienti). Questo vocabolario di termini supporta i casi d'uso, i requisiti, la struttura, l'architettura e i test di accettazione.

### Passo sostenibile

Come sviluppatori, all'interno di un progetto software, abbiamo l'impegno e il dover di portare a termine lo sviluppo ottenendo il miglior risultato possibile. Per ottenere ciò, abbiamo anche il diritto e il dovere di procedere a un _Passo sostenibile_. Un progetto software è una maratona, non uno sprint. Se si tenta di correre troppo velocemente, producendo ore e ore di straordinari, si rischia di arrivare a metà progetto senza alcuna energia e questo può facilmente farci commettere degli errori nello sviluppo.

#### Impegno

Fare gli straordinari non è un buon modo per dimostrare il vostro impegno al vostro datore di lavoro. Così facendo, mostrate solo che siete dei cattivi pianificatori, che accettate scadenze irrealizzabili, che siete solo un lavoratore e non un professionista. Questo non vuol dire che tutti gli straordinari siano negativi, ma devono trattarsi di circostanze estremamente rare.

#### Sonno

Per la vita di un programmatore, il riposo è fondamentale. Per essere produttivi occorre dormire almeno 7-8 ore a notte. Considerate che ogni ora di sonno mancante, vi costerà circa due ore di lavoro in più.

### Proprietà collettiva

In un progetto Agile, nessuno possiede il codice. Esso è di proprietà dell'intero team. Ogni membro del team può modificare e migliorare ogni modulo del progetto in qualsiasi momento. Il team possiede il codice collettivamente. _Proprietà collettiva_ non significa che non vi sia spazio per le specializzazioni. Tuttavia, anche se vi specializzate, dovete essere in grado di conoscere il funzionamento generale del sistema. Quando un team mette in pratica la _Proprietà collettiva_, la conoscenza risulta distribuita su tutto il team.

### Integrazione continua

Questa pratica esorta il team a integrare continuamente il proprio codice eseguendo build continue. Il codice, prima di essere integrato, deve passare tutti i test delle unità e i test di accettazione.

#### La disciplina delle build continue

Le build continue non dovrebbero mai fallire i test. Se una build fallisce i test, l'intero team si deve mettere al lavoro per risolvere al più presto il problema. Spesso, invece, accade che il team, messo sotto pressione da una deadline, lascia deliberatamente che la build fallisce. Quello che accade è che si decide di rimuovere i test che la build fallisce, con la promessa che "poi" verranno sistemati. Spesso, però, ci si dimentica della pila di test falliti che si pensava di sistemare "dopo". E così, al cliente viene consegnato un sistema che non funziona.

### Standup meeting

Gli standup meeting sono delle riunioni dove ogni membro del team tecnico deve rispondere alle seguenti tre domande:

* Che cosa ho fatto rispetto lo scorso meeting?
* Che cosa farò prima del prossimo meeting?
* Quali ostacoli vedo?

Le caratteristiche di uno standup meeting sono:

* Il meeting è opzionale. I membri del team possono procedere anche senza partecipare
* Può anche non essere proprio "quotidiano"
* Dovrebbe durare una decina di minuti anche per grandi team
* Ogni membro del team ha circa trenta secondi per rispondere alle tre domande

Questo è tutto. Nessuna discussione. Nessuna spiegazione. Gli standup meeting sono fatti per aggiornare gli altri membri del team in maniera rapida e veloce.

### Conclusioni

Le pratiche descritte in questo capitolo aiutano i team a definire il linguaggio da impiegare per comunicare, e anche le aspettative a proposito di come i membri del team si comporteranno l'uno con l'altro e nei confronti del progetto che stanno svolgendo.
