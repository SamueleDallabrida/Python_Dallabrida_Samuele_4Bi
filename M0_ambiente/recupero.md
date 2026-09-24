# Esercizio 11 — Recupero di file versionati per errore

## Sequenza dei Comandi Eseguiti

# Tracciamento errato dei file temporanei
git add M0_ambiente/temporanei
git commit -m "test(env): aggiunti file temporanei per errore"

# Inserimento regola nel file .gitignore
# Aggiunta riga "M0_ambiente/temporanei/" al file .gitignore

# Rimozione dei file dall'indice mantenendoli sul disco
git rm -r --cached M0_ambiente/temporanei
git add .gitignore
git commit -m "fix(ignore): rimossa cartella temporanei dal tracciamento"

## Spiegazione:

Il file ```.gitignore``` indica a Git quali file o cartelle non devono essere presi in considerazione durante il tracciamento. Tuttavia, le sue regole agiscono esclusivamente sui file che non sono ancora stati committati.  

Se un file o una cartella sono già stati inclusi nel repository tramite un precedente commit, Git continuerà a monitorarli ignorando la regola del ```.gitignore```.   
Per interrompere il tracciamento mantenendo i file sul disco fisso, occorre rimuoverli manualmente dall'indice/staging area usando il comando ```git rm --cached```.   
Una volta registrato il commit della rimozione, la regola nel ```.gitignore``` inizierà a funzionare correttamente.   