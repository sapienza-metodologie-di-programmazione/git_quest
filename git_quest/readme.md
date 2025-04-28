# Git Quest: L'Avventura del Controllo di Versione - Istruzioni per gli Avventurieri

Benvenuti, giovani Avventurieri, nel vostro viaggio per padroneggiare le arti del Controllo di Versione con la potente magia di Git! Seguite attentamente queste istruzioni per completare le vostre missioni e diventare veri esperti.

**Setup Iniziale (Guidato dall'Istruttore):**

1.  **Clonare il Repository:** L'Istruttore vi fornirà un link a un repository Git. Utilizzate il seguente comando nel vostro terminale (o Git Bash su Windows) per scaricare il repository sul vostro computer:
    ```bash
    git clone <link_del_repository>
    ```
    *(Sostituite `<link_del_repository>` con l'indirizzo fornito dall'Istruttore).*

2.  **Entrare nel Reame del Progetto:** Una volta scaricato, navigate all'interno della cartella del repository:
    ```bash
    cd git_quest
    ```

**Missioni Autonome (Da completare individualmente, seguendo le indicazioni):**

**Missione 1: L'Esplorazione Iniziale**

1.  Navigate all'interno della **Forgia del Progetto**:
    ```bash
    cd forgia_del_progetto
    ```
2.  Utilizzate la vostra **Vista dello Stato** per osservare l'ambiente circostante e identificare gli artefatti presenti:
    ```bash
    git status
    ```
    *Cosa notate riguardo allo stato dei file `artefatto_1.txt` e `artefatto_2.txt`?*

**Missione 2: La Raccolta e la Registrazione degli Artefatti**

1.  Utilizzate la magia di **Aggiungere al Libro Mastro** per preparare gli artefatti (`artefatto_1.txt` e `artefatto_2.txt`) per la registrazione:
    ```bash
    git add artefatto_1.txt artefatto_2.txt
    ```
    *(Oppure `git add .` per aggiungere tutti i file nella directory corrente.)*
2.  Verificate nuovamente lo **Stato** per assicurarvi che gli artefatti siano pronti per essere registrati:
    ```bash
    git status
    ```
    *Come è cambiato lo stato dei file?*
3.  Sigillate il vostro progresso nel **Libro Mastro** con un **Incantesimo del Commit**:
    ```bash
    git commit -m "Registrati i primi artefatti."
    ```

**Missione 3: L'Esplorazione di Nuove Vie**

1.  Create un nuovo **ramo** chiamato `ramo_esplorazione`:
    ```bash
    git branch ramo_esplorazione
    ```
2.  Verificate quali **rami** esistono ora:
    ```bash
    git branch
    ```
    *Qual è il ramo attivo (indicato dall'asterisco)?*
3.  Passate al nuovo reame (`ramo_esplorazione`) utilizzando l'incantesimo del **Cambio di Reame**:
    ```bash
    git checkout ramo_esplorazione
    ```
4.  Verificate nuovamente il **ramo** attivo:
    ```bash
    git branch
    ```
    *Ora su quale ramo vi trovate?*
5.  Modificate l'**artefatto_2.txt** aggiungendo una vostra "scoperta" o idea. Salvate il file.
6.  Registrate questa modifica nel ramo `ramo_esplorazione` (aggiungendo e committando il file).
7.  Tornate al reame principale (`main` o `master`):
    ```bash
    git checkout main
    ```

**Missioni Guidate (Da completare seguendo le istruzioni dell'Istruttore):**

**Missione 4: Affrontare l'Enigma del Conflitto**

1.  L'Istruttore vi guiderà attraverso una situazione in cui dovrete unire il `ramo_esplorazione` nel ramo principale (`main`).
2.  Eseguite il comando di **Unione**:
    ```bash
    git merge ramo_esplorazione
    ```
    *Se si verifica un conflitto (l'Istruttore simulerà modifiche contrastanti nel file `arena_delle_sfide/enigma_del_conflitto.txt`), l'Istruttore vi spiegherà come visualizzare e risolvere i conflitti direttamente nel file utilizzando un editor di testo.*
3.  Dopo aver risolto il conflitto, aggiungete il file modificato allo staging e completate l'unione con un commit.

**Missione 5: La Ridenominazione della Pergamena**

1.  Seguendo le indicazioni dell'Istruttore, utilizzate la magia di **Ridenominazione** per correggere il nome della pergamena errata:
    ```bash
    git mv arena_delle_sfide/pergamena_da_rinominare.txt nuovo_nome.txt
    ```
    *(Sostituite `nuovo_nome.txt` con il nome indicato dall'Istruttore).*
2.  Registrate la ridenominazione con un commit.

**Missione 6: L'Esplorazione delle Cronache Perdute**

1.  Utilizzate la **Vista della Cronologia** per consultare gli eventi passati (i commit):
    ```bash
    git log --oneline --decorate --graph --all
    ```
    *Osservate la struttura della cronologia, i rami e i commit.*
2.  L'Istruttore vi chiederà di trovare l'**Hash** di un commit specifico (ad esempio, il commit iniziale).
3.  Utilizzando l'**Hash** identificato, provate a tornare a una versione precedente di un artefatto (ad esempio, `artefatto_1.txt`):
    ```bash
    git checkout <hash_del_commit> forgia_del_progetto/artefatto_1.txt
    ```
    *(Sostituite `<hash_del_commit>` con l'hash fornito).*
4.  Osservate lo stato del vostro repository con `git status`. L'Istruttore spiegherà lo stato di "detached HEAD".
5.  Tornate al ramo principale (`main` o `master`):
    ```bash
    git checkout main
    ```

**Missioni Avanzate (Opzionali, guidate dall'Istruttore):**

* Ripristinare Commit Precedenti (`git reset`)
* Annullare Modifiche (`git checkout -- <file>`)
* Collaborare con Rami Remoti (`git push`, `git pull`)

Ricordate, Avventurieri, la pratica rende maestri. Non abbiate paura di sperimentare (con cautela!) e di porre domande al Maestro Git (l'Istruttore). Buona fortuna nella vostra Git Quest!