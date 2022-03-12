# Pratiche di natura tecnica

Molte aziende hanno tentato di applicare Agile senza considerare queste pratiche di natura tecnica. E hanno fallito, perché queste pratiche attengono al nucleo stesso di Agile. Senza _TDD, Refactoring, Simple Design_ e _Pair Programming_, Agile diviene inefficace.

### Test-Driven Development (TDD)

Il Test-Driven Development è una pratica in cui ogni comportamento previsto viene specificato due volte: una volta sotto forma di test e poi di nuovo come codice di produzione che passa i test. I programmatori che applicano il TDD hanno la possibilità d'individuare gli errori nel codice rapidamente e di essere guidati nella progettazione del software stesso. Il Test-Driven Development può essere descritto con tre semplici regole:

* Non scrivere del codice di produzione prima di aver scritto un test che fallisca a causa della mancanza di tale codice
* Non scrivere più test di quanti sono sufficienti per far fallire il programma - e una mancata compilazione conta come un fallimento
* Non scrivere più codice di produzione di quanto è sufficiente per passare il test attualmente fallito

Queste regole implicano un ciclo di programmazione della durata di pochi secondi. Seppur questo _modus operandi_ può sembrare assurdo, esso ci fornisce in realtà un grande aiuto su tutti i fronti.

#### Debugging

Come sarebbero le cose se tutto funzionasse _sempre_ un solo minuto fa? Quanto debugging ci sarebbe da fare? Se tutto funzionava un solo minuto fa, allora quasi ogni problema presente nel codice risalirà a meno di un minuto fa. Probabilmente non occorrerà nemmeno utilizzare il debugger per scovare il problema. Saper utilizzare efficacemente il debugger non fa di voi dei bravi programmatori. Al contrario, se sapete utilizzare perfettamente il debugger, significa che avete dovuto dedicare molto tempo al debugging, in quanto nel vostro codice vi sono sempre parecchi bug.

#### Documentazione

Se seguite le tre regole, i test che scriverete diverranno la documentazione del vostro sistema. Se volete sapere come richiamare una funzione API o come costruire un oggetto, vi sono test che richiamano quella funzione o costruiscono quell'oggetto in tutti i modi possibili. I test sono una forma di documentazione che descrive il sistema sottoposto a test.

#### Completezza

Immaginate che avete del codice di produzione che volete sottoporre a test. Ora immaginate che per scrivere il test che vi serve dovete cambiare un po' la struttura del vostro sistema spezzando alcuni accoppiamenti e/o aggiungendo alcune astrazioni. Questo tipo di modifica costituisce un bel rischio, soprattutto perché il codice già funziona. Vedendo questa situazione vi convincete che non sia necessario scrivere questo test, ma così facendo non fate altro che praticare un "buco" nel pacchetto di test compromettendo di fatto il codice di produzione. Al contrario, se seguite le tre regole, allora ogni riga di codice è stata scritta per passare un test. Pertanto, il pacchetto di test è molto completo e questo vi consente di prendere una decisione: _eseguire il deployment_. Ovviamente non è necessario che i test coprano il 100% del codice per eseguire il deploy. Probabilmente basta il "90 e qualcosa"% per raggiungere questo obiettivo.

#### Progettazione

Vi è mai capitato di aver scritto una funzione così difficile da essere praticamente impossibile da sottoporre a test? L'unico modo per collaudarla sarebbe quello di disaccoppiarla, ma, sapendo che ormai funziona, eviterete di fare ciò. Al contrario, se scrivete i test prima, accade qualcosa di molto differente. Semplicemente non potete scrivere una funzione che sia difficile da sottoporre a test. Poiché scrivete prima i test, progetterete la funzione in modo che sia facile da testare. Per tale ragione, il Test-Driven Development viene spesso considerato una tecnica di progettazione.

#### Coraggio

Uno dei motivi cardine per cui si applica il Test-Driven Development è dato dal fatto che esso infonde "coraggio" allo sviluppatore. Quante volte vi è capitato d'imbattervi in del codice "scritto male" a tal punto da essere costretti a ripulirlo? Quante volte vi siete lasciati sopraffarre dalla paura di poter "rompere il codice funzionante" tanto da abbandonare subito l'idea di ripulirlo? Ebbene, se poteste contare su un pacchetto di test completo, questa paura non esisterebbe e questo vi consentirebbe di mantenere il codice sempre pulito e funzionante.

### Refactoring

La rifattorizzazione è una pratica che consiste nel migliorare la struttura del codice senza alterarne il comportamento. In altre parole, apportiamo modifiche ai nomi, alle classi, alle funzioni e alle espressioni senza fallire nessuno dei test. Naturalmente, questa pratica va a braccetto con il Test-Driven Development. Per rifattorizzare senza timore il codice, abbiamo bisogno di un pacchetto di test che ci fornisca una sicurezza quasi assoluta che non stiamo rovinando nulla.

#### Rosso/Verde/Refactoring

Il processo di rifattorizzazione è fortemente intrecciato con le tre regole del TDD in un ciclo chiamato Rosso/Verde/Refactoring

![Rosso/Verde/Refactoring](.gitbook/assets/red-green-refactor.png)

* Innanzitutto, creiamo dei test che falliscano
* Poi facciamo in modo che il codice passi i test
* Poi ripuliamo il codice
* Infine torniamo al passo 1

L'idea è che scrivere codice funzionante e scrivere codice pulito sono due dimensioni distinte della programmazione. Pertanto, prima ci concentriamo sul fatto che il codice funzioni, per quanto sia sporco. Poi, una volta che funziona, e passa i test, ripuliamo tutto lo sporco che abbiamo lasciato. Il refactoring è quindi un processo continuo e non da svolgere in tempi ben pianificati. Non possiamo accumulare codice sporco e poi tentare di ripulirlo.

### Simple Design

Il _Simple Design_ è uno degli obiettivi del _Rafactoring_. Esso è la pratica dello scrivere solamente il codice affinché la struttura sia il più possibile semplice, compatta ed espressiva. Le regole del Simple Design sono le seguenti:

1. Il codice deve passare tutti i test
2. Il codice deve rivelare lo scopo del programmatore
3. Eliminare ogni duplicazione presente nel codice
4. Ridurre il più possibile gli elementi presenti nel codice

L'elenco comunica sia l'ordine di esecuzione che la priorità.

Il punto 1 è ovvio. Il codice deve funzionare, pertanto, deve passare tutti i test.

Il punto 2 dice che il codice, oltre a funzionare, deve essere facile da leggere e autodescrittivo. Deve rivelare l'intenzione del programmatore.

Il punto 3 dice che dobbiamo eliminare ogni duplicazione presente nel codice. Qui sicuramente ci possono venire in soccorso i Design Patterns.

Il punto 4 dice che, una volta che abbiamo eliminato ogni duplicazione, dobbiamo tentare di ridurre il numero di elementi strutturali, come le classi, le funzioni, le variabili e così via.

L'obiettivo del Simple Design è quello di ridurre il più possibile il _peso del progetto_.

#### Il "peso" di un progetto

Più complessa è la struttura di un progetto, maggiore è il carico cognitivo richiesto per comprendere il progetto stesso. Tale carico cognitivo è il _peso del progetto_. Anche i requisiti di sistema possono andare dal poco al molto complesso. I requisiti complessi, tuttavia, possono essere semplificati impiegando un progetto più complesso. Conseguire questo equilibrio fra complessità del progetto e delle funzionalità è l'obiettivo del Simple Design.

### Pair Programming

Lavorando a coppie, due persone collaborano su un singolo problema di programmazione. La coppia può operare sulla stessa workstation o su due workstation connesse fra loro, sempre che vedano e manipolano lo stesso codice. Nel Pair Programming ci possono essere ruoli differenti. Uno può essere il pilota e l'altro il navigatore. Un'altra possibilità è che un programmatore scriva un test e l'altro il relativo codice di produzione (in questo caso si parla di _Ping-Pong_). Le coppie sono generalmente di breve durata. Una sessione di Pair Programming può durare da un minimo di 15/30 minuti fino a un massimo di 1 giorno, ma spesso sono di un'ora o due.

#### Perché proprio a coppie?

Il lavoro a coppie è il modo migliore per condividere la conoscenza fra i membri del team e impedire la formazione di silos di conoscenza. È il modo migliore per assicurarsi che nessuno, nel team, sia indispensabile. Inoltre, lavorare a coppie è anche un modo più immediato per effettuare una revisione del codice.

#### Il management

I programmatori spesso temono che i manager si lamentino del lavoro a coppie. Se vi trovate in questa situazione e uno dei vostri manager si lamenta che "perdiate tempo", fategli capire che siete voi gli esperti del campo e che pertanto siete voi, e non il manager, a dovervi occupare del metodo di lavoro.

### Conclusioni

Le pratiche di natura tecnica di Agile sono l'ingrediente più essenziale di ogni attività Agile. Senza queste pratiche di natura tecnica a mantenere elevato il livello della qualità del codice, la produttività del team inizierà rapidamente a vacillare ed entrerà inesorabilmente in una spirale mortale.
