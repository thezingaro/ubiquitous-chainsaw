<< [Torna indietro all'indice](../README.md)

- [La documentazione](#la-documentazione)
  - [L'intestazione della Documentazione](#lintestazione-della-documentazione)
  - [Il corpo della Documentazione](#il-corpo-della-documentazione)
  - [Griglia di Valutazione per la documentazione](#griglia-di-valutazione-per-la-documentazione)
- [L'implementazione del progetto](#limplementazione-del-progetto)
  - [La consegna dell'implementazione](#la-consegna-dellimplementazione)
  - [Griglia di Valutazione per l'implementazione](#griglia-di-valutazione-per-limplementazione)
- [La dimostrazione (demo)](#la-dimostrazione-demo)

Globalmente, vengono consegnati due prodotti: la documentazione e l'implementazione (il codice sorgente) del progetto. 
La valutazione finale avviene mediante un esame orale, nella quale vengono discusse le strategie con la quale i prodotti consegnati sono stati generati.
Le domande saranno rivolte a tutti i partecipanti al gruppo, i quali potranno scegliere l'esposizione organizzata dei contenuti.

- non si accettano richieste di eccezioni sui progetti con motivazioni legate a esigenze di laurearsi
- chi copia o fa copiare invalida il progetto - il codice viene controllato con un programma per il rilevamento di plagio - si rimanda alla pagina del tutor per maggiori informazioni sul [codice d'onore](https://spz.netlify.app/teaching/2020/02/24/operative-system-laboratory-computer-science-management) del laboratorio.

## La documentazione

È possibile scrivere la documentazione nel formato preferito, l'importante è che il PDF generato rispetti la struttura del modello (più avanti). 
La documentazione ha lunghezza di **almeno** quattro o cinque pagine (quindi da 8 a 10 facciate), è scritto con font di grandezza _12pt_ e viene consegnato in formato PDF. Il limite è un _lower bound_; non esiste un _upper bound_ per la lunghezza del report che può quindi essere di un numero arbitrario di pagine.

Di seguito viene riportato un esempio di documentazione con le principali caratteristiche da inserire.

### L'intestazione della Documentazione

- Laboratorio Sistemi Operativi A.A. 2019-2020
- Nome del Gruppo
- Indirizzo mail del referente: nome.cognome@studio.unibo.it
- Componenti:
  - Cognome, Nome, Matricola
  - ...

### Il corpo della Documentazione

1. Descrizione generale del progetto
   1. Componenti del progetto
   2. Funzionalità implementate
   3. Contenuto della documentazione
2. Istruzioni per la demo - le istruzioni per eseguire una demo.
3. Discussione sulle strategie di implementazione:
   1. Struttura del progetto - come è stato diviso il progetto tra i componenti del grupppo. Quali sono i problemi principali riscontrati nell'implementazione? Quali sono le alternative considerate? Perché sono state adottate alcune soluzinoi piuttosto di altre?
   2. Sezione di descrizione della  - ad esempio, abbiamo implementato l'operazione `foo` perché abbiamo bisogno di ... Il codice di esempio (riporto il codice) mostra il problema appena descritto ... risolto con ...

In ogni caso motivare le proprie scelte giustificando le proprie azioni.

### Griglia di Valutazione per la documentazione

La valutazione della documentazione verte sull'analisi dello scritto e sulla sua capacità di esprimere con chiarezza i concetti descritti, soprattutto **grazie all'uso di esempi**.

In particolare la griglia di valutazione usata è la seguente:

| Criterio | Descrizione |
|---|---|
| **Qualità dell'informazione** | Riconoscimento dei problemi (di concorrenza) e loro descrizione |
| **Uso degli esempi** | Presenza di almeno un esempio in tutte le scelte implementative |
| **Analisi delle scelte implementative** | Descrizione  della propria scelta implementativa e presenza di proposte di alternative valide |

## L'implementazione del progetto

Il progetto viene sviluppato utilizzando il linguaggio Jolie. 
Non ci sono requisiti riguardo ai protocolli _protocolli_ e i _media_  utilizzati per realizzare la comunicazione tra i componenti del sistema.

La gestione del progetto avviene col supporto del sistema `git`, a [questa pagina](https://education.github.com/git-cheat-sheet-education.pdf) è possibile trovare una lista di comandi utili per imparare ad usare questo strumento di scrittura collaborativa.

Il codice del progetto è contenuto in uno spazio in cloud del servizio online [GitLab](http://gitlab.com) e gestito seguendo la procedura descritta di seguito.

**N.B. Le istruzioni che seguono devono essere completate entro e non oltre la scadenza di presentazione dei gruppi.**

1. Ogni membro del gruppo [crea un account su GitLab o accede con le proprie credenziali](https://gitlab.com/users/sign_in)
2. Il **referente del gruppo** crea un nuovo progetto cliccando sul bottone **+** in alto a destra nella schermata principale di GitLab, inserendo `LabSO_NomeGruppo` come nome del progetto e cliccando su **New Project**
   - una volta che il progetto è stato creato, il referente aggiunge ogni membro del gruppo con `role permission` $>$ `Developer` andando su `Settings` $>$ `Members` nel menù a sinistra, cercandoli in base allo username con il quale questi si sono registrati su GitLab;
   - il referente aggiunge l'utente [`pio_zingaro`](https://gitlab.com/pio_zingaro) con `role permission` $>$ `Reporter`.

### La consegna dell'implementazione

Al momento della consegna, il repository dovrà contenere i sorgenti del progetto e la relazione, nominata `REPORT_LSO.pdf`. 

Per effettuare la consegna:

1. Nella pagina del progetto, cliccare sulla voce del menù `Repository` $>$ `Tags` $>$ `New Tag`
2. Digitare come `Tag Name` il nome **Consegna**
3. Cliccare su `Create Tag` per eseguire la creazione del `Tag` di consegna

Una volta creato il Tag, inviare una email di notifica di consegna con soggetto **CONSEGNA LSO - NOME GRUPPO** a stefanopio.zingaro@unibo.it.

### Griglia di Valutazione per l'implementazione

La valutazione dell'implementazione del sistema si basa sull'analisi del codice Jolie, sull'uso dei costrutti del linguaggio per la creazione di soluzioni efficienti, sulla tolleranza ai guasti del sistema implementato e sulla gestione delle eccezioni.

In particolare la griglia di valutazione usata è la seguente:

| Criterio | Descrizione |
|---|---|
| **Uso dei costrutti di Jolie** | Corretto utilizzo dei costrutti per la gestione della concorrenza, uso corretto di `execution(...)` |
| **Distribuzione del carico di lavoro nel gruppo** | Omogeneità nella ripartizione dei compiti nel gruppo, ogni membro partecipa egualmente allo sviluppo indicando il singolo contributo, assenza di dissimmetria di informazione. |
| **Grado di partecipazione alla comunità** | Presenza di domande e risposte significative sui canali di comunicazione offerti dal corso, richieste di ricevimento e delucidazioni, bug fixing del materiale messo a disposizione del docente e dalla comunità _open source_ di Jolie |

## La dimostrazione (demo)

Insieme alla documentazione ed al codice sorgente, dovrà essere preparato uno script che permette di automatizzare i test. 
Almeno nella fase iniziale della prova orale, può essere utile preparare del materiale da correlare allo script (ad esempio _screenshot_), che permetteranno di velocizzare le operazioni di controllo del codice. 
Tale suite di test _può_ essere intergrata nel codice sorgente (è tuttavia opzionale).
