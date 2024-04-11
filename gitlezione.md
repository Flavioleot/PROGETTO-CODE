

Git è un programma utilissimo per modificare, risolvere bug e aggiungere funzione nel codice.
Permette anche a più persone di lavorare contemporaneamente sullo stesso codice.
Tra le sue funzioni possiamo trovare:
1)la creazione di repository: ovvero delle librerie digitali che contengono un singolo progetto( es. codice di un gioco javascript)
Dopo aver installato Git, apri il terminale o la riga di comando e spostati nella cartella del progetto che desideri versionare. Esegui il comando:
bashCopy code
git init
2) ogni volta che si modifica un progetto è possibile tenere traccia di tutte le modifiche, cosa è stato modificato e  da chi.
3) È possibile vedere tutte le versioni precedenti delle parti modificate, grazie alla funzione snapshot.
4) Possibilità di creare "branch" di codice, ovvero parti del codice principale modificabili senza intaccare il codice principale. sviluppare una nuova funzionalità isolata dal ramo principale (solitamente chiamato "master"):
bashCopy code
git branch <nome_ramificazione>
Passa alla nuova ramificazione:
bashCopy code
git checkout <nome_ramificazione>
Quando hai completato il lavoro sulla nuova funzionalità, puoi unire la tua ramificazione al ramo principale:
bashCopy code
git checkout master
git merge <nome_ramificazione>

5) Merging: dà la possibilità di incorporare il codice di una branch nel codice prinicpale senza problemi.Durante il merging, potrebbero verificarsi conflitti se due o più rami hanno modificato le stesse parti dello stesso file. È necessario risolvere i conflitti manualmente e quindi eseguire di nuovo il commit.

Alcuni comandi comuni includono git log per visualizzare la cronologia dei commit, git diff per visualizzare le differenze tra i file e git clone per clonare un repository esistente.
Repository: Sì, git init viene utilizzato per inizializzare un nuovo repository Git in una cartella locale. Questo crea una copia del repository vuoto nella tua directory di lavoro locale, dove puoi iniziare a lavorare e versionare il tuo codice.
1. Tenere traccia delle modifiche: Git tiene traccia delle modifiche attraverso i commit. Ogni volta che fai un commit, stai essenzialmente registrando uno snapshot dello stato del tuo progetto in quel momento. Questo ti consente di monitorare le modifiche nel tempo e di tornare a versioni precedenti del codice se necessario.
2. Snapshot delle versioni precedenti: Esatto, Git mantiene uno storico completo delle modifiche sotto forma di snapshot. Puoi navigare tra queste versioni precedenti per vedere come il codice è cambiato nel tempo e, se necessario, tornare a una versione precedente.
3. Branching e merging: I branch sono una delle caratteristiche più potenti di Git. Consentono di sviluppare nuove funzionalità o lavorare su correzioni di bug in modo isolato, senza influire sul codice principale. Il merging ti consente poi di incorporare le modifiche di un branch in un altro, come ad esempio unire una feature branch nel branch principale (spesso chiamato master o main). È importante notare che i conflitti possono sorgere durante il merging se due o più branch hanno modificato le stesse parti dello stesso file. In tal caso, è necessario risolvere manualmente questi conflitti prima di completare il merge.
4. Comandi comuni: Hai menzionato alcuni comandi comuni come git log, git diff, e git clone, che sono essenziali per navigare e lavorare con repository Git. git log mostra la cronologia dei commit, git diff mostra le differenze tra i file, e git clone è utilizzato per clonare un repository esistente in una nuova directory locale.

Certamente, ecco alcuni comandi aggiuntivi che possono essere utili per utilizzare al meglio Git:
1. git status: Questo comando ti mostra lo stato attuale del tuo repository Git. Mostra quali file sono stati modificati, quali sono stati aggiunti al staging area e quali sono pronti per essere committati. È un buon modo per tenere traccia delle modifiche che hai apportato al tuo codice.
Esempio:
luaCopy code
git status
2. git add: Questo comando viene utilizzato per aggiungere le modifiche dei file al staging area, preparandoli per il commit. Puoi aggiungere file specifici o tutte le modifiche nella directory di lavoro.
Esempio:
csharpCopy code
git add nome_del_file
git add .
3. git commit: Questo comando viene utilizzato per registrare le modifiche nel repository. È necessario fornire un messaggio di commit che descriva le modifiche apportate.
Esempio:
sqlCopy code
git commit -m "Messaggio di commit descrittivo"
4. git push: Quando hai committato le tue modifiche localmente, puoi utilizzare git push per inviare queste modifiche al repository remoto, sincronizzando il tuo repository locale con quello remoto.
Esempio:
perlCopy code
git push origin nome_del_ramo
5. git pull: Questo comando viene utilizzato per scaricare le modifiche dal repository remoto e unirle con il tuo repository locale. È utile per mantenere il tuo repository locale aggiornato con le ultime modifiche fatte da altri collaboratori.
Esempio:
Copy code
git pull origin nome_del_ramo
6. git checkout: Questo comando viene utilizzato per spostarsi tra i branch o ripristinare i file a una determinata versione. Può essere utilizzato anche per creare nuovi branch.
Esempio:
cssCopy code
git checkout nome_del_ramo
git checkout -- nome_del_file
git checkout -b nuovo_ramo
7. git remote: Questo comando viene utilizzato per gestire i repository remoti associati al tuo progetto locale. Puoi aggiungere, rimuovere o visualizzare i repository remoti.
Esempio:
csharpCopy code
git remote add nome_remoto URL_remoto
git remote remove nome_remoto
git remote -v
8. git log: Hai già menzionato git log, ma è utile sottolineare che è possibile personalizzarne l'output e visualizzare solo le informazioni desiderate.
Esempio:
cssCopy code
git log --oneline --graph --decorate --all
Questi sono solo alcuni dei comandi più comuni e utilizzati in Git. Ci sono molte altre funzionalità e opzioni disponibili per ciascun comando, quindi è utile consultare la documentazione ufficiale di Git per saperne di più.
Le cartelle dentro le cartelle, devono essere aperte trascinandole su visula studio code, NON APRIRLE SU GIT.

Per aggiungrere i file, mettere il link che segue https://github.com/Flavioleot/progettocode.git
 Il prompt di windows è diverso da quello del mac!