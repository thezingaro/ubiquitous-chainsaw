In questo spazio presentiamo alcune informazioni utili alla realizzazione del progetto per il corso di Intelligenza Artificiale per la Laurea Magistrale in Informatica dell'Università di Bologna, Anno Accademico 2021-2022.

In particolare, i contenuti di questa pagina riguardano:
1. [la gestione dei gruppi](#gestione-dei-gruppi)
2. [la struttura del progetto](#struttura-del-progetto)
3. [le modalità di valutazione](#modalità-di-valutazione)

**In ogni momento e compatibilmente con la disponibilità dei docenti, è possibile concordare un ricevimento con un messaggio di posta elettronica al [tutor](mailto:stefanopio.zingaro@unibo.it) (specificare la motivazione nella mail).**

# Gestione dei gruppi

Ogni gruppo è composto da un minimo di una (1) ad un massimo di tre (3) persone. 
Coloro che intendono partecipare all'esame comunicano la composizione del gruppo di lavoro **via posta elettronica** al [tutor](mailto:stefanopio.zingaro@unibo.it).
 
Il messaggio deve essere inviato dalla propria mail istituzionale `@studio.unibo.it`, ha come oggetto **GRUPPO AI** e contiene:

1. Il nome del gruppo;
2. Una riga per ogni componente: cognome, nome e matricola;
3. Un indirizzo di posta elettronica di riferimento a cui mandare le notifiche (è incarico del referente trasmettere le eventuali informazioni agli altri membri).

Un esempio del corpo della **mail** con **oggetto** _GRUPPO AI_.

```
| NOME_GRUPPO | NUMERO_COMPONENTI |
|:-|-:|
| [Nome Referente](mailto:nome.referente@studio.unibo.it) | matricola |
| Nome Componente | matricola |
```

L'avvenuta registrazione del gruppo può essere monitorata nella [pagina dedicata](docs/groups.md).
Allo stesso indirizzo è possibile trovare, per coloro che sono alla ricerca di un gruppo, le informazioni di contatto per i referenti e il numero di persone per ogni gruppo esistente.

Chi non riuscisse a trovare un gruppo invia al [tutor](mailto:stefanopio.zingaro@unibo.it) un messaggio con oggetto **CERCO GRUPPO AI**, specificando:

- Cognome, Nome, Matricola, Email;
- Eventuali preferenze legate a tempi di lavoro (si cercherà di costituire gruppi di persone con tempi di lavoro compatibili, nel limite delle possibilità).

Un esempio del corpo della **mail** con **oggetto** _CERCO GRUPPO AI_.

```
Annio Ennio, 123456
A causa di lavoro full-time (in allegato autocertificazione) sono disponibile solo di sera e nei weekend.
```

**Le persone senza un gruppo vengono assegnate il prima possibile senza possibilità di ulteriori modifiche.**

# Struttura del progetto

In generale, il progetto è composto da report (scritto) e implementazione (codice sorgente).
I progetti proposti sono quelli elencati durante la lezione e verranno aggiornati _in itinere_.

# Modalità di valutazione 

Globalmente, vengono consegnati due prodotti: il report (scritto) e l'implementazione (il codice sorgente). 
La valutazione finale avviene mediante un esame orale nel quale vengono discussi il progetto e i prodotti consegnati.
Le domande saranno rivolte a tutti i componenti del gruppo, i quali potranno scegliere come organizzare l'esposizione dei contenuti.

**Non si accettano richieste di eccezioni con motivazioni legate a esigenze di laurearsi.**
**Chi copia o fa copiare invalida il progetto (il codice viene controllato con un programma per il rilevamento di plagio).**

## Il report

Il report è un documento testuale che contiene tutte le informazioni che riguardano gli autori, gli scopi e la realizzazione del progetto.
Concretamente, il report ha le seguenti caratteristiche:

- **non ha limiti di lunghezza** (non esistono _lower bound_ o _upper bound_),
- è scritto con font di grandezza _12pt_,
- è scritto nel formato preferito (e.g., `lateX`, `docx`),
- rispetta la struttura del [modello](#modello-di-report),
- viene consegnato in formato `PDF`.

### Modello di report

Di seguito riportiamo un esempio di indice del report che serva da indicazione sui contenuti principali da inserire.

```
Nome del Progetto
Corso di Laurea
Anno Accademico

Nome del Gruppo
Indirizzo mail del referente: nome.cognome@studio.unibo.it
Componenti:
  - Cognome, Nome, Matricola
  - ...

1. Introduzione
  - Descrizione del problema: perché è un problema?
  - Descrizione della soluzione proposta: come si intende affrontare la realizzazione di una soluzione?
  - [extra] Revisione della letteratura: Accenno alle soluzioni presenti nella letteratura esistente 
  - [extra] Collaborazione: come è stato diviso il progetto tra i componenti del grupppo?
  - Accenno ai risultati ottenuti
2. Metodo
  - Ricerca dell soluzione: quali alternative sono state considerate nella scelta della soluzione proposta?
  - Giustificazione della scelta: perché sono state adottate alcune soluzioni piuttosto di altre?
3. Risultati sperimentali
  - Istruzioni per la dimostrazione
  - Elenco delle tecnologie usate per gli esperimenti
  - Descrizione del metodo per la misurazione delle performance
  - Risultati della configurazione migliore
  - [extra] Comparazione tra le diverse configurazioni
  - [extra] Comparazione con le soluzioni presenti in letteratura
4. Discussione e conclusioni
  - Discussione dei risultati ottenuti (in termini di performance)
  - Il metodo proposto rispetta le attese? Perché sì/no?
  - Quali sono i limiti della soluzione proposta
  - Lavori futuri: come si intende portare avanti il lavoro 
```

**In generale, l'idea è quella di motivare le proprie scelte giustificando le proprie azioni, immaginando che il progetto realizzato debba essere ri-preso da un vostro collega in futuro.**

Le voci `[extra]` **devono** essere discusse nei progetti dei gruppi con un numero di componenti **maggiore o uguale a due (2)** (sono opzionali per i gruppi di un componente). 

### Valutazione del report

La valutazione del report verte sull'analisi dello scritto e sulla sua capacità di esprimere con chiarezza i concetti descritti, soprattutto **grazie all'uso di esempi**.

In particolare la griglia di valutazione usata è la seguente:

| Criterio | Descrizione |
|---|---|
| **Qualità dell'informazione** | Riconoscimento dei problemi e loro descrizione |
| **Uso degli esempi** | Presenza di almeno un esempio in tutte le scelte implementative |
| **Analisi delle scelte implementative** | Descrizione  della propria scelta implementativa e presenza di proposte di alternative valide |

## L'implementazione

Il progetto viene sviluppato utilizzando la tecnologia che si preferisce. 
Non esisteono requisiti riguardo alle tecnologie usate.

La gestione del progetto **avviene col supporto del sistema `git`**, a [questa pagina](https://education.github.com/git-cheat-sheet-education.pdf) è possibile trovare una lista di comandi utili per imparare ad usare questo strumento di scrittura collaborativa.

Il codice del progetto è contenuto in uno spazio in cloud fornito dal servizio online [GitLab](http://gitlab.com) e gestito seguendo la procedura descritta di seguito.

1. Ogni membro del gruppo [crea un account su GitLab o accede con le proprie credenziali](https://gitlab.com/users/sign_in)
2. Il **referente del gruppo** crea un nuovo progetto cliccando sul bottone **+** in alto a destra nella schermata principale di GitLab, inserendo `AI_NomeGruppo` come nome del progetto e cliccando su **New Project**
   - una volta che il progetto è stato creato, il referente aggiunge ogni membro del gruppo con `role permission` $>$ `Developer` andando su `Settings` $>$ `Members` nel menù a sinistra, cercandoli in base allo username con il quale questi si sono registrati su GitLab;
   - il referente aggiunge l'utente [`szingaro`](https://gitlab.com/szingaro) con `role permission` $>$ `Reporter`.

### Valutazione dell'implementazione

La valutazione dell'implementazione del sistema si basa sull'efficienza del codice.

## Consegna 

Al momento della consegna, il repository dovrà contenere i sorgenti del progetto e il report, nominato `REPORT_AI.pdf`. 

Per effettuare la consegna:

1. Nella pagina del progetto, cliccare sulla voce del menù `Repository` $>$ `Tags` $>$ `New Tag`
2. Digitare come `Tag Name` il nome **Consegna**
3. Cliccare su `Create Tag` per eseguire la creazione del `Tag` di consegna

Una volta creato il Tag, inviare una email di notifica di consegna con soggetto **CONSEGNA AI - NOME GRUPPO** al [tutor](mailto:stefanopio.zingaro@unibo.it).

## La dimostrazione (demo)

Insieme alla documentazione ed al codice sorgente, dovrà essere preparato uno script che permette di automatizzare i test. 
Almeno nella fase iniziale della prova orale, può essere utile preparare del materiale da correlare allo script (ad esempio _screenshot_), che permetteranno di velocizzare le operazioni di controllo del codice. 
Tale suite di test _può_ essere intergrata nel codice sorgente (è tuttavia opzionale).


In generale, la valutazione del progetto comprenderà la valutazione dell'implementazione e del report così come verranno esposte in sede di esame orale.
La data presa in considerazione per la consegna dell'implementazione e del report del progetto sarà quella di creazione del **Tag** su [GitLab](https://gitlab.com).
Le istruzioni per la creazione del consegna si trovano nella [pagina dedicata](consegna.md).

## Calendario per l'esame orale
Solo in seguito alle consegne, vengono fissate data ed orario della discussione (notificate alla mail del referente), **il prima possibile dopo la consegna**.

# Note

In generale, non è necessario usare il contenuto del repository ma solo leggerne le informazioni. 
In ogni caso, è possibile scaricare (download) oppure clonare il codice con il comando `git`:

```bash
git clone https://github.com/szingaro/ubiquitous-chainsaw
```

# Licenza

Il presente progetto è rilasciato con licenza GNU v3; per maggiori dettagli consultare il file [LICENSE](LICENSE).
